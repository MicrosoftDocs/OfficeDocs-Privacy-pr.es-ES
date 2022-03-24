---
title: Generar informes y cumplir una solicitud de derechos de sujeto
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
description: Obtenga información sobre cómo administrar los paquetes de datos creados por Microsoft Priva para solicitudes de derechos de sujeto y cumplir la solicitud al interesado.
ms.openlocfilehash: a72dfb53e4f642cd2c567896c854af2beaedd416
ms.sourcegitcommit: beeb693075ef692e95d679f366301df8517b2ac3
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/23/2022
ms.locfileid: "63765523"
---
# <a name="generate-reports-and-fulfill-a-subject-rights-request"></a>Generar informes y cumplir una solicitud de derechos de sujeto

Después de completar la revisión de datos para una solicitud de derechos de sujeto en Microsoft Priva, puede pasar a cumplir la solicitud. Priva creará informes y recopilará los archivos marcados como **Incluir** durante el proceso de revisión de datos. Los archivos seleccionados de estos paquetes de datos se pueden enviar al interesado para completar su solicitud. Priva también admite el aprovechamiento de la API Microsoft 365 solicitudes de derechos de sujeto para introducir funciones de automatización.

## <a name="understanding-reports"></a>Descripción de informes

Después de seleccionar **Completar revisión en** la fase **revisar** datos de la solicitud de derechos del sujeto, los informes finales de la solicitud empezarán a generarse automáticamente. En la **pestaña Informes** de la página detalles de solicitudes de derechos del sujeto, la columna Estado indica cuándo se está  generando el informe y cuándo está listo para **descargarse un informe**. Puede tardar hasta 30 minutos en terminar de crear los informes.

Los informes se dividen en dos secciones:
1. **Informes para el interesado**: estos informes contienen información que se puede devolver al interesado como parte del cumplimiento de la solicitud. Aquí es donde encontrará el paquete de datos **que contiene los** archivos que puede enviar al interesado.
   > [!IMPORTANT]
   > Solo se generará un paquete de datos si marca elementos como **Incluir durante** la revisión de datos.

   > [!IMPORTANT]
   > Solo se generará un paquete de datos para los tipos de solicitudes **Export** y **Access** . No se generará un paquete de datos para una **lista etiquetada para la solicitud de** seguimiento. Revise los detalles sobre [los tipos de solicitud de derechos de sujeto](subject-rights-requests-create.md#use-the-subject-rights-request-creation-wizard).

2. **Informes para uso interno**: estos informes son para los registros internos de su organización relacionados con la solicitud de derechos de sujeto. Incluyen un registro de auditoría y una lista de todos los archivos a los que aplicó etiquetas durante la revisión de datos para realizar un seguimiento o realizar más acciones.

> [!NOTE]
> Cuando se generan informes, la organización completa la solicitud enviando los informes correspondientes de forma segura al interesado para cumplir la solicitud de derechos del sujeto. Si el interesado ha solicitado la eliminación de sus datos, es responsabilidad de la organización identificar los elementos para su eliminación y llevar a cabo la eliminación.

## <a name="data-package"></a>Paquete de datos

El paquete de datos de solicitud de derechos del sujeto contiene elementos marcados como **Incluir** durante la fase de revisión de datos del proceso. El paquete de datos se genera como un archivo zip. Cuando esté listo para su descarga, seleccione la fila del informe en la pestaña Informes  de la página detalles de la solicitud de derechos del sujeto. Se abrirá un panel desplegable con un botón para **descargar** el informe. Las **siguientes instrucciones sobre qué** hacer en el panel desplegable proporcionan una referencia rápida sobre cómo trabajar con el contenido.

Cuando esté listo para descargar el paquete de datos, seleccione **Descargar**, busque la descarga y, a continuación, abra el archivo zip descargado.

### <a name="contents-of-the-data-package"></a>Contenido del paquete de datos

El archivo zip del paquete de datos contiene los siguientes elementos:

- Una carpeta denominada **Azure**: esta carpeta contiene los materiales clave para el interesado. Vea la explicación detallada a continuación.
- Archivos fuera de la **carpeta de Azure** : pueden incluir dos hojas de cálculo denominadas **Resultados** **y Resumen**. Estos archivos fuera de la carpeta de Azure se proporcionan como referencia y deben ser usados principalmente por los administradores de la organización.

Cuando Priva identifica y recupera archivos para una solicitud de derechos de sujeto, los archivos que exporta en este proceso se renombran con identificadores únicos para ayudar a proteger los datos personales. Puede hacer referencia cruzada a los nombres únicos con los nombres de archivo originales mediante **elExport_load_file.csv** archivo. Dado que los nombres de archivo originales pueden incluir información confidencial, debe seguir las directivas que se aplican a dicha información.

> [!NOTE]
> Se recomienda revisar detenidamente el contenido de esta carpeta y enviar solo los archivos necesarios al interesado. Debe evaluar su respuesta para asegurarse de que está adaptada para cumplir los requisitos de la legislación aplicable.

### <a name="azure-folder-contents"></a>Contenido de la carpeta de Azure

Abra la **carpeta azure** y, **a continuación** , abra el archivoAEDExport.zip, que contiene otra carpeta de archivos con un nombre largo formado por números y letras. Abra la carpeta con el nombre largo para mostrar el contenido descrito a continuación:

- **Extracted_text_files** : contiene texto extraído de los archivos nativos (donde se admite).
- **Carpeta NativeFiles** : contiene todos los elementos marcados durante la revisión de datos como **Incluidos**, en su formato de archivo nativo. Cada elemento de esta carpeta tiene un nombre de archivo único para proteger los datos personales. Puede hacer referencia cruzada a estos nombres únicos con su nombre de archivo original mediante el Export_load_file.csv archivo, que se explica a continuación.
  - Los archivos que se redactó mediante la función **Anotar** durante el proceso de revisión de datos se encuentran en la carpeta **NativeFiles** y tienen el sufijo "_burn.pdf".
- **Export_load_file.csv** : contiene los nombres de archivo originales para que pueda hacer referencia a ellos con los nombres de archivo únicos proporcionados en la carpeta NativeFiles.
- **Archivo de** texto de resumen: proporciona un resumen de los tipos de archivos del paquete de datos, el número de archivos y su tamaño.

##### <a name="what-to-do-with-the-folder-contents"></a>Qué hacer con el contenido de la carpeta

Abra la **carpeta de Azure** y los archivos zip como se explicó anteriormente. La siguiente tarea consiste en revisar los elementos, determinar qué enviar al interesado y modificar el contenido del archivo zip si es necesario.

Por ejemplo, para una solicitud de exportación en la que el interesado desea recibir una copia de todos los elementos que contienen sus datos personales en poder de la organización, querrá revisar estrechamente los elementos de la carpeta **NativeFiles** y quitar cualquier elemento que no desee enviar al interesado.

Para una solicitud de acceso en la que el interesado desea recibir un resumen de toda su información personal en poder de la organización, querrá centrarse en el archivo **de** texto de resumen.

Modifique el archivo zip para quitar cualquier contenido que no desee incluir en el paquete final. Una vez completado, envíe el archivo zip de forma segura al interesado que realizó la solicitud de derechos del sujeto.

## <a name="audit-log"></a>Registro de auditoría

El registro de auditoría es un archivo CSV que proporciona un registro de la progresión de las fases de cada solicitud de derechos de sujeto. Enumera cada fase del proceso junto con la fecha y hora completadas, y el nombre de usuario de la persona que completó el paso.

## <a name="tagged-files-reports"></a>Informes de archivos etiquetados

Los informes etiquetados como Archivos etiquetados **como...** son archivos CSV que indican los elementos de contenido a los que se aplicaron las etiquetas durante el proceso de revisión de datos. Las etiquetas se usan para marcar elementos de contenido para mayor atención o acción por parte de la organización. Obtenga más información [sobre la configuración de las etiquetas](priva-settings.md#data-review-tags).

## <a name="retention-periods-for-reports-and-data"></a>Períodos de retención para informes y datos

Los informes generados por solicitudes de derechos de sujeto y datos asociados, como archivos anotados guardados en Azure, se almacenan durante un período de tiempo especificado. El período de retención predeterminado es de 30 días a partir de la fecha en que se cierra una solicitud de derechos de sujeto.

El período de retención de datos se define en Priva **Configuración** y se aplica a todas las solicitudes de derechos de sujeto. Para ver o cambiar el período de retención de datos, siga los pasos siguientes:

1. Desde cualquier lugar de Priva Subject Rights Requests, **selecciona Configuración** (el icono de engranaje) en la esquina superior derecha de la pantalla.
2. Seleccione **Períodos de retención de datos** en la navegación izquierda.
3. En el **menú desplegable Datos recopilados** e informes, seleccione 30 o 90 días como período de retención.
4. Seleccione **Guardar** para guardar la configuración.

Asegúrese de comprobar que los períodos de retención de datos elegidos cumplen con las directivas y obligaciones legales de su organización.

## <a name="integrate-with-partner-solutions"></a>Integrar con soluciones de partners

Puede integrar la solución Priva Subject Rights Requests con sus herramientas y procesos empresariales existentes aprovechando la API Microsoft 365 solicitud de derechos del sujeto. Esto le ofrece una forma sencilla pero eficaz de introducir la automatización en su estrategia de derechos de sujeto.

Cuando los interesados solicitan información de su organización, puede aprovechar nuestras API para crear dichas solicitudes dentro de Microsoft 365 según los criterios personalizados para esa solicitud. Puede crear la solicitud de derechos de sujeto en Microsoft 365, realizar un seguimiento del progreso de la solicitud a través de sus fases y confirmar cuándo la solicitud ha completado el procesamiento y el contenido está listo para recuperarse. Nuestras API están disponibles para que cualquier persona pueda usarlas para hacer que sus soluciones sean más extensibles: ya sea para isv, partners para adaptarse a Microsoft 365 en sus soluciones o para que las organizaciones las usen con su línea de aplicaciones empresariales.

Para obtener más información, vea [Use the Microsoft Graph subject rights request API](/graph/api/resources/subjectrightsrequest-subjectrightsrequestapioverview).

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legales

[Declinación de responsabilidades legales de Microsoft Priva](priva-disclaimer.md)
