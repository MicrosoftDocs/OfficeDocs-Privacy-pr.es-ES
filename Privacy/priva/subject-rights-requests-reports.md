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
ms.openlocfilehash: 9931422434414146601ede959af910caf1befcc1
ms.sourcegitcommit: 1f3f2757f456628ec904bc3df985b00ffba8f892
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 02/11/2022
ms.locfileid: "62542838"
---
# <a name="generate-reports-and-fulfill-a-subject-rights-request"></a>Generar informes y cumplir una solicitud de derechos de sujeto

Después de completar la revisión de datos para una solicitud de derechos de sujeto en Microsoft Priva, puede pasar a solicitar el cumplimiento. Priva creará informes y recopilará los archivos marcados para **Incluir** durante el proceso de revisión de datos. Los archivos seleccionados de estos paquetes de datos se pueden enviar al interesado para completar su solicitud. Priva también admite el aprovechamiento de la API Microsoft 365 solicitudes de derechos de sujeto para introducir funcionalidades de automatización.

## <a name="prepare-final-reports-for-the-data-subject"></a>Preparar informes finales para el interesado

El paquete de datos de solicitud de derechos del sujeto se genera como un archivo zip. Puede tardar hasta 30 minutos en generar este paquete. Cuando esté listo, abra la solicitud de derechos del sujeto desde la página solicitudes de derechos del sujeto, abra  la pestaña Informes, busque la descarga y abra el archivo zip.

El paquete de datos contiene una variedad de archivos. Los archivos fuera de la carpeta de Azure se proporcionan como referencia y deben ser usados principalmente por los administradores. Los materiales clave para el interesado se encuentran en la **carpeta de Azure** .

Se recomienda revisar detenidamente el contenido de esta carpeta y enviar solo los archivos necesarios al interesado. Debe evaluar su respuesta para asegurarse de que está adaptada para cumplir los requisitos de la legislación aplicable.

### <a name="azure-folder-contents"></a>Contenido de la carpeta de Azure

Abra esta carpeta y, a continuación **, abraAEDExport.zip** archivo. El contenido incluye:

- La **Extracted_text_files** contiene texto extraído de los archivos nativos (donde se admite).
- La **carpeta NativeFiles** contiene todos los **elementos Incluidos** en su formato de archivo nativo.
- Los archivos redactados se encuentran en la **carpeta NativeFiles** y tienen el sufijo "_burn.pdf".
- Los archivos exportados se renombran con identificadores únicos para ayudar a proteger los datos personales. Puede hacer referencia cruzada a los nombres únicos con los nombres de archivo originales mediante el **Export_load_file.csv**. Dado que los nombres de archivo originales pueden incluir información confidencial, debe seguir las directivas que se aplican a dicha información.

Después de revisar el contenido del archivo zip, modifiquelo según sea necesario para quitar cualquier contenido que no desee incluir en el paquete final. Una vez completado, envíelo de forma segura al interesado.

## <a name="integrate-with-partner-solutions"></a>Integrar con soluciones de partners

Puede integrar la solución Priva Subject Rights Requests con sus herramientas y procesos empresariales existentes aprovechando la API Microsoft 365 solicitud de derechos del sujeto. Esto le ofrece una forma sencilla pero eficaz de introducir la automatización en su estrategia de derechos de sujeto.

Cuando los interesados solicitan información de su organización, puede aprovechar nuestras API para crear dichas solicitudes dentro de Microsoft 365 según los criterios personalizados para esa solicitud. Puede crear la solicitud de derechos de sujeto en Microsoft 365, realizar un seguimiento del progreso de la solicitud a través de sus fases y confirmar cuándo la solicitud ha completado el procesamiento y el contenido está listo para recuperarse. Nuestras API están disponibles para que cualquier persona pueda usarlas para hacer que sus soluciones sean más extensibles: ya sea para isv, partners para acomodar Microsoft 365 en sus soluciones o para que las organizaciones las usen con su línea de aplicaciones empresariales.

Para obtener más información, consulte [Use the Microsoft Graph subject rights request API](/graph/api/resources/subjectrightsrequest-subjectrightsrequestapioverview).

## <a name="manage-data-retention"></a>Administrar la retención de datos

Los informes generados a través de esta herramienta y los datos asociados, como los archivos anotados guardados en Azure, se almacenan durante un período de tiempo especificado. El período de retención de datos se define en Priva **Configuración** y se aplica a todas las solicitudes de derechos de sujeto. Para ver o cambiar los períodos de retención de datos, siga los pasos siguientes:

1. Desde cualquier lugar de Priva Subject Rights Requests, **selecciona Configuración** (el icono de engranaje) en la esquina superior derecha de la pantalla.
2. Seleccione **Períodos de retención de datos** en la navegación izquierda.
3. Con el menú desplegable, seleccione 30 días o 90 días como período de retención.

Asegúrese de comprobar que los períodos de retención de datos elegidos cumplen con las directivas y obligaciones legales de su organización.

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legales

[Declinación de responsabilidades legales de Microsoft Priva](priva-disclaimer.md)
