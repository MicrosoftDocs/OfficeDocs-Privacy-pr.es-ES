---
title: Crear una solicitud de derechos de sujeto
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
ms.openlocfilehash: 9de1047950a556b4456fd4453ea8d860a0a01c38
ms.sourcegitcommit: 16dd1c0320bf1c58ad75edbbe2113fc79013f504
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/25/2022
ms.locfileid: "64404614"
---
# <a name="create-a-subject-rights-request"></a>Crear una solicitud de derechos de sujeto

Los administradores de administración de derechos de sujeto pueden abrir nuevas solicitudes a través de la página principal solicitudes de derechos de sujeto de Priva. Un asistente le guiará a través del proceso de búsqueda de datos personales sobre un interesado e inicio del proceso de cumplimiento de su solicitud.

También puede optar por cargar material adicional para permitir que Priva identifique a los interesados en función de los valores de datos proporcionados exactamente. Para obtener más información, vea [Coincidencia de datos para solicitudes de derechos del sujeto](subject-rights-requests-data-match.md).

## <a name="request-types"></a>Tipos de solicitud

Priva Subject Rights Requests admite tres tipos diferentes de solicitudes:

1. **Access**: proporciona un resumen de la información personal del interesado en poder de su organización en Microsoft 365.

2. **Exportar**: proporciona un resumen y un archivo exportado de elementos de contenido que contienen la información personal del interesado. Estos son los elementos revisados y marcados como **Incluidos** durante la revisión de los datos recopilados por la configuración de búsqueda.

3. **Lista etiquetada para seguimiento**: genera un resumen de los archivos etiquetados durante la revisión de datos que pueden requerir acciones adicionales fuera de Priva. Por ejemplo, es posible que deba facilitar la eliminación de la información personal del interesado de acuerdo con su solicitud. Puede ver las etiquetas incluidas y configurar etiquetas personalizadas para su organización en [la configuración de Priva](priva-settings.md).

## <a name="use-the-subject-rights-request-creation-wizard"></a>Usar el Asistente para creación de solicitudes de derechos de sujeto

1. En la [Centro de cumplimiento de Microsoft 365](https://compliance.microsoft.com/), seleccione **Priva Subject Rights Requests** en la navegación izquierda.

2. En la esquina superior derecha, seleccione **Crear una solicitud**.

3. En la **página Información** del interesado, agregue el nombre y apellidos del interesado, la dirección de correo electrónico, el país de residencia y especifique su relación con su empresa. Después, seleccione **Siguiente**.

4. En la **página** Ubicaciones, elija las Microsoft 365 donde desea buscar los datos personales del interesado. Obtenga detalles sobre [la configuración de la ubicación](#choose-locations). Cuando haya terminado de elegir ubicaciones, seleccione **Siguiente.**

5. En la **página Configuración de** búsqueda, puede cambiar la configuración de búsqueda para refinar la búsqueda y elegir si primero se obtiene una estimación antes de recuperar datos. No es necesario elegir ninguna opción en esta página, lo que da como resultado una búsqueda predeterminada en función de las ubicaciones especificadas en el paso anterior. Para obtener más información sobre las opciones aquí, vea [Definir la configuración de búsqueda](#define-search-settings). Cuando esté listo para continuar, seleccione **Siguiente**.

6. En la **página Tipo de** solicitud, elija [](#request-types) un tipo de solicitud en función de lo que el interesado desea que haga con sus **datos: Access**, **Export** o **Tagged list for follow up**. Si su solicitud se relaciona con un reglamento de privacidad de datos específico, también puede seleccionarlo en una lista proporcionada para agregar más contexto. Establecer una fecha límite (obligatoria) facilita la ordenación de las solicitudes que se acercan o vencidas y se resuelven en tiempo y forma. Cuando haya terminado, seleccione **Siguiente**.

7. En **el nombre de la** solicitud, confirme o edite el nombre de esta solicitud y agregue una descripción opcional para su referencia. Después, seleccione **Siguiente**.

8. En la **página Revisar y finalizar** , revise las selecciones. Cualquier sección se puede editar. Cuando haya terminado, seleccione **Crear solicitud**.

La solicitud tendrá su propia página de detalles y aparecerá en la página principal de solicitud de derechos de sujeto. Después de crear la solicitud, Priva empezará a buscar coincidencias con la información del interesado que proporcionó en las ubicaciones especificadas. Podría tardar varios minutos en mostrar una estimación de datos en la página de detalles de la solicitud en función del ámbito de la búsqueda.

## <a name="choose-locations"></a>Elegir ubicaciones

Para cada solicitud de derechos de sujeto, puede establecer la búsqueda para buscar datos en todas o ubicaciones específicas dentro de Exchange y Sharepoint. Elija una ubicación moviendo su modificador de alternancia a la **posición On** . Puede elegir buscar en todas las cuentas y sitios o designar cuentas o sitios específicos dentro de cada ubicación. Lea los detalles a continuación sobre lo que se trata en cada ubicación.

- **Exchange**: esta opción buscará datos en Exchange buzones de correo y en chats individuales o Teams grupo. Puede buscar en todas las Exchange de la organización o seleccionar Elegir cuentas para seleccionar usuarios  individuales en el panel desplegable Exchange **buzones** de correo.

- **SharePoint**: esta opción buscará datos en SharePoint sitios, OneDrive para la Empresa y Teams canales. Puede buscar en todos los SharePoint de la organización o seleccionar Elegir sitios para seleccionar usuarios  individuales en el panel desplegable SharePoint **sitios**.

Para obtener ayuda para identificar los términos de búsqueda adecuados, consulte los siguientes temas:

- **SharePoint sitios y direcciones URL**: administrar sitios en el Centro de administración de [SharePoint](/sharepoint/manage-sites-in-new-admin-center) proporciona instrucciones sobre cómo ordenar y filtrar sitios y cómo buscar un sitio SharePoint web. Úselo para buscar direcciones URL para escribir en el campo de búsqueda en el **panel SharePoint desplegable de sitios**.

- **Teams chats y canales**: [Get-Team](/powershell/module/teams/get-team) muestra cómo encontrar equipos en Microsoft Teams proporcionando propiedades o información específicas.

- **OneDrive sitios y direcciones** URL: acerca de [las direcciones URL](/onedrive/list-onedrive-urls#about-onedrive-urls) de OneDrive proporciona información sobre el formato y las propiedades adecuados para la dirección URL de OneDrive usuario. Úselo para ayudarle a identificar OneDrive sitios en la búsqueda.

Se recomienda revisar cuidadosamente las selecciones para asegurarse de identificar al interesado correcto. Por ejemplo, si busca buzones por su nombre y encuentra varias personas con nombres similares, compruebe el correcto antes de agregarlos a la solicitud.

## <a name="define-search-settings"></a>Definir la configuración de búsqueda

Al crear una solicitud de derechos de sujeto, se ejecutará una búsqueda predeterminada en función de las selecciones en la **página Ubicaciones del** asistente para creación. Si desea realizar una búsqueda más dirigida o si desea obtener una estimación de los datos antes de que se recuperen los elementos de contenido, puede realizar dichas selecciones en la página Configuración de  búsqueda del asistente para la creación de solicitudes.

### <a name="advanced-search-options"></a>Opciones de búsqueda avanzadas

- **Refinar la búsqueda**: esta opción permite especificar propiedades adicionales para ayudar a identificar al interesado entre los datos de la organización. Después de elegir esta opción, se le pedirá que agregue más parámetros de búsqueda, que se explican a continuación [en Refinar la búsqueda](#refine-your-search).
- **Incluir contenido creado por el interesado**: esta opción buscará el contenido creado por el interesado. Algunos ejemplos incluyen archivos creados por el interesado o cargados SharePoint por el interesado. Seleccionar esta opción puede aumentar significativamente la cantidad de datos devueltos.
- **Incluir todas las versiones de** elementos: si ha seleccionado SharePoint como ubicación de búsqueda, la consulta de búsqueda predeterminada devolverá solo la versión actual de SharePoint búsqueda. Si se marca esta casilla, se devolverán las versiones actuales y todas las versiones anteriores de SharePoint elementos, lo que dará lugar a una cantidad de datos significativamente mayor para su revisión.

### <a name="data-estimate"></a>Estimación de datos

La **opción Obtener una estimación primero** presentará una estimación de la cantidad de datos que esperamos encontrar antes de que los datos se recuperen automáticamente. Cuando la estimación se muestra en la página de detalles de la solicitud, puede elegir ver los resultados de la búsqueda y obtener una vista previa de un muestreo de los elementos que se detectaron. Si los elementos representan los resultados esperados, deberá seleccionar **Recuperar** datos para continuar con la recuperación real de elementos de contenido.

## <a name="refine-your-search"></a>Refinar la búsqueda

Si elige **Refinar** la búsqueda en la  página Configuración de búsqueda, cuando seleccione  Siguiente, se le pedirá que proporcione detalles sobre los atributos personales y las condiciones para orientar aún más los resultados de la búsqueda. Puede realizar adiciones en una o ambas categorías. Cuando haya terminado de realizar selecciones en esta sección, la recuperación de datos de la solicitud se basará en la configuración de búsqueda.

#### <a name="add-personal-attributes"></a>Agregar atributos personales

Escriba valores en los campos de texto para los nombres, sobrenombres, direcciones de correo electrónico y dirección del interesado. Puede agregar otros identificadores, como la fecha de nacimiento o el número de teléfono, y los campos de texto admiten varias entradas separadas por un punto y coma. Cuando haya terminado, seleccione **Siguiente para** continuar con la **página Condiciones** .

#### <a name="conditions"></a>Condiciones

Seleccione **el botón** Agregar condición para elegir entre una serie de condiciones para dirigirse más a la búsqueda, incluidos el nombre del elemento, los nombres de remitente y destinatario, el tipo de datos personales y si el elemento se compartió externamente fuera de la organización. Los campos de texto admiten varias entradas separadas por punto y coma. Cuando haya terminado, seleccione **Siguiente para** guardar la configuración de búsqueda y el progreso en la configuración del tipo de solicitud.

## <a name="next-steps"></a>Siguientes pasos

Una vez que cree la solicitud, verá que aparece en la página de solicitud de derechos del sujeto. Para obtener más información sobre cómo continuar con la revisión, vea [Revisar datos y colaborar en solicitudes](subject-rights-requests-data-review.md).

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legales

[Declinación de responsabilidades legales de Microsoft Priva](priva-disclaimer.md)
