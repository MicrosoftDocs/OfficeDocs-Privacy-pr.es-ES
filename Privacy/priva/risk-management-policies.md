---
title: Crear directivas en Administración de riesgos de privacidad
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
description: Obtenga información sobre cómo crear y personalizar directivas de privacidad para controlar los datos personales de su organización en Microsoft 365.
ms.openlocfilehash: ce8f2d5e6728bcd01a99775450668c002c9cb59e
ms.sourcegitcommit: f145dff5e387a8e26db2f3a2c7de125978fbacc9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/28/2022
ms.locfileid: "62249185"
---
# <a name="create-policies-in-privacy-risk-management"></a>Crear directivas en Administración de riesgos de privacidad

Puede crear nuevas directivas en Privacy Risk Management para abordar escenarios de riesgo importantes para su organización. Para un inicio rápido, use las plantillas predeterminadas para crear nuevas directivas para la sobreexposición de datos, las transferencias de datos y la minimización de datos y escenarios. También puede personalizar sus propias directivas, usando cualquiera de estas plantillas como punto de partida.

Durante la creación o edición de directivas, puede configurar notificaciones de correo electrónico o, cuando esté disponible, sugerencias de directiva para Teams para llamar la atención de los usuarios para su corrección.

## <a name="create-a-policy-from-a-template"></a>Crear una directiva a partir de una plantilla

Siga estos pasos para crear una directiva con cualquiera de las plantillas predeterminadas.

1. En el [Centro de cumplimiento de Microsoft 365](https://compliance.microsoft.com/), vaya a la sección Administración de riesgos de privacidad de Priva y seleccione **Directivas**.
1. Seleccione **Crear directiva**.
1. Elija el tipo de plantilla que desee. Se abrirá un panel desplegable con información sobre la plantilla.
1. Para revisar la configuración predeterminada de la plantilla, incluidos los tipos de datos, las ubicaciones de datos y las condiciones que desencadenan coincidencias de directiva, seleccione **Ver configuración**.
     - Tienes la opción aquí para seleccionar **Editar configuración** para realizar cambios. Esto le dirigirá al asistente para personalizar la configuración.
1. Si está listo para usar la configuración predeterminada, asigne a la directiva un nombre descriptivo y seleccione **Crear directiva.**

Al crear una directiva directamente desde una plantilla, se elegirán automáticamente muchas opciones de configuración. También se iniciará en modo de prueba de forma predeterminada, lo que significa que no se generarán alertas ni notificaciones. Si está listo para activar completamente la directiva después de ejecutarla en modo de prueba y revisar los resultados de la directiva, puede encontrarlo en la lista de directivas y editar la directiva para activarla.

## <a name="create-a-custom-policy"></a>Crear una directiva personalizada

Para controlar pormenorización la configuración de una directiva, puede crear una directiva personalizada con una de las plantillas existentes como línea base. Priva proporciona un asistente para guiarlo a través de estos pasos.

Todos los tipos de directiva siguen este flujo básico. Determinadas opciones y configuraciones cambiarán en función de la directiva elegida.

1. En el [Centro de cumplimiento de Microsoft 365](https://compliance.microsoft.com/), vaya a la sección Administración de riesgos de privacidad de Priva y seleccione **Directivas**.
1. Seleccione **Crear directiva**.
1. Elija la **opción** Personalizado para empezar a usar el asistente.
1. Elija el tipo de plantilla de línea base: **Sobreexposición de datos,** **Transferencias de datos** o **Minimización de datos**. Cada una de ellas le dará determinadas opciones durante la creación de directivas.
1. Asigne un nombre y describa la directiva. Se recomienda usar nombres claros y descriptivos para identificar las directivas, ya que estos nombres aparecerán más adelante en alertas sobre coincidencias de directivas.
1. Continúe con el asistente y elija la configuración que desee. Entre las opciones se incluyen:
    - **Datos que se van a supervisar**: seleccione el tipo de datos personales que supervisará la directiva.
    - **Usuarios y grupos**: aplique la directiva a todos los usuarios o usuarios seleccionados.
    - **Ubicaciones**: aplique la directiva a áreas seleccionadas de Microsoft 365.
    - **Condiciones**: establezca las condiciones de la directiva. Estas opciones varían según el tipo de directiva.
    - **Resultados**: defina los resultados cuando se encuentra una coincidencia de directiva, como las notificaciones de usuario.
    - **Alertas**: decida la frecuencia de las alertas a los administradores cuando se encuentra una coincidencia de directiva.
    - **Modo**: elija si desea ejecutar primero la directiva en modo de prueba.
1. Cuando se completen todas las opciones, revise las opciones, realice las modificaciones que desee y, a continuación, **seleccione Enviar** para crear la directiva.

## <a name="learn-about-key-settings-for-all-policies"></a>Obtenga información sobre la configuración clave de todas las directivas

### <a name="choose-data-to-monitor"></a>Elegir datos para supervisar

Al editar o configurar cualquier tipo de directiva personalizada, se le pedirá que seleccione qué tipos de datos debe supervisar la directiva. A continuación se indican las opciones posibles:

- **Grupos de clasificación**: una lista de conjuntos de datos que se pueden buscar en función de las normativas clave de privacidad, como RGPD o HIPAA. Vea los detalles de cualquier grupo para ver qué tipos de información confidencial abarca. Seleccione uno o varios de estos conjuntos para usarlos tal como están.
- **Tipos individuales** de información confidencial: al elegir tipos específicos de información confidencial, como números de seguridad social o información de licencia de conducir, puede personalizar su propio grupo o grupos de datos para tener en cuenta. Este asistente le permite seleccionar de la lista completa de tipos de información confidencial dentro de Privacy Risk Management. Cada tipo de información tiene sus propias propiedades. Usa el botón de información junto a cualquiera de ellos para obtener detalles y notas sobre la configuración recomendada. Si crea más de un grupo, el asistente le permite aplicar operadores booleanos para relacionarlos y definir su orden de operaciones.

Si selecciona entre los grupos de clasificación existentes, tampoco puede seleccionar tipos individuales ni crear sus propios grupos. Para mayor flexibilidad, elige tipos de información confidencial individuales. Para usar los estándares más comunes, elija entre los grupos de clasificación.

### <a name="set-user-email-notifications"></a>Establecer notificaciones de correo electrónico de usuario

Con [las notificaciones por correo](risk-management-notifications.md) electrónico, puedes enviar notificaciones sobre coincidencias de directiva directamente a los propietarios de contenido. Estos correos electrónicos resumen qué datos deben revisarse y las posibles acciones que deben realizarse, como hacer que los documentos sean privados, mantenerlos en el archivo, informar de las coincidencias de falsos positivos y agregar notas para futuras referencias. Estos correos electrónicos también incluyen vínculos para formar a los destinatarios sobre cómo tratar estos casos. Es necesario proporcionar estos vínculos y debe apuntar a su propia documentación interna sobre procesos y procedimientos recomendados.

Las notificaciones se pueden habilitar para directivas individuales durante la creación de directivas personalizadas o al editar cualquier directiva. Establece tus preferencias en la **sección Resultados** .

La configuración necesaria incluye la frecuencia de las notificaciones y el vínculo al aprendizaje de privacidad.

La configuración opcional incluye determinados campos personalizables para los correos electrónicos. Seleccione la **opción Vista previa y editar correo** de notificación para abrir un panel desplegable que muestre una notificación de ejemplo. Aquí puede editar la línea de asunto del correo electrónico, el encabezado y el texto del cuerpo, así como el nombre para mostrar y la dirección URL de su aprendizaje de privacidad.

Tenga en cuenta que la capacidad general de la Administración de riesgos de privacidad para enviar notificaciones por correo electrónico se controla **en Configuración**. Está habilitada de forma predeterminada. Desactivar esta configuración detendrá todos los correos electrónicos incluso si las notificaciones se han configurado en un nivel de directiva individual.

## <a name="learn-about-settings-for-data-minimization-policies"></a>Obtenga información sobre la configuración de las directivas de minimización de datos

Las directivas de minimización de datos se centran en la antigüedad del contenido y en cuánto tiempo ha pasado desde que se modificó por última vez. La supervisión de los datos personales que aún se conservan en contenido antiguo sin usar puede ayudarle a administrar mejor los datos almacenados y reducir los riesgos. Esta configuración se controla en la **pantalla Condiciones** .

De forma predeterminada, las directivas de minimización de datos buscan contenido que contenga datos personales que se crearon o modificaron por última vez hace al menos 60 días. Al editar o crear una directiva personalizada, puede seleccionar entre otros marcos de tiempo preestablecidos.

## <a name="learn-about-settings-for-data-transfer-policies"></a>Más información sobre la configuración de las directivas de transferencia de datos

Las directivas de transferencia de datos permiten supervisar la transferencia de datos entre determinadas regiones del mundo o entre distintos departamentos de la organización. En la **pantalla Condiciones** , puedes elegir qué tipos de transferencias debe buscar la Administración de riesgos de privacidad.

De forma predeterminada, las directivas de transferencia de datos buscan transferencias entre Norteamérica y otras regiones. Al editar o crear una directiva personalizada, puede elegir el tipo de transferencia y, a continuación, realizar selecciones para las regiones o departamentos de remitente y destinatario.

Las directivas de transferencia de datos también admiten proporcionar sugerencias y recomendaciones de directiva a los usuarios en Teams, para que puedan mantenerse informados sobre los procedimientos recomendados para el tratamiento de datos. Se puede alternar en la **pantalla Resultados** .

## <a name="learn-about-settings-for-data-overexposure-policies"></a>Información sobre la configuración de las directivas de sobreexposición de datos

Su organización puede almacenar contenido en varios niveles de acceso, incluidas las áreas de acceso público y otras que están restringidas. En la **pantalla** Condiciones, puede optar por que la Administración de riesgos de privacidad busque posibles sobreexposición de datos para el contenido almacenado en cualquiera de los siguientes niveles de acceso:

- **Público**: cualquier persona con un vínculo puede ver este contenido.
- **Externo**: las personas específicas fuera de la organización tienen acceso.
- **Interno**: los usuarios de la organización tienen acceso.

De forma predeterminada, las directivas de sobreexposición de datos evalúan los tres niveles de acceso. Al editar o crear una directiva personalizada, puede elegir todos o cualquiera de estos niveles.

## <a name="next-steps"></a>Pasos siguientes

Para obtener más información acerca de cómo administrar las directivas y realizar cambios después de crearlas, consulte [Administrar directivas](risk-management-policies-manage.md).

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legales

[Declinación de responsabilidades legales de Microsoft Priva](priva-disclaimer.md)
