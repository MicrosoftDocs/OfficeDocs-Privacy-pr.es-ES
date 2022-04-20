---
title: Creación de una solicitud de derechos de sujeto
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
description: Obtenga información sobre cómo crear una nueva solicitud de derechos de sujeto en Microsoft Priva.
ms.openlocfilehash: b2d846aa4020be315705bbd16e00378c7514146c
ms.sourcegitcommit: 09ecdaded9a9f8f79587f2acb978dc53b83e5c01
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/19/2022
ms.locfileid: "64930611"
---
# <a name="create-a-subject-rights-request"></a>Creación de una solicitud de derechos de sujeto

Los administradores de administración de derechos del firmante pueden abrir nuevas solicitudes a través de la página principal solicitudes de derechos del sujeto de Priva. Un asistente le guiará a través del proceso de búsqueda de datos personales sobre un interesado e iniciar el proceso de satisfacer su solicitud.

También puede optar por cargar material adicional para permitir que Priva identifique a los interesados en función de los valores de datos suministrados exactamente. Para más información, consulte [Coincidencia de datos para solicitudes de derechos del interesado](subject-rights-requests-data-match.md).

## <a name="request-types"></a>Tipos de solicitud

Priva Subject Rights Requests admite tres tipos diferentes de solicitudes:

1. **Acceso**: proporciona un resumen de la información personal del interesado en su organización en Microsoft 365.

2. **Exportar**: proporciona un resumen y un archivo exportado de elementos de contenido que contienen la información personal del interesado. Estos son los elementos revisados y marcados como **Incluidos** durante la revisión de los datos recopilados por la configuración de búsqueda.

3. **Lista etiquetada para seguimiento**: genera un resumen de los archivos etiquetados durante la revisión de datos que pueden requerir una acción adicional fuera de Priva. Por ejemplo, es posible que deba facilitar la eliminación de la información personal del interesado según su solicitud. Puede ver las etiquetas incluidas y configurar etiquetas personalizadas para su organización en [Configuración de Priva](priva-settings.md).

## <a name="use-the-subject-rights-request-creation-wizard"></a>Uso del Asistente para la creación de solicitudes de derechos del firmante

1. En el [portal de cumplimiento de Microsoft Purview](https://compliance.microsoft.com/), vaya a la sección Priva y seleccione **Solicitudes de derechos de sujeto priva**.
1. Para iniciar una nueva solicitud, seleccione **Crear una solicitud**.
1. Identifique al interesado que realizó la solicitud y especifique su relación con su empresa.
1. Ejecutaremos una búsqueda predeterminada de elementos relacionados con el interesado. Si desea refinar la búsqueda u obtener una estimación antes de recuperar datos, puede realizar esas selecciones en esta fase. También puede dejar todos los elementos en blanco y pasar al paso siguiente. Para obtener más información sobre las opciones, vea [Definir la configuración de búsqueda](#define-search-settings) y [Refinar la búsqueda](#refine-your-search).
1. Elija un tipo de solicitud en función de lo que el interesado quiere que haga con sus datos. Si su solicitud está relacionada con un reglamento de privacidad de datos específico, también puede seleccionarlo en una lista proporcionada para agregar más contexto. Establecer una fecha límite (obligatoria) facilita la ordenación de las solicitudes que se aproximan o vencidas y las resuelve de forma oportuna. Los tipos de solicitud incluyen:
   - **Acceso**: proporciona un resumen de la información personal del interesado en su organización en Microsoft 365.
   - **Exportar**: proporciona un resumen y una exportación de la información personal del interesado, tal como se recopila y anota durante la revisión.
   - **Lista etiquetada para seguimiento**: genera un resumen de los archivos que los usuarios etiquetan durante la revisión y que pueden requerir una acción adicional fuera de Priva. Por ejemplo, es posible que tenga que facilitar la eliminación de la información personal del interesado según su solicitud. Las etiquetas de revisión de datos personalizadas para solicitudes de derechos del interesado se pueden administrar en **Configuración globales.**
1. Confirme el nombre de esta solicitud y agregue una descripción opcional como referencia.
1. Revise el resumen de lo que ha escrito durante los pasos anteriores. Cualquier campo se puede editar antes de seleccionar **Crear solicitud**.

Para cada solicitud de derechos de sujeto, puede establecer la búsqueda para buscar datos en todas o ubicaciones específicas dentro de Exchange y Sharepoint. Elija una ubicación moviendo su modificador de alternancia a la posición **Activado** . Puede elegir buscar en todas las cuentas y sitios o designar cuentas o sitios específicos dentro de cada ubicación. Lea los detalles siguientes sobre lo que se trata en cada ubicación.

- **Exchange**: esta opción buscará datos en buzones de Exchange y en chats Teams individuales o grupales. Puede elegir buscar en todas las cuentas de Exchange de su organización o seleccionar **Elegir cuentas** para seleccionar usuarios individuales en el panel flotante Exchange **buzones**.

- **SharePoint**: esta opción buscará datos en sitios de SharePoint, sitios OneDrive para la Empresa y canales de Teams. Puede elegir buscar en todos los sitios SharePoint de su organización o seleccionar **Elegir sitios** para seleccionar usuarios individuales en el panel flotante **SharePoint sitios**.

Para obtener ayuda con la identificación de los términos de búsqueda adecuados, consulte los temas siguientes:

- **SharePoint sitios y direcciones URL**: [Administrar sitios en el centro de administración de SharePoint](/sharepoint/manage-sites-in-new-admin-center) proporciona instrucciones sobre cómo ordenar y filtrar sitios y cómo buscar un sitio SharePoint. Use esta opción para buscar direcciones URL que se escriban en el campo de búsqueda del panel flotante **SharePoint sitios**.

- **Teams chats y canales**: [Get-Team](/powershell/module/teams/get-team) muestra cómo buscar equipos en Microsoft Teams proporcionando propiedades o información específicas.

- **OneDrive sitios y direcciones URL**: [Acerca de las direcciones URL de OneDrive](/onedrive/list-onedrive-urls#about-onedrive-urls) proporciona información sobre el formato y las propiedades adecuados para la dirección URL de OneDrive de un usuario. Úselo para ayudarle a identificar OneDrive sitios en la búsqueda.

Se recomienda revisar cuidadosamente las selecciones para asegurarse de identificar al interesado correcto. Por ejemplo, si busca buzones por nombre y encuentra varias personas con nombres similares, compruebe el correcto antes de agregarlos a la solicitud.

## <a name="define-search-settings"></a>Definición de la configuración de búsqueda

Al crear una solicitud de derechos de asunto, se ejecutará una búsqueda predeterminada en función de las selecciones en la página **Ubicaciones** del asistente para la creación. Si desea realizar una búsqueda más dirigida o si desea obtener una estimación de los datos antes de recuperar los elementos de contenido, puede realizar esas selecciones en la página **Configuración** de búsqueda del Asistente para la creación de solicitudes.

### <a name="advanced-search-options"></a>Opciones de búsqueda avanzadas

- **Refinar la búsqueda**: esta opción le permite especificar propiedades adicionales para ayudar a identificar al interesado entre los datos de la organización. Después de elegir esta opción, se le pedirá que agregue más parámetros de búsqueda, que se explican a continuación en [Refinar la búsqueda](#refine-your-search).
- **Incluir contenido creado por el interesado**: esta opción buscará el contenido creado por el interesado. Algunos ejemplos son los archivos creados por el interesado o cargados en SharePoint por. La selección de esta opción puede aumentar significativamente la cantidad de datos devueltos.
- **Incluir todas las versiones de elementos**: si seleccionó SharePoint como ubicación de búsqueda, la consulta de búsqueda predeterminada devolverá solo la versión actual de SharePoint elementos. Al activar esta casilla, se devolverán las versiones actuales y todas las versiones anteriores de SharePoint elementos, lo que producirá una cantidad significativamente mayor de datos para que pueda revisarlos.

### <a name="data-estimate"></a>Estimación de datos

La **primera opción Obtener una estimación** presentará una estimación de la cantidad de datos que esperamos encontrar antes de que los datos se recuperen automáticamente. Cuando se muestra la estimación en la página de detalles de la solicitud, puede elegir ver los resultados de la búsqueda y obtener una vista previa de un muestreo de los elementos detectados. Si los elementos representan los resultados esperados, deberá seleccionar **Recuperar datos** para continuar con la recuperación real de elementos de contenido.

## <a name="refine-your-search"></a>Refinar la búsqueda

Si elige **Refinar la búsqueda** en la página **Configuración** de búsqueda, al seleccionar **Siguiente** , se le pedirá que proporcione detalles de los atributos y condiciones personales para dirigirse aún más a los resultados de la búsqueda. Puede realizar adiciones en cualquiera de las dos categorías o en ambas. Cuando haya terminado de realizar selecciones en esta sección, la recuperación de datos de la solicitud se basará en la configuración de búsqueda.

#### <a name="add-personal-attributes"></a>Agregar atributos personales

Escriba valores en los campos de texto para los nombres, los alias, las direcciones de correo electrónico y la dirección del interesado. Puede agregar otros identificadores, como la fecha de nacimiento o el número de teléfono, y los campos de texto admiten varias entradas separadas por un punto y coma. Cuando haya terminado, seleccione **Siguiente** para continuar con la página **Condiciones** .

#### <a name="conditions"></a>Condiciones

Seleccione el botón **Agregar condición** para elegir entre una serie de condiciones para dirigirse aún más a la búsqueda, incluidos el nombre del elemento, los nombres de remitente y destinatario, el tipo de datos personales y si el elemento se ha compartido externamente fuera de la organización. Los campos de texto admiten varias entradas separadas por un punto y coma. Cuando haya terminado, seleccione **Siguiente** para guardar la configuración de búsqueda y avanzar a la configuración del tipo de solicitud.

## <a name="next-steps"></a>Siguientes pasos

Una vez creada la solicitud, la verá en la página de la solicitud de derechos del sujeto. Para más información sobre cómo continuar con la revisión, consulte [Revisión de datos y colaboración en las solicitudes](subject-rights-requests-data-review.md).

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legal

[Declinación de responsabilidades legal de Microsoft Priva](priva-disclaimer.md)
