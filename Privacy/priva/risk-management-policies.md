---
title: Directivas de administración de riesgos de privacidad
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
- M365-priva-privacy-risk-management
search.appverid:
- MOE150
- MET150
description: Obtenga información sobre cómo crear y administrar directivas en Gestión de riesgos de privacidad Microsoft Priva para controlar los datos personales de su organización en Microsoft 365.
ms.openlocfilehash: ff8ee92f192d2dc45998a97638e1bd0bada1fef3
ms.sourcegitcommit: 3c83e8133a5a71f4e1d76a0b2981ab3ec9cd6602
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/13/2022
ms.locfileid: "66046614"
---
# <a name="privacy-risk-management-policies"></a>Directivas de administración de riesgos de privacidad

Las directivas de administración de riesgos de privacidad pueden ayudarle a abordar los escenarios de riesgo que son importantes para su organización. Nuestras plantillas de directivas se centran en fomentar prácticas de control de datos sólidas.  Las alertas permiten a los administradores saber cuándo se detectan coincidencias de directivas y es posible que necesiten más investigación. Las notificaciones y sugerencias por correo electrónico en Microsoft Teams ayudan a los usuarios a comprender qué actividades conllevan riesgos de privacidad, permite a los usuarios corregir inmediatamente los problemas y los señala a la formación de privacidad.

Para un inicio rápido, use una plantilla con la configuración predeterminada para crear nuevas directivas para la sobreexposición de datos, las transferencias de datos y la minimización de datos y escenarios. También puede personalizar la configuración de plantilla para crear directivas que se adapten a las necesidades de su organización.

## <a name="policy-template-types"></a>Tipos de plantilla de directiva

Privacy Risk Management tiene tres plantillas de directiva diseñadas para ayudarle a abordar las principales áreas de preocupación relacionadas con la protección de datos personales. Cada plantilla tiene una configuración predeterminada que puede aceptar en el proceso de configuración rápida o personalizar mediante un proceso guiado. Al crear una nueva directiva, la primera tarea será elegir una de las tres plantillas que se enumeran a continuación:

- **Sobreexposición de datos**: esta directiva identifica los elementos de contenido que contienen datos personales que pueden ser demasiado accesibles para otras personas. Cuando se encuentran coincidencias, puede configurar notificaciones que pidan a los propietarios de contenido que apliquen rápidamente la protección.

- **Transferencias de datos**: esta directiva puede detectar transferencias de datos personales a través de los límites que determine, lo que podría implicar transferencias fuera de la organización o transferencias internas entre departamentos o regiones geográficas. Cuando se encuentran coincidencias, puede configurar notificaciones que animen a los remitentes a revocar el acceso al contenido.

- **Minimización de datos**: esta directiva identifica los elementos de contenido que contienen datos personales que han estado intactos durante largos períodos de tiempo. Cuando se encuentran coincidencias, puede enviar notificaciones a los propietarios de contenido para pedirles que realicen acciones rápidas para mantener o eliminar el elemento.

## <a name="quick-setup-using-a-template-with-default-settings"></a>Configuración rápida: uso de una plantilla con la configuración predeterminada

Al crear una directiva directamente desde una plantilla, se elegirá la mayoría de la configuración automáticamente para ayudarle a ponerse en marcha rápidamente. Siga estos pasos para crear una directiva con la configuración predeterminada mediante una de nuestras plantillas:

1. En el [Centro de cumplimiento de Microsoft Purview](https://compliance.microsoft.com/), busque Administración de riesgo de privacidad Priva en el panel de navegación izquierdo y seleccione **Directivas**.

2. Seleccione **Crear una directiva** en la esquina superior derecha de la pantalla, que muestra un panel flotante que enumera todas las opciones de creación de directivas.

3. Busque el tipo de directiva que desea crear y, en su tarjeta, seleccione **Crear**.

4. Un panel flotante contiene detalles de directiva. Al seleccionar **Ver configuración** , se mostrarán los valores predeterminados. Puede editar la configuración desde aquí, lo que le lleva al proceso guiado que se describe a continuación. Para seguir creando la directiva con la configuración predeterminada, simplemente escriba un nombre descriptivo y, a continuación, seleccione **Crear directiva**.

La directiva se creará y la encontrará en la página **Directivas** .

La directiva comenzará a ejecutarse en modo de prueba, lo que significa que no se generarán alertas ni notificaciones y podrá supervisar su rendimiento. Cuando esté listo para activar la directiva, seleccione la directiva y edítela para activarla.

## <a name="custom-setup-guided-process-to-choose-all-settings"></a>Configuración personalizada: proceso guiado para elegir toda la configuración

La opción de directiva personalizada es un proceso guiado para crear una directiva. Para empezar, elija una plantilla y, a continuación, recorra cada configuración para personalizar la directiva. En las instrucciones siguientes se proporcionan detalles sobre la configuración básica que se aplica a cada uno de los tres tipos de directiva. Cuando la configuración sea diferente por tipo de directiva, se vinculará a instrucciones específicas.

Siga los pasos siguientes para crear una directiva:

1. En el [portal de cumplimiento de Microsoft Purview](https://compliance.microsoft.com/), busque Administración de riesgo de privacidad Priva en el panel de navegación izquierdo. En el menú desplegable, seleccione **Directivas**.

2. Seleccione **Crear directiva**.

3. Elija la opción **Personalizada** para crear la directiva mediante el asistente para la creación de directivas en Administración de riesgos de privacidad.

4. Elija el tipo de directiva: **Sobreexposición de datos,** **Transferencias de datos** o **Minimización de datos**.

5. Asigne a la directiva un nombre descriptivo que le ayude a identificarla en la lista de directivas. Proporcione una descripción opcional y, a continuación, seleccione **Siguiente**.

6. Los pasos siguientes le permiten definir toda la configuración de directiva. Puede ir directamente a las descripciones de en este artículo para obtener más detalles. Entre las opciones se incluyen:
    - [**Datos que se van a supervisar**](#choose-data-to-monitor): seleccione el tipo de datos personales que supervisará la directiva.
    - [**Usuarios y grupos**](#choose-users-and-groups): aplique la directiva a todos los usuarios o usuarios seleccionados.
    - [**Ubicaciones**](#choose-locations): aplique la directiva a las áreas seleccionadas en Microsoft 365.
    - [**Condiciones**](#set-conditions): establezca las condiciones de la directiva. Estas opciones varían en función del tipo de directiva.
    - [**Resultados**](#define-outcomes-user-email-notifications-and-tips): defina los resultados cuando se encuentre una coincidencia de directiva, como las notificaciones por correo electrónico del usuario.
    - [**Alertas**](#set-alerts): decida la frecuencia de las alertas para los administradores cuando se encuentre una coincidencia de directiva.
    - [**Modo**](#testing-a-policy): elija si primero debe ejecutar la directiva en modo de prueba.
7. Cuando se completen todas las opciones, revise las opciones, realice las modificaciones deseadas y, a continuación, seleccione **Enviar** para crear la directiva.

Después de unos segundos, verá una confirmación de que se creó la directiva. Seleccione **Listo** en la página de confirmación, que le llevará a la página **Directivas** , donde verá la nueva directiva en la parte superior de la tabla.

En las secciones inmediatamente siguientes se proporcionan más detalles sobre cada configuración de directiva.

## <a name="choose-data-to-monitor"></a>Elección de los datos que se van a supervisar

Al crear o editar una directiva, le pediremos que seleccione qué tipos de datos debe supervisar la directiva. Hay dos opciones:

- **Grupos de clasificación**: una lista en la que se pueden realizar búsquedas de agrupaciones de tipos de información confidencial; por ejemplo, un grupo basado en la Ley de registros de salud de Australia o un grupo basado en información de identificación personal de EE. UU., como un número de pasaporte estadounidense.

- **Tipos de información confidencial individuales**: una lista de tipos de información confidencial que se pueden buscar; por ejemplo, números del Seguro Social o números de licencia de conducir.

Si selecciona entre los grupos de clasificación existentes, tampoco puede seleccionar tipos individuales ni crear sus propios grupos. Para obtener la mayor flexibilidad, elija tipos de información confidencial individuales. Para usar los estándares más comunes, elija entre los grupos de clasificación. Más información sobre cada tipo de datos a continuación.

### <a name="classification-groups"></a>Grupos de clasificación

Los grupos de clasificación son agrupaciones de [tipos de información confidencial](/microsoft-365/compliance/sensitive-information-type-entity-definitions) que se usan para detectar contenido relacionado con datos personales o regulaciones específicas.

Al seleccionar esta opción en la página **Datos para supervisar** , deberá seleccionar **+Agregar grupos de clasificación** y elegir uno o varios grupos de la lista que aparece en un panel flotante.

### <a name="individual-sensitive-information-types"></a>Tipos de información confidencial individuales

Al elegir tipos de [información confidencial](/microsoft-365/compliance/sensitive-information-type-entity-definitions) específicos, como los números del Seguro Social o la información de licencia de conducir, puede personalizar su propio grupo o grupos de datos para buscarlos. Puede seleccionar en la lista completa de tipos de información confidencial en Privacy Risk Management. Cada tipo de información tiene sus propias propiedades.

Al seleccionar esta opción en la página **Datos para supervisar** , aparece un selector con **El valor predeterminado** aparece como un nombre para el grupo de tipos de información confidencial que seleccionará. Mantenga o edite este nombre de grupo y, a continuación, seleccione **Agregar** para seleccionar uno o más tipos de información confidencial en la lista completa de Administración de riesgos de privacidad. Cada tipo de información tiene sus propias propiedades y configuraciones recomendadas, que puede detectar seleccionando el icono de información situado a la derecha del menú desplegable confianza después de agregar el tipo de información. También puede cambiar el recuento de instancias para cada tipo de información confidencial. Esta configuración designa el número de instancias únicas de cada tipo de información confidencial que quiere que detecte la directiva.

Si crea más de un grupo, el asistente le permite seleccionar cómo deben relacionarse los grupos (una relación "y" o "o") y definir su orden de operaciones.

## <a name="choose-users-and-groups"></a>Elección de usuarios y grupos

Tiene dos opciones para decidir qué usuarios cubrirá una directiva: todos los usuarios y grupos, o usuarios y grupos específicos.

- **Todos los usuarios y grupos**: esta opción aplicará la directiva a todos los usuarios y grupos de Office 365 de la organización.

- **Usuarios o grupos específicos**: esta opción le permite seleccionar usuarios individuales, grupos de Office 365 individuales o una combinación de ambos.
  - **Para elegir usuarios**: seleccione **Elegir usuarios** y, en el panel flotante, escriba una dirección de correo electrónico en el cuadro de búsqueda para buscar un usuario. O busque el usuario de la lista y seleccione la casilla situada a la izquierda de su nombre. Puede seleccionar hasta 100 usuarios. Cuando haya terminado, seleccione **Agregar.**
  - **Para elegir grupos**: seleccione **Elegir grupos** y, en el panel flotante, active la casilla situada a la izquierda de cada nombre de grupo. Puede seleccionar hasta diez grupos. Cuando haya terminado, seleccione **Agregar**.

Después de designar usuarios y grupos, seleccione **Siguiente** para avanzar al paso siguiente.

## <a name="choose-locations"></a>Elegir ubicaciones

En este paso, designará dónde en el entorno de Microsoft 365 desea que la directiva busque coincidencias de datos personales. Las opciones de ubicación dependerán del tipo de directiva y puede seleccionar más de una. Cada una de las ubicaciones se explica a continuación.

- **Exchange**: La directiva identificará las coincidencias en las cuentas de Exchange de los usuarios, que incluyen contenido en el cuerpo de los correos electrónicos y en los datos adjuntos enviados o recibidos por Exchange buzones.

- **OneDrive**: la directiva identificará las coincidencias en los archivos almacenados en la cuenta de OneDrive para la Empresa de los usuarios.

- **Teams**: La directiva identificará las coincidencias en los mensajes de los usuarios en Teams canales y chats.

- **SharePoint**: la directiva identificará las coincidencias en los archivos almacenados en los sitios de SharePoint de los usuarios. Al seleccionar esta opción, elegirá entre las siguientes opciones:
    - **Todos los sitios SharePoint**: esta selección cubrirá todos los sitios de todos los usuarios de la organización.

    - **Sitios SharePoint específicos**: esta selección le pide que designe sitios específicos a los que se va a aplicar la directiva. Puede escribir la dirección URL de un sitio específico directamente en el cuadro URL y, a continuación, seleccionar el **+** signo para agregarlo a la lista de sitios. También puede seleccionar **Elegir sitios** y, en el panel flotante, busque y seleccione en la lista de sitios a los que tiene acceso. Active la casilla que aparece al mantener el puntero sobre el sitio que desea seleccionar. Después de realizar las selecciones, seleccione **Agregar**.  Todos los sitios elegidos se mostrarán en la parte inferior de la página **Ubicaciones** .
    
    > [!TIP]
    > Si necesita ayuda para identificar los sitios de SharePoint de su organización, visite [Administrar sitios en el centro de administración de SharePoint](/sharepoint/manage-sites-in-new-admin-center).

Una vez que haya terminado de designar ubicaciones, seleccione **Siguiente**.

## <a name="set-conditions"></a>Establecer condiciones

Las condiciones para detectar coincidencias de directivas varían en función de la plantilla de directiva.

- **Sobreexposición de datos**: consulte el paso de condiciones de las [instrucciones de configuración personalizadas de la directiva de exposición de datos](risk-management-policy-data-overexposure.md#custom-setup-guided-policy-creation-process).
- **Transferencias de datos**: consulte el paso de condiciones de las [instrucciones de configuración personalizada de la directiva de transferencia de datos](risk-management-policy-data-transfer.md#custom-setup-guided-policy-creation-process).
- **Minimización de datos**: consulte el paso de condiciones de las [instrucciones de configuración personalizada de la directiva de minimización de datos](risk-management-policy-data-minimization.md#custom-setup-guided-policy-creation-process).

## <a name="define-outcomes-user-email-notifications-and-tips"></a>Definición de resultados: sugerencias y notificaciones por correo electrónico del usuario

La configuración de resultados se controla en la página **Resultados** del Asistente para la creación de directivas. En esta página, puede elegir enviar una notificación por correo electrónico a los usuarios cuando realicen una acción que coincida con las condiciones de una directiva.

Las directivas de transferencia de datos tienen una opción adicional para mostrar sugerencias a los usuarios en Teams cuando sus acciones generan una coincidencia de directiva. Estas sugerencias incluirán vínculos al entrenamiento de privacidad que proporcione e incluirán mecanismos para corregir posibles riesgos.

Estas notificaciones pueden ser oportunidades útiles para evitar que los problemas se escalen y para crear las aptitudes y la confianza de los usuarios en la adopción de prácticas seguras de control de datos.

Visite [Notificaciones de usuario en Administración de riesgos de privacidad](risk-management-notifications.md) para obtener más información sobre cómo trabajar con las notificaciones de usuario.

## <a name="set-alerts"></a>Establecimiento de alertas

Las alertas ayudan a los administradores a saber cuándo un evento de usuario coincide con las condiciones de una directiva. La configuración de alertas es opcional y controla la frecuencia con la que se generan las alertas, el umbral que se debe alcanzar antes de que se genere una alerta y la gravedad de la alerta. Las alertas se muestran en la tarjeta **Alertas** de la página **Directivas** . Obtenga más información sobre [cómo ver, investigar y corregir alertas](risk-management-alerts.md).

#### <a name="turn-on-alerts"></a>Activar alertas

Puede activar las alertas cuando cree una directiva por primera vez o editarla más adelante para activarlas. En la página **Alertas** del Asistente para la creación de directivas, establezca el modificador de alternancia **Crear alertas** en la posición **Activado** .

#### <a name="alert-frequency-and-thresholds"></a>Frecuencia y umbrales de alertas
Después de activar las alertas, decida con qué frecuencia se generarán.

- **Alerta cada vez que se produce una coincidencia de directiva**: la selección de esta opción podría producir un gran número de alertas.
- **Alerta cuando se alcanza un umbral específico**: establecerá umbrales en función del número y la frecuencia de los eventos de usuario detectados.

#### <a name="alert-severity-level"></a>Nivel de gravedad de alerta
Seleccione un nivel de gravedad bajo, medio o alto. Sugerimos que su organización defina lo que cada nivel representa para usted.

## <a name="testing-a-policy"></a>Prueba de una directiva

Al crear una directiva, la configuración predeterminada es iniciarla en modo de prueba. Esto significa que una vez creada la directiva:

- No se generará ninguna alerta. Sin embargo, verá información en la página de detalles de la directiva cuando se detecten coincidencias, incluidos los tipos de datos detectados y sus ubicaciones.

- No se enviará ninguna notificación por correo electrónico de usuario cuando se detecten coincidencias de directiva. Sin embargo, verá información en la página de detalles de la directiva que muestra qué usuarios están asociados a las coincidencias de directiva.

El modo de prueba le permite buscar coincidencias de los últimos 30 días de actividad del usuario. Con estas conclusiones, puede medir el comportamiento de la directiva y revisar los tipos de alertas que se pueden generar cuando la directiva está activada.

Se recomienda probar la directiva durante al menos cinco días para ayudarle a comprender el tipo y el volumen de coincidencias que generará. Puede [editar la directiva](#edit-a-policy) mientras está en modo de prueba para poder supervisar cómo afectan los cambios a su rendimiento antes de activarla. Por ejemplo, puede encontrar que la directiva es demasiado amplia y que sus condiciones necesitan ajustarse. O bien, puede darse cuenta de que, en función de la actividad, detecta que las alertas no se generarán en un período de tiempo que le resulte útil.

La página de detalles de la directiva indica cuántos días se ha estado ejecutando la prueba. Verá cuántas coincidencias se han encontrado por ubicación, cuántos eventos de usuario que coinciden con las condiciones de la directiva y los tipos de datos personales detectados por las coincidencias de directiva.

> [!NOTE]
> Si cambia el modificador **Ejecutar en modo de prueba** a la posición **Desactivado** , *se activará la directiva* cuando haya terminado de crearla. Esto significa que las alertas o las notificaciones de usuario que configure comenzarán a generarse cuando se detecten coincidencias.

Cuando esté satisfecho con la configuración de la directiva y esté listo para activarla, seleccione el botón azul **Activar directiva** . La directiva ahora estará activa y generará las alertas y notificaciones de usuario que haya configurado.

## <a name="turn-on-a-policy"></a>Activar una directiva

Puede establecer una directiva para activarla en cuanto termine de crearla. Esto no se recomienda, ya que es mejor supervisar el rendimiento y la configuración colocando la directiva en modo de prueba antes de activarla (consulte [Prueba de una directiva](#testing-a-policy)).

Si ha creado la directiva en modo de prueba, puede activarla rápidamente siguiendo estos pasos:

1. En **la página Directivas** , busque la directiva y seleccione su nombre para abrir su página de detalles.
2. En la tarjeta **Estado de** la directiva, seleccione **Activar directiva**.

La directiva ahora estará activa y generará las alertas y notificaciones de usuario que haya configurado.

## <a name="turn-off-a-policy"></a>Desactivar una directiva

Para desactivar una directiva en cualquier momento, seleccione **Desactivar directiva** en la esquina superior derecha de la página de detalles de una directiva. Cuando una directiva está desactivada, no detectará coincidencias ni generará alertas ni notificaciones por correo electrónico. Al desactivar una directiva no se eliminará una directiva. Para volver a activar una directiva, seleccione **Activar directiva** en la esquina superior derecha de la página de detalles de la directiva.

## <a name="view-details-and-activity-from-the-policy-details-page"></a>Ver los detalles y la actividad de la página de detalles de la directiva

Cada directiva tiene una página de detalles que muestra las actividades detectadas por la directiva y la información para ayudarle a abordar los riesgos.

Una vez creada la directiva, seleccione su nombre en la tabla de la página principal **Directivas** . En la pestaña **Información general** de la página de detalles de la directiva se indica el estado de la directiva, se proporciona información sobre los datos y se resaltan las coincidencias de directiva. Aquí puede ver detalles sobre coincidencias de directivas específicas y obtener más información sobre los pasos siguientes. Si la directiva se ejecuta en modo de prueba, verá los pasos siguientes recomendados en esta página y un botón para activar la directiva.

Cuando la directiva esté activada, puede seguir revisando su página de detalles de la directiva para ver información continua sobre las áreas problemáticas, la gravedad y las tendencias de las alertas y las acciones correctivas realizadas.

### <a name="overview-tab"></a>Pestaña Información general

En la pestaña **Información general** de la página de detalles de la directiva, encontrará detalles sobre lo que detecta la directiva con respecto a los tipos y las ubicaciones de los datos y la actividad del usuario. A continuación se describen las conclusiones de la página de detalles de la directiva. Después de activar una directiva, los datos pueden tardar hasta 48 horas en pasar.

#### <a name="policy-status"></a>Estado de la directiva

La tarjeta de estado de la directiva indicará si la directiva está en uno de los tres estados: **Testing**, **On** o **Off**.

**Pruebas**: en esta sección se muestra el número de días que la directiva ha estado en modo de prueba, lo que significa que busca coincidencias de directiva en función de las condiciones establecidas, pero no genera alertas ni notificaciones de usuario. Proporcionaremos una recomendación cuando sea un buen momento para activar la directiva. Puede activarla en cualquier momento seleccionando el botón **Activar directiva** de esta tarjeta.

**Activado**: cuando la directiva está activada, la tarjeta de estado muestra métricas que resaltan cuándo se ha producido una acción correctiva después de que una directiva coincida genera alertas y notificaciones de usuario.

- **Acciones de usuario realizadas**: esta métrica muestra el número de acciones de corrección realizadas por los usuarios cuando se le solicita desde un correo electrónico de notificación del número total de notificaciones enviadas. Por ejemplo, el 10/8 representaría que de cada 10 notificaciones de usuario enviadas, los usuarios realizaron una acción de corrección en 8 instancias.

- **Tasa de resolución** de usuarios: esta métrica es la velocidad a la que los usuarios realizan las acciones de corrección en función del número de notificaciones generadas. Si el porcentaje es bajo, es posible que desee [editar el contenido del correo electrónico](risk-management-notifications.md#preview-and-customize-email-content) o examinar detenidamente las coincidencias para determinar si la directiva está detectando la actividad prevista.

- **Acciones de administración realizadas**: esta métrica muestra el número de acciones de corrección realizadas por los administradores cuando la directiva genera una alerta. Obtenga más información sobre [cómo realizar acciones en las alertas](risk-management-alerts.md#manage-alerts).

- **Tasa de resolución** de administradores: esta métrica es la velocidad a la que los administradores realizan las acciones de corrección en función del número de alertas.

#### <a name="matches-by-location"></a>Coincide por ubicación

La tarjeta **Coincidencias por ubicación** muestra el número de elementos de contenido detectados por la directiva según Microsoft 365 ubicación.

#### <a name="user-notifications"></a>Notificaciones de usuario 

La tarjeta Notificaciones de usuario muestra un gráfico de barras que muestra el número de correos electrónicos de notificación de usuario **generados** por la directiva si tiene esas funcionalidades activadas.

#### <a name="matches-by-user"></a>Coincidencias por usuario

La tarjeta **Coincidencias por usuario** muestra los usuarios principales cuyas acciones han desencadenado una coincidencia de directiva. Verá el número de eventos detectados por la directiva para cada usuario, junto con el número de acciones de corrección realizadas desde las notificaciones por correo electrónico. Seleccione **Ver todos los usuarios** de esta tarjeta para revisar la lista completa de usuarios detectados por la directiva.

#### <a name="matches-by-data-type"></a>Coincidencias por tipo de datos

La tarjeta **Coincidencias por tipo de datos** muestra los tipos de datos personales detectados por las coincidencias de directiva y la cantidad de cada tipo. El gráfico circular ayuda a demostrar visualmente si un determinado tipo de datos personales, por ejemplo, números del Seguro Social o números de tarjeta de crédito, se representa predominantemente en los escenarios de riesgo que intenta identificar.

> [!TIP]
> Al examinar holísticamente las ubicaciones, los tipos de datos y el número de usuarios implicados en las coincidencias de directivas, es posible que tenga un mejor sentido en cuanto a los tipos de medidas de entrenamiento y protección de datos necesarias para ayudar a su organización a proteger los datos personales que almacena.

### <a name="matched-items-tab"></a>Pestaña Elementos coincidentes

La pestaña **Elementos coincidentes** muestra una lista de todos los elementos de contenido que coinciden con una condición establecida en la directiva. Desde esta vista, puede seleccionar un elemento de su fila para obtener una vista previa de él en la ventana situada a la derecha de la lista de elementos.

En la ventana de vista previa, encontrará las pestañas siguientes que proporcionan detalles sobre cada elemento:
- **Origen**: muestra los datos personales que desencadenaron la coincidencia.
- **Detalles**: muestra el propietario del contenido (usuario de su organización) para el elemento, la ubicación Microsoft 365 del elemento, el número de tipos de datos personales dentro del elemento y los tipos de datos personales específicos.
- **Actividades de archivo**: muestra cualquier etiqueta o clasificación aplicada al elemento.
- **Historial de corrección**: muestra información sobre las acciones de corrección realizadas por usuarios o administradores en el elemento.

## <a name="edit-a-policy"></a>Editar una directiva

Puede editar la configuración de una directiva en cualquier momento, ya sea en modo de prueba o activado. Puede actualizar la mayoría de la configuración de directiva, incluido volver a poner una directiva en modo de prueba después de activarla. La única configuración que no se puede editar es la plantilla de directiva y el nombre de la directiva.

Para editar una directiva, siga estos pasos:

1. En el [portal de cumplimiento de Microsoft Purview](https://compliance.microsoft.com/), busque Administración de riesgo de privacidad Priva en el panel de navegación izquierdo. En el menú desplegable, seleccione **Directivas**.

2. Seleccione la directiva que desea editar desde su fila en la página **Directivas** , que muestra la página de detalles de esa directiva.

3. En la página de detalles de la directiva, seleccione el comando **Editar** en la esquina superior derecha de la página. Esta acción le llevará a la creación de directivas en Privacy Risk Management.

4. Siga los pasos para acceder a la configuración que desea cambiar. Puede editar toda la configuración excepto la plantilla de directiva y el nombre de la directiva. Seleccione **Siguiente** para avanzar a cada paso siguiente.

5. En la página **Finalizar** , revise la configuración y, a continuación, seleccione **Enviar** para guardar los cambios realizados.

## <a name="delete-a-policy"></a>Eliminar una directiva

Si necesita quitar una directiva de Administración de riesgos de privacidad existente, búsquíela en la lista de la página **Directivas** , seleccione el menú acción (puntos suspensivos verticales) y elija la acción **Eliminar directiva** . También puede abrir la página de detalles de la directiva y seleccionar **Eliminar** en la esquina superior derecha.

Se le pedirá que confirme su elección antes de que la eliminación sea definitiva y la directiva se quite de forma permanente. La eliminación de una directiva no afectará a los archivos previamente evaluados por la directiva, y los problemas y alertas generados por la directiva seguirán aparecen en las páginas **Alertas** y **problemas** .

## <a name="next-steps"></a>Pasos siguientes

Una vez que la directiva está activada y comienza a generar alertas, querrá empezar a comprender los riesgos que pueden presentar a su organización. Obtenga información sobre cómo administrar alertas, investigar eventos y realizar acciones de corrección en Privacy Risk Management visitando [Investigar y corregir alertas](risk-management-alerts.md).

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legal

[Microsoft Priva declinación de responsabilidades legal](priva-disclaimer.md)
