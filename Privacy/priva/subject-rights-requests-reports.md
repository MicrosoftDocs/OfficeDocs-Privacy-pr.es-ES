---
title: Generación de informes y cierre una solicitud
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
description: Obtenga información sobre cómo administrar los paquetes de datos creados por Microsoft Priva para solicitudes de derechos del interesado y satisfacer la solicitud al interesado.
ms.openlocfilehash: 44113c480f81e6ef885de3649d9e04810c776d7c
ms.sourcegitcommit: 3c83e8133a5a71f4e1d76a0b2981ab3ec9cd6602
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/13/2022
ms.locfileid: "66046694"
---
# <a name="generate-reports-and-close-a-request"></a>Generación de informes y cierre una solicitud

**En este artículo**: Comprender el tipo de informes que se generan en solicitudes de derechos del sujeto. Obtenga información sobre los períodos de retención de los datos recopilados y busque instrucciones para entregar resultados al interesado y cerrar la solicitud.

Después de completar la revisión de datos para una solicitud de derechos del interesado, la siguiente fase es generar los informes necesarios para satisfacer la solicitud. Priva creará informes y recopilará los archivos marcados como **Incluir** durante el proceso de revisión de datos. Los archivos seleccionados de estos paquetes de datos se pueden enviar al interesado para completar su solicitud.

## <a name="understanding-reports"></a>Descripción de los informes

Después de seleccionar **Completar revisión** en la fase **Revisar datos** de la solicitud de derechos del interesado, los informes finales de la solicitud comenzarán a generarse automáticamente. En la pestaña **Informes** de la página de detalles de solicitudes de derechos del sujeto, la columna **Estado** indica cuándo está **en curso** la generación del informe y cuándo está **listo para descargarse** un informe. La creación de los informes puede tardar hasta 30 minutos.

Los informes se dividen en dos secciones:
1. **Informes para el interesado**: estos informes contienen información que se puede devolver al interesado como parte del cumplimiento de la solicitud. Aquí es donde encontrará el **paquete de datos** que contiene los archivos que se van a enviar al interesado.
   > [!IMPORTANT]
   > Solo se generará un paquete de datos si marca los elementos como **Incluir** durante la revisión de datos.

   > [!IMPORTANT]
   > Solo se generará un paquete de datos para los tipos de solicitudes **De exportación** y **Acceso** . No se generará un paquete de datos para una **lista etiquetada para la solicitud de seguimiento** . Revise los detalles sobre [los tipos de solicitud de derechos del firmante](subject-rights-requests-create.md#request-types).

2. **Informes para uso interno**: estos informes son para los registros internos de la organización relacionados con la solicitud de derechos del sujeto. Incluyen un registro de auditoría y una lista de todos los archivos a los que aplicó etiquetas durante la revisión de datos con el fin de realizar un seguimiento o realizar más acciones.

> [!NOTE]
> Cuando se generan informes, la organización completa la solicitud enviando los informes adecuados de forma segura al interesado con el fin de satisfacer la solicitud de derechos del interesado. Si el interesado ha solicitado la eliminación de sus datos, es responsabilidad de la organización identificar los elementos para su eliminación y llevar a cabo la eliminación.

## <a name="data-package"></a>Paquete de datos

El paquete de datos de solicitud de derechos del interesado contiene elementos marcados como **Incluir** durante la fase de revisión de datos del proceso. El paquete de datos se genera como un archivo ZIP. Cuando esté listo para su descarga, seleccione la fila del informe en la pestaña **Informes** de la página de detalles de la solicitud de derechos del asunto. Se abrirá un panel flotante con un botón para **descargar** el informe. Las **siguientes instrucciones sobre qué hacer** en el panel flotante proporcionan una referencia rápida sobre cómo trabajar con el contenido.

Cuando esté listo para descargar el paquete de datos, seleccione **Descargar**, busque la descarga y abra el archivo zip descargado.

### <a name="contents-of-the-data-package"></a>Contenido del paquete de datos

El archivo zip del paquete de datos contiene los siguientes elementos:

- Una carpeta denominada **Azure**: esta carpeta contiene los materiales clave para el interesado. Consulte la explicación detallada a continuación.
- Archivos fuera de la carpeta de **Azure** : pueden incluir dos hojas de cálculo denominadas **Resultados** y **Resumen**. Estos archivos fuera de la carpeta de Azure se proporcionan como referencia y los deben usar principalmente los administradores de la organización.

Cuando Priva identifica y recupera archivos para una solicitud de derechos de sujeto, se cambia el nombre de los archivos que exporta en este proceso mediante identificadores únicos para ayudar a proteger los datos personales. Puede hacer referencia cruzada a los nombres únicos con los nombres de archivo originales mediante el archivo **Export_load_file.csv** . Dado que los nombres de archivo originales pueden incluir información confidencial, debe seguir las directivas que se aplican a dicha información.

> [!NOTE]
> Se recomienda revisar cuidadosamente el contenido de esta carpeta y enviar únicamente los archivos necesarios al interesado. Debe evaluar su respuesta para asegurarse de que se adapta a los requisitos de la ley aplicable.

### <a name="azure-folder-contents"></a>Contenido de la carpeta de Azure

Abra la carpeta **de Azure** y, a continuación, abra el archivo **AEDExport.zip** , que contiene otra carpeta de archivos con un nombre largo compuesto por números y letras. Abra la carpeta con el nombre largo para mostrar el contenido que se describe a continuación:

- **Extracted_text_files** carpeta: contiene texto extraído de los archivos nativos (si se admite).
- **Carpeta NativeFiles** : contiene todos los elementos marcados durante la revisión de datos como **Incluidos**, en su formato de archivo nativo. A cada elemento de esta carpeta se le asigna un nombre de archivo único para proteger los datos personales. Puede hacer referencia cruzada a estos nombres únicos con su nombre de archivo original mediante el archivo Export_load_file.csv, que se explica a continuación.
  - Los archivos que se redactaron mediante la función **Anotar** durante el proceso de revisión de datos se encuentran en la carpeta **NativeFiles** y tienen el sufijo "_burn.pdf".
- **Export_load_file.csv** archivo: contiene los nombres de archivo originales para que pueda hacer referencia cruzada a ellos con los nombres de archivo únicos proporcionados en la carpeta NativeFiles.
- **Archivo** de texto de resumen: proporciona un resumen de los tipos de archivos del paquete de datos, el número de archivos y su tamaño.

##### <a name="what-to-do-with-the-folder-contents"></a>Qué hacer con el contenido de la carpeta

Abra la carpeta **de Azure** y los archivos ZIP como se explicó anteriormente. La siguiente tarea consiste en revisar los elementos, determinar qué enviar al interesado y modificar el contenido del archivo ZIP si es necesario.

Por ejemplo, para una solicitud de exportación en la que el interesado quiere recibir una copia de todos los elementos que contienen sus datos personales en poder de la organización, querrá revisar detenidamente los elementos de la carpeta **NativeFiles** y quitar cualquier elemento que no quiera devolver al interesado.

En el caso de una solicitud de acceso en la que el interesado quiera recibir un resumen de toda su información personal en poder de la organización, querrá centrarse en el archivo de texto **Resumen** .

Modifique el archivo ZIP para quitar cualquier contenido que no quiera incluir en el paquete final. Una vez completado, envíe el archivo ZIP de forma segura al interesado que realizó la solicitud de derechos del interesado.

## <a name="audit-log"></a>Registro de auditoría

El registro de auditoría es un archivo CSV que proporciona un registro de la progresión de las fases para cada solicitud de derechos de sujeto. Enumera cada fase del proceso junto con la fecha y hora de finalización, y el nombre de usuario de la persona que completó el paso.

## <a name="tagged-files-reports"></a>Informes de archivos etiquetados

Los informes etiquetados como **Archivos etiquetados como...** son archivos CSV que enumeran los elementos de contenido a los que se aplicaron etiquetas durante el proceso de revisión de datos. Las etiquetas se usan para marcar los elementos de contenido para una mayor atención o acción por parte de la organización. Obtenga más información sobre [la configuración de etiquetas](priva-settings.md#data-review-tags).

## <a name="retention-periods-for-reports-and-data"></a>Períodos de retención para informes y datos

Los informes generados por solicitudes de derechos del firmante y datos asociados, como archivos anotados guardados en Azure, se almacenan durante un período de tiempo especificado. El período de retención predeterminado es de 30 días a partir de la fecha en que se cierra una solicitud de derechos de sujeto.

El período de retención de datos se define en Priva **Configuración** y se aplica a todas las solicitudes de derechos del interesado. Para ver o cambiar el período de retención de datos, siga estos pasos:

1. Desde cualquier lugar de Solicitudes de los interesados Priva, seleccione **Configuración** (el icono de engranaje) en la esquina superior derecha de la pantalla.
2. Seleccione **Períodos de retención de datos** en el panel de navegación izquierdo.
3. En el menú desplegable **Datos recopilados e informes** , seleccione 30 días o 90 días como período de retención.
4. Seleccione **Guardar** para guardar la configuración.

Asegúrese de comprobar que los períodos de retención de datos elegidos cumplen las directivas y las obligaciones legales de su organización.

## <a name="close-the-request"></a>Cerrar la solicitud

Cuando haya realizado todas las acciones necesarias relacionadas con la solicitud de derechos del firmante, marque la solicitud como cerrada; para ello, seleccione **Cerrar la solicitud** en la esquina superior derecha de la página de detalles de la solicitud. Una solicitud cerrada significa que ya no está activa e indica que no se necesita ningún trabajo adicional para satisfacer la solicitud original del interesado a su organización.

Las solicitudes cerradas no se pueden volver a abrir, pero puede volver a la solicitud para ver los detalles y las notas de la solicitud. Los informes de la solicitud se conservan según el período de [retención](#retention-periods-for-reports-and-data) establecido.

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legal

[Microsoft Priva declinación de responsabilidades legal](priva-disclaimer.md)
