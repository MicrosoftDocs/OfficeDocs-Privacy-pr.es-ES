---
title: Coincidencia de datos para solicitudes de derechos del sujeto
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
description: Obtenga información sobre cómo cargar información adicional en Microsoft Priva sobre los interesados.
ms.openlocfilehash: 1339962a1c4dba18a1d0b21d8a2cebb17ad0f91a
ms.sourcegitcommit: f145dff5e387a8e26db2f3a2c7de125978fbacc9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/28/2022
ms.locfileid: "62249200"
---
# <a name="data-matching-for-subject-rights-requests"></a>Coincidencia de datos para solicitudes de derechos del sujeto

Con la coincidencia de datos, las organizaciones pueden permitir a Microsoft Priva identificar a los interesados en función de los valores de datos exactos proporcionados. Esto puede ayudar a aumentar la precisión de la localización del contenido del interesado que corresponde a esos valores de datos tanto para el personal interno como para los usuarios externos con los que interactúa. También simplifica la necesidad de proporcionar campos manualmente durante la creación de solicitudes de derechos de sujeto y proporciona contexto dentro de las solicitudes de derechos del sujeto y para el icono Información general que muestra los elementos con más contenido del interesado. Para obtener más información sobre esa vista, consulte [Buscar y visualizar datos personales en Priva](priva-data-profile.md#items-with-the-most-data-subject-content).

Para usar la característica de coincidencia de datos, deberá ser miembro del grupo de roles De administración de privacidad. Desde dentro de Priva en el [Centro de cumplimiento de Microsoft 365](https://compliance.microsoft.com/), seleccione **Configuración** en la navegación superior y, a continuación, **Coincidencia de datos**. A partir de aquí, deberá definir el esquema de datos personales y proporcionar una carga de datos personales como se muestra a continuación. Ten en cuenta que puedes agregar elementos y puedes eliminar los elementos que agregues a través de la interfaz de usuario. Sin embargo, no puedes modificar un elemento en su lugar desde la interfaz de usuario en este momento.

## <a name="prepare-for-data-import"></a>Preparar la importación de datos

Antes de definir el esquema o cargar datos, deberá identificar el origen de la información del interesado. El formato de archivo requerido es .csv, que puede leer una aplicación como Microsoft Excel. Estructura esta exportación para que los encabezados de columna aparezcan en la primera fila. Estos encabezados deben incluir los nombres de los atributos del esquema de datos personales. Compruebe el formato de los datos en cada campo. Si alguno de los datos contiene comas, envuelve estos valores entre comillas dobles para asegurarse de que no se analizarán en campos independientes.

## <a name="define-the-personal-data-schema"></a>Definir el esquema de datos personales

El esquema de datos personales describirá los atributos de los interesados. Upload este esquema en la primera pestaña del área de configuración de coincidencia de datos. Los archivos necesarios incluyen un archivo XML **de esquema de datos** personales y un **archivo XML del paquete de** reglas.

### <a name="personal-data-schema-xml"></a>XML de esquema de datos personales

El archivo de esquema de datos personales es un archivo XML que definirá los nombres de columna que se esperan.

- Asigne a este archivo de *esquema unpdm.xml*.
- Defina cada nombre de columna con la etiqueta Nombre de campo como se muestra en el ejemplo siguiente.
- Use searchable = "true" para los campos que desea que se puedan buscar, hasta un máximo de cinco campos. Al menos uno de los nombres de campo debe poder buscarse. Sintaxis de ejemplo: `\<Field name="" searchable=""/>`.
- El esquema de datos personales tiene una sección de etiqueta DataStore. Se deben asignar cuatro campos obligatorios a los nombres de los campos: primaryKeyField, upnField, firstNameField, lastNameField.

Por ejemplo, el siguiente archivo XML define un esquema de ejemplo, con cinco campos especificados como buscables: PatientID, MRN, SSN, Teléfono y DOB. PrimaryKeyField se asigna a PatientID, upnField se asigna a MRN, firstNameField se asigna a FirstName y lastNameField se asigna a LastName.

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

Al configurar el paquete de reglas, asegúrese de hacer referencia correctamente al archivo de esquema de datos personales creado anteriormente: pdm.xml. En el siguiente código XML del paquete de reglas de ejemplo, se deben personalizar los siguientes campos para crear el tipo confidencial de coincidencia de datos:

- **Id. rulePack** &  **Id. de PrivacyMatch**: use New-GUID para generar un GUID.
- **Almacén de datos**: este campo especifica el almacén de datos de búsqueda de coincidencia de datos personales que se va a usar. Proporcione el nombre datastore definido de un esquema de datos personales configurado.
- **idMatch**: este campo apunta al elemento principal de la coincidencia de datos personales.
  - **Coincidencias**: especifica el campo que se usará en la búsqueda exacta. Proporcione un nombre de campo que se puede buscar desde el esquema de datos personales.
  - **Clasificación**: este campo especifica la coincidencia de tipo confidencial que desencadena la búsqueda de coincidencia de datos personales. Puede especificar el nombre o el GUID de una clasificación personalizada o integrada existente. Para evitar problemas de rendimiento, si usa un tipo de información confidencial personalizado como elemento Classification en la coincidencia de datos personales, no use un tipo de información confidencial personalizado que coincida con un gran porcentaje de contenido (como "cualquier número" o "cualquier palabra de cinco letras"). Se recomienda agregar palabras clave de compatibilidad o incluir formato en la definición del tipo de información confidencial de clasificación personalizada.
- **Match**: este campo apunta a pruebas adicionales encontradas cerca de idMatch.
  - **Coincidencias**: proporcione cualquier nombre de campo en el esquema de datos personales de DataStore.
- **Recurso**: esta sección especifica el nombre y la descripción del tipo confidencial en varias configuraciones regionales.
  - **idRef**: proporcione GUID para el identificador ExactMatch.
  - **Nombre & descripciones**: personalizar según sea necesario.

En el siguiente ejemplo XML del paquete de reglas, estamos haciendo referencia pdm.xml archivo de ejemplo del paso anterior que crea el XML del esquema de datos personales:

- **Almacén de datos**: el nombre dataStore hace referencia al archivo de esquema que creamos anteriormente: dataStore = "PatientRecords".
- **idMatch**: el valor idMatch hace referencia a un campo que se puede buscar que aparece en el archivo pdm.xml que creamos anteriormente: idMatch matches = "SSN".
  - **Clasificación**: el valor de clasificación hace referencia a un tipo de información confidencial existente o personalizada: classification = "U.S. Social Security Number (SSN)". (En este caso, usamos el tipo de información confidencial existente del número de la seguridad social de Estados Unidos).

Cree un paquete de regla en formato XML (con codificación Unicode), como en el siguiente código de ejemplo. Puede copiar, modificar y usar este ejemplo.

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

## <a name="upload-personal-data"></a>Upload datos personales
Después de definir el esquema de datos personales, puede realizar la carga de datos **personales** en la segunda pestaña de la página de configuración de coincidencia de datos. Cuando seleccione **Agregar**, elija el esquema personal que definió en el primer paso y, a continuación, cargue el archivo que contiene los datos personales.

Puede cargar estos datos personales eligiendo un archivo local o suministrando una dirección URL de SAS a una ubicación Microsoft Azure Storage que contenga el archivo de datos personales.
Si ha preparado un archivo como primer paso de este proceso que se ajusta al esquema creado, puede usar ese archivo para la carga.

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legales

[Declinación de responsabilidades legales de Microsoft Priva](priva-disclaimer.md)
