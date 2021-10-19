---
title: Crear una solicitud de derechos de sujeto en la administración de privacidad
f1.keywords:
- CSH
ms.author: v-jgriffee
author: jmgriffee
manager: laurawi
audience: Admin
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: medium
ms.collection:
- M365-security-compliance
- M365-privacy-management
search.appverid:
- MOE150
- MET150
description: Obtenga información sobre cómo crear una nueva solicitud de derechos de sujeto en la administración de privacidad.
ms.openlocfilehash: 316d515be454b6aceed95f68c6f3da6fa0e7567c
ms.sourcegitcommit: 85e085eb17af8b4efd1f45207445e1b3c3679600
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/19/2021
ms.locfileid: "60478365"
---
# <a name="create-a-subject-rights-request"></a>Crear una solicitud de derechos de sujeto

Los administradores de administración de derechos de sujeto pueden abrir nuevas solicitudes de derechos de sujeto a través de la página principal de solicitudes de derechos de sujeto de la administración de privacidad. Un asistente le guiará a través del proceso de búsqueda de datos personales sobre un interesado e inicio del proceso de cumplimiento de su solicitud.

También puede optar por cargar material adicional para permitir que la administración de privacidad identifique a los interesados en función de los valores de datos proporcionados exactamente. Para obtener más información, vea [Manage data matching](privacy-management-subject-rights-requests-data-matching.md).

## <a name="use-the-subject-rights-request-creation-wizard"></a>Usar el Asistente para creación de solicitudes de derechos de sujeto

1. En el [Centro de cumplimiento de Microsoft 365](https://compliance.microsoft.com/), vaya a la sección Administración de privacidad y seleccione **Solicitudes de derechos de sujeto**.
1. Para iniciar una nueva solicitud, seleccione **Crear una solicitud**.
1. Identifique al interesado que realizó la solicitud y especifique su relación con su empresa.
1. Ejecutaremos una búsqueda predeterminada de elementos relacionados con el interesado. Si desea refinar la búsqueda u obtener una estimación antes de recuperar datos, puede realizar esas selecciones en esta fase. También puede dejar todos los elementos en blanco y pasar al paso siguiente. Para obtener más información sobre las opciones, vea [Definir la configuración de búsqueda y](#define-search-settings) [Refinar la búsqueda.](#refine-your-search)
1. Elija un tipo de solicitud en función de lo que el interesado desea que haga con sus datos. Si su solicitud se relaciona con un reglamento de privacidad de datos específico, también puede seleccionarlo en una lista proporcionada para agregar más contexto. Establecer una fecha límite (obligatoria) facilita la ordenación de las solicitudes que se acercan o vencidas y se resuelven en tiempo y forma. Los tipos de solicitud incluyen:
   - **Access:** proporciona un resumen de la información personal del interesado en poder de su organización en Microsoft 365.
   - **Export:** proporciona un resumen y una exportación de la información personal del interesado, tal como se recopila y se anota durante la revisión.
   - **Lista etiquetada para seguimiento:** genera un resumen de los archivos que los usuarios etiquetan durante la revisión que pueden requerir acciones adicionales fuera de la administración de privacidad. Por ejemplo, es posible que deba facilitar la eliminación de la información personal del interesado según su solicitud. Las etiquetas de revisión de datos personalizadas para solicitudes de derechos de sujeto se pueden administrar en la **Configuración.**
1. Confirme el nombre de esta solicitud y agregue una descripción opcional para su referencia.
1. Revise el resumen de lo que ha escrito durante los pasos anteriores. Cualquier campo se puede editar antes de seleccionar **Crear solicitud**.

### <a name="define-search-settings"></a>Definir la configuración de búsqueda

Al crear una solicitud de derechos de sujeto, puede elegir una o todas estas opciones de búsqueda para buscar datos sobre el asunto:

- **Incluir contenido creado por el** interesado: incluye el contenido creado por el interesado y puede devolver un mayor volumen de datos.
- **Refinar la búsqueda:** esto le permitirá especificar propiedades adicionales que le ayudarán a identificar al interesado. Aquí puede establecer el ámbito de la búsqueda Microsoft 365 recursos o servicios específicos, o seleccionar otras condiciones para ajustar el ámbito de la solicitud. Después de elegir esta opción, se le pedirá que escriba los parámetros de búsqueda personalizados.
- **Obtener una estimación primero:** esto le permite ver la cantidad de datos que esperamos encontrar antes de que los datos se recuperen automáticamente.

### <a name="refine-your-search"></a>Refinar la búsqueda

Si decides refinar la búsqueda al definir la configuración de búsqueda, se te pedirá que rellenes los parámetros de búsqueda avanzados. Puede agregar **identificadores, establecer** **condiciones** y elegir ubicaciones específicas en Microsoft 365 buscar. 

- **Agregar identificadores:** proporcione más información de identificación sobre el interesado, como nombres, direcciones de correo electrónico y/u otras opciones. Separe varios valores en cada campo con un punto y coma.
- **Condiciones:** empiece a agregar condiciones para la búsqueda eligiendo un tipo en el desplegable. Estos tipos corresponden a posibles propiedades de los datos, como el período de tiempo, el tamaño, las etiquetas de retención, los remitentes y los destinatarios, y muchos otros. Seleccione cualquier tipo para agregarlo y, a continuación, establezca las propiedades deseadas. Para las entradas de campo de texto, puede agregar varias palabras clave separadas por puntos y comas. Puede agregar tantos tipos de contenido como desee.
- **Ubicaciones:** puede establecer el ámbito de la búsqueda para que se SharePoint sitios específicos, Teams canales y OneDrive para la Empresa específicas. Para cada ubicación, puede seleccionar todas las instancias, como todos los buzones de correo Exchange o instancias específicas, como el buzón de un usuario. Seleccione el **vínculo Elegir...** de cada ubicación para especificar información sobre instancias específicas. Para obtener ayuda para identificar los términos de búsqueda adecuados, vea lo siguiente:
  - [Administrar sitios en el nuevo SharePoint de](/sharepoint/manage-sites-in-new-admin-center)administración: proporciona instrucciones sobre cómo ordenar y filtrar sitios y cómo buscar un SharePoint sitio. Úselo para buscar direcciones URL para el SharePoint de búsqueda.
  - [Get-Team:](/powershell/module/teams/get-team)proporciona información sobre cómo buscar equipos en Microsoft Teams por propiedades o información específicas. Úse esto para ayudarle a identificar Teams chats y canales.
  - [Acerca OneDrive direcciones URL:](/onedrive/list-onedrive-urls#about-onedrive-urls)proporciona información sobre el formato y las propiedades adecuados para la dirección URL de OneDrive usuario. Úselo para ayudarle a identificar OneDrive sitios en la búsqueda.

Se recomienda revisar cuidadosamente las selecciones para asegurarse de identificar al interesado correcto. Por ejemplo, si busca buzones por su nombre y encuentra varias personas con nombres similares, compruebe el correcto antes de agregarlos a la solicitud.

## <a name="next-steps"></a>Próximos pasos

Una vez que cree la solicitud, verá que aparece en la página de solicitud de derechos del sujeto. Para obtener más información sobre cómo continuar con la revisión, vea [Revisar datos y colaborar en solicitudes](privacy-management-subject-rights-requests-review.md).

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legales

[Declinación de responsabilidades legales de administración de privacidad](privacy-management-disclaimer.md)
