---
title: Creación de una solicitud y definición de la configuración de búsqueda en solicitudes de derechos del firmante
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
description: Obtenga información sobre cómo crear una nueva solicitud de derechos de sujeto y definir la configuración de búsqueda en Solicitudes de datos personales Microsoft Priva.
ms.openlocfilehash: bd67b68a1c0d017b8f0d667fb3e4ad21726cc976
ms.sourcegitcommit: 8cbafebb1a1b26a0bd92e500a1e6d6c60243c64b
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/20/2022
ms.locfileid: "66166659"
---
# <a name="create-a-request-and-define-search-settings"></a>Creación de una solicitud y definición de la configuración de búsqueda

**En este artículo**: Obtenga información sobre cómo crear una solicitud en Priva para empezar a cumplir una solicitud de derechos de sujeto. Comprenda la configuración de búsqueda para la recuperación de datos y cómo refinar la búsqueda.

Los usuarios que tienen un rol en el grupo de roles Administradores de solicitudes de derechos del firmante que no sean el rol de solo vista (consulte [Priva permisos](priva-permissions.md)) pueden crear una solicitud. Hay dos maneras de crear una solicitud:

- A partir de una [plantilla](#quick-setup-use-a-template-with-default-settings), una opción rápida "lista para usar" que usa la configuración predeterminada personalizada; O
- La opción [personalizada](#custom-setup-guided-process-to-choose-all-settings) , que es un proceso guiado para recorrer toda la configuración.

> [!TIP]
> La primera vez que visite la solución **Subject Rights Requests** , ofrecemos una manera simplificada de crear una solicitud y explorar características. Consulte [Introducción a la primera solicitud](#getting-started-with-your-first-request) a continuación.

## <a name="request-types"></a>Tipos de solicitud

Solicitudes de los interesados Priva admite tres tipos diferentes de solicitudes:

1. **Acceso**: proporciona un resumen de la información personal del interesado en su organización en Microsoft 365.

2. **Exportar**: proporciona un resumen y un archivo exportado de elementos de contenido que contienen la información personal del interesado. Estos son los elementos revisados y marcados como **Incluidos** durante la revisión de los datos recopilados por la configuración de búsqueda.

3. **Lista etiquetada para seguimiento**: genera un resumen de los archivos etiquetados durante la revisión de datos que pueden requerir más acción fuera de Priva. Por ejemplo, es posible que deba facilitar la eliminación de la información personal del interesado según su solicitud. Puede ver las etiquetas incluidas y configurar etiquetas personalizadas para su organización en [Priva configuración](priva-settings.md).

## <a name="getting-started-with-your-first-request"></a>Introducción a la primera solicitud

Al iniciar una evaluación o suscripción de solicitudes de derechos del sujeto, ofrecemos una configuración sencilla y rápida para la primera solicitud que usa la configuración predeterminada. Esta configuración puede ayudarle a explorar el flujo de trabajo de solicitud de derechos del sujeto y familiarizarse con su funcionalidad.

La primera vez que llegue a la página Solicitudes de derechos del sujeto, verá un banner en la parte superior con un botón **Comenzar**. Cuando un usuario selecciona este botón, aparece un panel flotante con la información de ese usuario rellenada previamente en los campos nombre y correo electrónico, y muestra toda la configuración predeterminada.

**Explorar la funcionalidad de las solicitudes con su información**: probar una solicitud de derechos de sujeto basada en su propia información puede ayudarle a familiarizarse con cada fase del proceso. Verá lo que devolverá una búsqueda predeterminada y podrá practicar la refinación de los resultados ajustando la configuración de búsqueda. En la pestaña **Datos recopilados** , puede revisar los elementos del área de vista previa a la derecha y practicar la redacción de texto, la aplicación de etiquetas, la introducción de notas y el marcado de elementos para incluir o excluir para el informe final (busque detalles en [Revisar datos para una solicitud de derechos del interesado](subject-rights-requests-data-review.md)).

- No es necesario usar la información para crear la primera solicitud. Si está listo para iniciar una solicitud para un interesado, reemplace su nombre y dirección de correo electrónico por la información del interesado.

Para aceptar toda la configuración y crear la solicitud, seleccione **Crear**. El panel se cerrará y verá la nueva solicitud en la página **Solicitudes de derechos del firmante** . Para cambiar cualquiera de los valores predeterminados antes de crear la solicitud, seleccione **Editar detalles de la solicitud**, lo que le coloca en el [asistente para la creación de solicitudes de derechos de asunto](#custom-setup-guided-process-to-choose-all-settings).

> [!NOTE]
> Cualquier solicitud que cree contará para la asignación de suscripción de prueba o de pago, independientemente de qué información del interesado se use para la solicitud. El período de retención de datos estándar de 30 días se aplica después de cerrar la solicitud. Obtenga información sobre cómo cambiar [los períodos de retención de las solicitudes de derechos de los interesados](subject-rights-requests-reports.md#retention-periods-for-reports-and-data).

## <a name="quick-setup-use-a-template-with-default-settings"></a>Configuración rápida: usar una plantilla con la configuración predeterminada

Al crear una solicitud directamente desde una plantilla, la configuración predeterminada está pensada para ayudarle a ponerse en marcha rápidamente. Las tres plantillas corresponden a los [tres tipos de solicitud](#request-types): **Acceso a datos**, **Exportación de datos** y **Datos etiquetados para realizar más acciones.**  Puede ver la configuración predeterminada de una plantilla y realizar cambios durante el proceso de creación de la solicitud.

##### <a name="selecting-the-relationship"></a>Selección de la relación

Cada plantilla le permite seleccionar el tipo de relación entre el interesado y su organización, que a su vez determina la configuración predeterminada. En los puntos siguientes se explica cómo afecta la relación que elija a la configuración de búsqueda en las plantillas:

- **Empleado actual**: los resultados de la búsqueda se adaptan para evitar correos electrónicos o chats Teams en los que el empleado ha participado, o archivos creados por el empleado. Esta configuración simplifica los resultados de la búsqueda, ya que los empleados actuales generalmente tienen acceso al contenido que crearon o a la comunicación en la que participaron.

- **Empleado anterior**: la configuración de búsqueda prioriza el buzón del empleado anterior (si está disponible) y los elementos creados por el empleado. Esta configuración tiene como objetivo devolver contenido en el que los empleados anteriores generaron o participaron.

- **Cliente**, **Empleado potencial** y **Otros**: Los resultados de búsqueda de estas relaciones no incluirán contenido creado por el interesado y solo incluirán las versiones más recientes de SharePoint elementos (obtenga más información en [opciones de búsqueda avanzadas](#advanced-search-options)).

> [!TIP]
> En la página principal **Solicitudes de derechos de sujeto** , puede ordenar la lista de solicitudes por relación en la columna **Relación con la organización** .

#### <a name="steps-for-creating-a-request-from-a-template"></a>Pasos para crear una solicitud a partir de una plantilla

1. En el [centro de cumplimiento de Microsoft Purview](https://compliance.microsoft.com/), seleccione **Solicitudes de los interesados Priva** en el panel de navegación izquierdo.

2. En la esquina superior derecha de la pantalla, seleccione **Crear una solicitud**.

3. Busque el tipo de solicitud que desea crear (**acceso a datos**, **exportación de datos** o **Datos etiquetados para realizar una acción adicional**) y seleccione **Comenzar**. Aparecerá un panel flotante.

4. En **Relación con la organización**, seleccione la opción que describe la [relación](#selecting-the-relationship) entre el interesado y su organización. Si selecciona **Otro**, aparecerá un campo **de texto Otra relación** en el panel flotante. Escriba un término que tenga sentido para su organización; por ejemplo, "paciente" o "estudiante". 

5. Si desea revisar todos los valores predeterminados y realizar cambios en cualquiera de ellos, seleccione el botón **Ver configuración** . La configuración aparecerá en el panel flotante. Para cambiar cualquier configuración, seleccione **Editar configuración**, que le llevará al [proceso guiado](#custom-setup-guided-process-to-choose-all-settings) que se describe a continuación.

6. Escriba los detalles del interesado:
    - El nombre y el apellido, y la dirección de correo electrónico, son campos obligatorios. En el caso de los empleados actuales y anteriores, al escribir el nombre del interesado en el campo **Buscar un interesado** aparecerá una lista de usuarios entre los que elegir. También puede seleccionar el vínculo situado debajo de ese campo para escribir manualmente su nombre y correo electrónico.
    - Es opcional introducir el país de residencia del interesado, el reglamento de privacidad asociado a su solicitud y un período de tiempo.
   
    > [!TIP]
    >El período de tiempo predeterminado buscará el contenido creado o modificado en los últimos 12 meses. Puede cambiar esta configuración para seleccionar todo el contenido creado en cualquier momento o establecer un período de tiempo personalizado.

7. Cuando haya terminado, seleccione **Crear**. Volverá a la página Solicitud de derechos del **sujeto** con la nueva solicitud que aparece en la parte superior de la lista de solicitudes.

De forma predeterminada, la solicitud se denomina con el nombre y el tipo de solicitud del interesado. Para editar el nombre de la solicitud, seleccione la solicitud de la lista para abrir su página de detalles y seleccione el comando **Editar** en la parte superior de la pantalla. Llegará al Asistente para la creación de solicitudes. Seleccione **Siguiente** hasta que avance a la página Nombre de la **solicitud** , donde puede editar el nombre y agregar una descripción.

Ninguna de las plantillas [se pausa automáticamente en la fase de estimación de datos](subject-rights-requests-data-retrieval.md#pause-in-data-estimate). Sin embargo, puede cambiar esta y otras [opciones de búsqueda](subject-rights-requests-create.md#defining-search-settings) seleccionando **Ver Configuración** en el panel flotante de la plantilla.

## <a name="custom-setup-guided-process-to-choose-all-settings"></a>Configuración personalizada: proceso guiado para elegir toda la configuración

La opción de solicitud personalizada es un proceso guiado para crear una directiva. Para empezar, elija una plantilla y, a continuación, recorra cada configuración para personalizar la directiva. En las instrucciones siguientes se proporcionan detalles sobre la configuración básica que se aplica a cada uno de los tres tipos de directiva. Cuando la configuración sea diferente por tipo de directiva, se vinculará a instrucciones específicas.

Siga los pasos siguientes para crear una solicitud:

1. En el [portal de cumplimiento Microsoft Purview](https://compliance.microsoft.com/), seleccione **Solicitudes de los interesados Priva** en el panel de navegación izquierdo.

2. En la esquina superior derecha de la pantalla, seleccione **Crear una solicitud**.

3. En la opción **Personalizado**, seleccione **Comenzar**. Se le llevará al Asistente para la creación de solicitudes.

4. En la página **Información del interesado** , escriba los nombres y apellidos y la dirección de correo electrónico del interesado. Seleccione **Agregar residencia** para elegir el país de residencia del interesado. Seleccione la opción que identifica cómo está relacionado el interesado con su organización. Si elige **Otro**, escriba un término para describir la relación que tiene sentido para su organización; por ejemplo, "paciente" o "estudiante". Seleccione **Siguiente** para pasar al paso siguiente.

5. En la página **Ubicaciones** , decida dónde desea buscar la información del interesado. Elija una o ambas ubicaciones moviendo el modificador de alternancia de estado junto a cada opción a la posición **Activado** :

   - **Exchange**: busque datos en buzones de Exchange y en chats de Teams individuales o grupales. Puede elegir buscar en todas las cuentas de Exchange de su organización o seleccionar **Elegir cuentas** para seleccionar usuarios individuales en el panel flotante Exchange **buzones**.

   - **SharePoint**: busque datos en sitios de SharePoint, sitios OneDrive para la Empresa y canales de Teams. Puede elegir buscar en todos los sitios SharePoint de su organización o seleccionar **Elegir sitios** para seleccionar usuarios individuales en el panel flotante **SharePoint sitios**.

    > [!TIP]
    > Para obtener ayuda con la identificación de los términos de búsqueda adecuados, consulte los temas siguientes:
    > - SharePoint sitios y direcciones URL: [Administrar sitios en el centro de administración de SharePoint](/sharepoint/manage-sites-in-new-admin-center) proporciona instrucciones sobre cómo ordenar y filtrar sitios y cómo buscar un sitio SharePoint. Use esta opción para buscar direcciones URL que se escriban en el campo de búsqueda del panel flotante **SharePoint sitios**.
    > - Teams chats y canales: [Get-Team](/powershell/module/teams/get-team) muestra cómo buscar equipos en Microsoft Teams proporcionando propiedades o información específicas.
    > - OneDrive sitios y direcciones URL: Acerca de [las direcciones URL de OneDrive](/onedrive/list-onedrive-urls#about-onedrive-urls) proporciona información sobre el formato y las propiedades adecuados para la dirección URL de OneDrive de un usuario. Úselo para ayudarle a identificar OneDrive sitios en la búsqueda.

6. En la página **Definir configuración de búsqueda** , puede optar por realizar cambios en la búsqueda predeterminada eligiendo entre varias opciones de búsqueda avanzadas. Aquí es donde también puede elegir obtener una estimación primero antes de que los datos se devuelvan automáticamente. Si elige cualquiera de estas opciones, al seleccionar **Siguiente** , se procederá a pantallas adicionales. Obtenga detalles en [Definición de la configuración de búsqueda](#defining-search-settings) a continuación. Si no desea cambiar la búsqueda, deje todas las opciones en blanco y seleccione **Siguiente** para avanzar a la siguiente fase.

7. En **la página Seleccionar el tipo de solicitud** , elija el tipo de solicitud: **Access**, **Export** o **Tagged list for follow up** ([vea las descripciones anteriores](#request-types)). Indique si la solicitud pertenece a un reglamento de privacidad de datos. Revise o realice cambios en la fecha límite de finalización, que tiene como valor predeterminado dos semanas después de la fecha de creación de la solicitud. Después, seleccione **Siguiente**.

8. En la página **Confirmar o editar el nombre de esta solicitud** , puede conservar o editar el nombre descriptivo proporcionado para la solicitud y escribir una descripción opcional. Después, seleccione **Siguiente**.

9. En la página **Revisar y finalizar** , revise el resumen de lo que ha escrito durante los pasos anteriores. Cualquier campo se puede editar seleccionando el **vínculo Editar** en cada sección. Cuando haya terminado, seleccione **Crear solicitud**.

Verá una pantalla de confirmación una vez creada la solicitud. Seleccione **Listo** para volver a la pantalla principal Solicitudes de derechos del sujeto. La nueva solicitud se mostrará en la parte superior de la lista de solicitudes. Selecciónela de la lista para empezar a revisar y trabajar en las fases de progreso.

#### <a name="what-happens-after-your-request-is-created"></a>¿Qué ocurre después de crear la solicitud?

Calcularemos una estimación de la cantidad de datos que espera encontrar en función de los parámetros de búsqueda que comienza inmediatamente. Visite la página de detalles de la solicitud en unos minutos o una hora para ver los resultados de la estimación y si la solicitud ha pasado a la fase siguiente. La solicitud pasará automáticamente de **Estimación de datos** a **Recuperación de datos** , excepto en las siguientes circunstancias:

 - Si seleccionó recibir primero un esimtae de datos en el paso 5, **Definir la configuración de búsqueda**, podrá ver los detalles de la búsqueda y realizar cambios en la búsqueda antes de recuperar todos los datos. Deberá avanzar manualmente a la siguiente fase de **recuperación de datos** si se pausa en **Estimación de datos**.
 
 - Si no ha optado por detenerse en la estimación de datos, pero predice que la búsqueda producirá un gran volumen de datos, verá una barra de mensajes en la parte superior de la solicitud con un vínculo para editar la búsqueda antes de continuar con **la recuperación de datos**.

Visite [Estimación y recuperación de datos](subject-rights-requests-data-retrieval.md) para obtener más información sobre estas fases.

## <a name="defining-search-settings"></a>Definición de la configuración de búsqueda

Al crear una solicitud de derechos de asunto, se ejecutará una búsqueda predeterminada en función de las selecciones en la página **Ubicaciones** del asistente para la creación. Si desea realizar una búsqueda más dirigida o si desea obtener una estimación de los datos antes de recuperar los elementos de contenido, puede realizar esas selecciones en la página **Configuración** de búsqueda del Asistente para la creación de solicitudes.

### <a name="advanced-search-options"></a>Opciones de búsqueda avanzadas

- **Refinar la búsqueda**: esta opción le permite especificar propiedades adicionales para ayudar a identificar al interesado entre los datos de la organización. Después de elegir esta opción, se le pedirá que agregue más parámetros de búsqueda, que se explican a continuación en [Refinación de la búsqueda](#refining-your-search).
- **Incluir contenido creado por el interesado**: esta opción buscará el contenido creado por el interesado. Algunos ejemplos son los archivos creados por el interesado o cargados en SharePoint por. La selección de esta opción puede aumentar significativamente la cantidad de datos devueltos.
- **Incluir todas las versiones de elementos**: si seleccionó SharePoint como ubicación de búsqueda, la consulta de búsqueda predeterminada devolverá solo la versión actual de SharePoint elementos. Al activar esta casilla, se devolverán las versiones actuales y todas las versiones anteriores de SharePoint elementos, lo que producirá una cantidad significativamente mayor de datos para que pueda revisarlos.

> [!TIP]
> Puede optar por cargar material adicional para permitir que Priva identifique a los interesados en función de los valores de datos exactos. Para más información, consulte [Coincidencia de datos para solicitudes de derechos del interesado](subject-rights-requests-data-match.md).

### <a name="data-estimate"></a>Estimación de datos

La **primera opción Obtener una estimación** presentará una estimación de la cantidad de datos que esperamos encontrar antes de que los datos se recuperen automáticamente. Cuando se muestra la estimación en la página de detalles de la solicitud, puede elegir ver los resultados de la búsqueda y obtener una vista previa de un muestreo de los elementos detectados. Si los elementos representan los resultados esperados, deberá seleccionar **Recuperar datos** para continuar con la recuperación real de elementos de contenido. Obtenga más detalles sobre la [fase de estimación de datos](subject-rights-requests-data-retrieval.md).

## <a name="refining-your-search"></a>Refinación de la búsqueda

Si elige **Refinar la búsqueda** en la página **Configuración** de búsqueda o si ha pausado en la fase **Estimación** de datos y decide editar la consulta de búsqueda, se le pedirá que proporcione detalles sobre los atributos y condiciones personales para dirigirse a los resultados de la búsqueda. Puede realizar adiciones en cualquiera de las dos categorías o en ambas. Cuando haya terminado de realizar selecciones en esta sección, la recuperación de datos de la solicitud se basará en la configuración de búsqueda.

Los detalles que se explican a continuación también son lo que se le pedirá que proporcione si ha pausado en la fase **Estimación de datos** y decide editar la consulta de búsqueda. 

#### <a name="add-personal-attributes"></a>Agregar atributos personales

Escriba valores en los campos de texto para los nombres, los alias, las direcciones de correo electrónico y la dirección del interesado. Puede agregar otros identificadores, como la fecha de nacimiento o el número de teléfono, y los campos de texto admiten varias entradas separadas por un punto y coma. Cuando haya terminado, seleccione **Siguiente** para continuar con la página **Condiciones** .

#### <a name="conditions"></a>Condiciones

Seleccione el botón **Agregar condición** para elegir entre una serie de condiciones para dirigirse aún más a la búsqueda, incluidos el nombre del elemento, los nombres de remitente y destinatario, el tipo de datos personales y si el elemento se ha compartido externamente fuera de la organización. Los campos de texto admiten varias entradas separadas por un punto y coma. Cuando haya terminado, seleccione **Siguiente** para guardar la configuración de búsqueda y avanzar a la configuración del tipo de solicitud.

## <a name="next-steps"></a>Pasos siguientes

Una vez creada la solicitud, la verá en la página de la solicitud de derechos del sujeto. Para más información sobre cómo continuar con la revisión, consulte [Revisión de datos y colaboración en las solicitudes](subject-rights-requests-data-review.md).

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legal

[Microsoft Priva declinación de responsabilidades legal](priva-disclaimer.md)
