---
title: Coincidencia de datos para solicitudes de derechos del interesado
f1.keywords:
- CSH
ms.author: chvukosw
author: chvukosw
manager: laurawi
audience: Admin
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: medium
ms.collection:
- M365-security-compliance
- M365-priva-subject-rights-requests
search.appverid:
- MOE150
- MET150
description: Obtenga información sobre cómo cargar información adicional a Microsoft Priva sobre los interesados.
ms.openlocfilehash: 90ee0e8e21d25954c11113992cbb7ece847c85ab
ms.sourcegitcommit: 6b88d22d0250cbb9a4ba1f71665f29cb67939851
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/05/2022
ms.locfileid: "65059744"
---
# <a name="data-matching-for-subject-rights-requests"></a>Coincidencia de datos para solicitudes de derechos del interesado

Con la coincidencia de datos, las organizaciones pueden permitir que Microsoft Priva identifique a los interesados en función de los valores de datos proporcionados exactamente. Esto puede ayudar a aumentar la precisión de la ubicación del contenido del interesado que se corresponde con esos valores de datos tanto para el personal interno como para los usuarios externos con los que interactúa. También simplifica la necesidad de proporcionar campos manualmente durante la creación de solicitudes de derechos del interesado, y proporciona contexto dentro de las solicitudes de derechos del sujeto y para el icono Información general que muestra los elementos con la mayoría del contenido del interesado. Para obtener más información sobre esa vista, consulte [Búsqueda y visualización de datos personales en Priva](priva-data-profile.md#items-with-the-most-data-subject-content).

Para usar la característica de coincidencia de datos, deberá ser miembro del grupo de roles Administración de privacidad. En Priva en el [portal de cumplimiento de Microsoft Purview](https://compliance.microsoft.com/), seleccione **Configuración** en la navegación superior y, a continuación, **Coincidencia de datos**. Desde aquí, tendrá que definir el esquema de datos personales y proporcionar una carga de datos personales como se muestra a continuación. Tenga en cuenta que puede agregar elementos y eliminar elementos que agregue, pero no puede modificar un elemento.

## <a name="prepare-for-data-import"></a>Preparación para la importación de datos

Antes de definir el esquema o cargar datos, deberá identificar el origen de la información del interesado. El formato de archivo necesario es .csv, que puede leer una aplicación como Microsoft Excel. Estructura esta exportación para que los encabezados de columna aparezcan en la primera fila. Estos encabezados deben incluir los nombres de los atributos del esquema de datos personales. Compruebe el formato de los datos en cada campo. Si alguno de los datos contiene comas, envuelve estos valores entre comillas dobles para asegurarse de que no se analizarán en campos independientes.

## <a name="define-the-personal-data-schema"></a>Definición del esquema de datos personales

El primer paso para configurar la coincidencia de datos es definir el esquema de datos personales, que describirá los atributos de los interesados. Cargará este esquema en la primera pestaña del área de configuración de coincidencia de datos. Los archivos necesarios incluyen un archivo XML de **esquema de datos personales** y un archivo XML **de paquete de reglas** .

### <a name="personal-data-schema-xml"></a>XML del esquema de datos personales

El archivo de esquema de datos personales es un archivo XML que definirá qué nombres de columna se esperan.

- Asigne a este archivo de esquema *el nombrepdm.xml*.
- Defina cada nombre de columna mediante la etiqueta Nombre de campo, como se muestra en el ejemplo siguiente.
- Use searchable = "true" para los campos en los que desea que se puedan buscar, hasta un máximo de cinco campos. Al menos uno de los nombres de campo debe poder buscarse. Sintaxis de ejemplo: `\<Field name="" searchable=""/>`.
- El esquema de datos personales tiene una sección de etiqueta DataStore. Se deben asignar cuatro campos obligatorios a los nombres de campo: primaryKeyField, upnField, firstNameField, lastNameField.

Por ejemplo, el siguiente archivo XML define un esquema de ejemplo, con cinco campos especificados como searchable: PatientID, MRN, SSN, Teléfono y DOB. PrimaryKeyField se asigna a PatientID, upnField se asigna a MRN, firstNameField se asigna a FirstName y lastNameField se asigna a LastName.

Puede copiar, modificar y usar nuestro ejemplo.

 ```xml
<PdmSchema xmlns="http://schemas.microsoft.com/office/2020/pdm">
      <DataStore name="Patientrecords" description="Schema for patient records" version="1" primaryKeyField="PatientID" upnField="MRN" firstNameField="FirstName" lastNameField="LastName">
            <Field name="PatientID" searchable="true"/>
            <Field name="MRN" searchable="true" />
            <Field name="FirstName" />
            <Field name="LastName" />
            <Field name="SSN" searchable="true" />
            <Field name="Phone" searchable="true" />
            <Field name="DOB" searchable="true" />
            <Field name="Gender" />
            <Field name="Address" />
      </DataStore>
</PdmSchema>
 ```

### <a name="rule-package-xml"></a>XML del paquete de reglas

Al configurar el paquete de reglas, asegúrese de hacer referencia correctamente al archivo de esquema de datos personales creado anteriormente: pdm.xml. En el siguiente xml de paquete de reglas de ejemplo, los siguientes campos deben personalizarse para crear el tipo confidencial de coincidencia de datos:

- **Identificador de RulePack** &  **Id. de PrivacyMatch**: use New-GUID para generar un GUID.
- **Almacén de datos**: este campo especifica el almacén de datos de búsqueda de coincidencias de datos personales que se va a usar. Proporcione el nombre definido de DataStore de un esquema de datos personales configurado.
- **idMatch**: este campo apunta al elemento principal para la coincidencia de datos personales.
  - **Coincidencias**: especifica el campo que se va a usar en la búsqueda exacta. Proporcione un nombre de campo que permite búsquedas desde el esquema de datos personales.
  - **Clasificación**: este campo especifica la coincidencia de tipos confidenciales que desencadena la búsqueda de coincidencias de datos personales. Puede especificar el nombre o el GUID de una clasificación personalizada o integrada existente. Para evitar causar problemas de rendimiento, si usa un tipo de información confidencial personalizada como elemento Classification en la coincidencia de datos personales, no use un tipo de información confidencial personalizada que coincida con un gran porcentaje de contenido (como "cualquier número" o "cualquier palabra de cinco letras"). Se recomienda agregar palabras clave auxiliares o incluir formato en la definición del tipo de información confidencial de clasificación personalizada.
- **Coincidencia**: este campo apunta a pruebas adicionales encontradas en la proximidad de idMatch.
  - **Coincidencias**: proporcione cualquier nombre de campo en el esquema de datos personales para DataStore.
- **Recurso**: en esta sección se especifica el nombre y la descripción del tipo confidencial en varias configuraciones regionales.
  - **idRef**: proporcione guid para exactmatch id.
  - **Nombre & descripciones**: personalice según sea necesario.

En el ejemplo XML del paquete de reglas siguiente, estamos haciendo referencia al archivo de ejemplo pdm.xml del paso anterior que crea el XML del esquema de datos personales:

- **Almacén de datos**: el nombre del almacén de datos hace referencia al archivo de esquema que creamos anteriormente: dataStore = "PatientRecords".
- **idMatch**: el valor de idMatch hace referencia a un campo que permite búsquedas que aparece en el archivo pdm.xml que creamos anteriormente: idMatch coincide con = "SSN".
  - **Clasificación**: el valor de clasificación hace referencia a un tipo de información confidencial existente o personalizado: classification = "U.S. Social Security Number (SSN)". (En este caso, usamos el tipo de información confidencial existente del número de la seguridad social de Estados Unidos).

Cree un paquete de reglas en formato XML (con codificación Unicode), como en el código de ejemplo siguiente. Puede copiar, modificar y usar este ejemplo.

 ```xml
<RulePackage xmlns="http://schemas.microsoft.com/office/2020/pdm">
  <RulePack id="fd098e03-1796-41a5-8ab6-198c93c62b21">
    <Version build="0" major="2" minor="0" revision="0" />
    <Publisher id="eb553734-8306-44b4-9ad5-c388ad970528" />
    <Details defaultLangCode="en-us">
      <LocalizedDetails langcode="en-us">
        <PublisherName>IP DLP</PublisherName>
        <Name>Health Care PDM Rulepack</Name>
        <Description>This rule package contains the Personal Data Match sensitive type for health care sensitive types.</Description>
      </LocalizedDetails>
    </Details>
  </RulePack>
  <Rules>
    <PrivacyMatch id = "E1CC861E-3FE9-4A58-82DF-4BD259EAB381" patternsProximity = "300" dataStore ="PatientRecords" recommendedConfidence = "65" >
      <Pattern confidenceLevel="65">
        <idMatch matches = "SSN" classification = "U.S. Social Security Number (SSN)" />
      </Pattern>
      <Pattern confidenceLevel="75">
        <idMatch matches = "SSN" classification = "U.S. Social Security Number (SSN)" />
        <Any minMatches ="3" maxMatches ="6">
          <match matches="PatientID" />
          <match matches="MRN"/>
          <match matches="FirstName"/>
          <match matches="LastName"/>
          <match matches="Phone"/>
          <match matches="DOB"/>
        </Any>
      </Pattern>
    </PrivacyMatch>
    <LocalizedStrings>
      <Resource idRef="E1CC861E-3FE9-4A58-82DF-4BD259EAB381">
        <Name default="true" langcode="en-us">Patient SSN Exact Match.</Name>
        <Description default="true" langcode="en-us">PDM Sensitive type for detecting Patient SSN.</Description>
      </Resource>
    </LocalizedStrings>
  </Rules>
</RulePackage>
 ```

## <a name="sensitive-info-types"></a>Tipos de información confidencial

El segundo paso para configurar la coincidencia de datos es crear tipos de información confidencial únicos para la coincidencia de datos personales (PDM). [Los tipos de información confidencial (SIT)](/microsoft-365/compliance/sensitive-information-type-learn-about) son clasificadores basados en patrones que detectan información confidencial, como números de seguro social o tarjetas de crédito. La configuración de un tipo de información confidencial de PDM permite usar valores de datos exactos en lugar de valores genéricos para detectar coincidencias. Para comenzar este paso, seleccione **Crear tipo de información confidencial de PDM** para iniciar el asistente para la creación.

## <a name="upload-personal-data"></a>Upload datos personales

Después de definir el esquema de datos personales y los tipos de información confidencial, el tercer paso es cargar datos personales. Vaya a la pestaña **Carga de datos personales** , seleccione **Agregar** y elija el esquema personal que definió en el primer paso y, a continuación, cargue el archivo que contiene los datos personales.

Para cargar estos datos personales, elija un archivo local o proporcione una dirección URL de SAS a una ubicación de Microsoft Azure Storage existente que contenga el archivo de datos personales.
Si preparó un archivo como primer paso de este proceso que se ajusta al esquema creado, puede usar ese archivo para la carga.

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legal

[Declinación de responsabilidades legal de Microsoft Priva](priva-disclaimer.md)
