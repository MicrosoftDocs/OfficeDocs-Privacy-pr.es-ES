---
title: Creación de directivas en Privacy Risk Management
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
ms.openlocfilehash: 2b655d778e73e2107c289988966fb491bf3ebb2e
ms.sourcegitcommit: 09ecdaded9a9f8f79587f2acb978dc53b83e5c01
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/19/2022
ms.locfileid: "64930511"
---
# <a name="create-policies-in-privacy-risk-management"></a>Creación de directivas en Privacy Risk Management

Puede crear nuevas directivas en Privacy Risk Management para abordar escenarios de riesgo importantes para su organización. Para un inicio rápido, use las plantillas predeterminadas para crear nuevas directivas para la sobreexposición de datos, las transferencias de datos y la minimización de datos y escenarios. También puede personalizar sus propias directivas, usando cualquiera de esas plantillas como punto de partida.

Al crear o editar directivas, puede configurar notificaciones por correo electrónico o, cuando esté disponible, sugerencias de directivas para Teams para poner las coincidencias de directivas en la atención de los usuarios para la corrección.

## <a name="create-a-policy-from-a-template"></a>Creación de una directiva a partir de una plantilla

Siga estos pasos para crear una directiva mediante cualquiera de las plantillas predeterminadas.

1. En el [portal de cumplimiento de Microsoft Purview](https://compliance.microsoft.com/), vaya a la sección Priva Privacy Risk Management y seleccione **Directivas**.
1. Seleccione **Crear directiva**.
1. Elija el tipo de plantilla que desee. Se abrirá un panel flotante con información sobre la plantilla.
1. Para revisar la configuración predeterminada de la plantilla, incluidos los tipos de datos, las ubicaciones de datos y las condiciones que desencadenan coincidencias de directiva, seleccione **Ver configuración**.
     - Aquí tiene la opción de seleccionar **Editar configuración** para realizar cambios. Esto le dirigirá al asistente para personalizar la configuración.
1. Si está listo para usar la configuración predeterminada, asigne un nombre descriptivo a la directiva y seleccione **Crear directiva.**

Al crear una directiva directamente desde una plantilla, se elegirán muchas opciones automáticamente. También se iniciará en modo de prueba de forma predeterminada, lo que significa que no se generarán alertas ni notificaciones. Si está listo para activar completamente la directiva después de ejecutarla en modo de prueba y revisar los resultados de la directiva, puede encontrarla en la lista de directivas y editarla para activarla.

## <a name="create-a-custom-policy"></a>Crear una directiva personalizada

Para tomar un control pormenorizado de la configuración de una directiva, puede crear una directiva personalizada mediante una de las plantillas existentes como línea base. Priva proporciona un asistente para guiarle a través de estos pasos.

Todos los tipos de directiva siguen este flujo básico. Ciertas opciones y configuraciones cambiarán en función de la directiva elegida.

1. En el [portal de cumplimiento de Microsoft Purview](https://compliance.microsoft.com/), vaya a la sección Priva Privacy Risk Management y seleccione **Directivas**.
1. Seleccione **Crear directiva**.
1. Elija la opción **Personalizada** para empezar a usar el asistente.
1. Elija el tipo de plantilla de línea base: **sobreexposición de datos,** **Transferencias de datos** o **Minimización de datos**. Cada uno de ellos le proporcionará ciertas opciones durante la creación de la directiva.
1. Asigne un nombre y describa la directiva. Se recomienda usar nombres descriptivos y claros para identificar las directivas, ya que estos nombres aparecerán más adelante en las alertas sobre coincidencias de directivas.
1. Continúe con el asistente y elija la configuración que desee. Entre las opciones se incluyen:
    - **Datos que se van a supervisar**: seleccione el tipo de datos personales que supervisará la directiva.
    - **Usuarios y grupos**: aplique la directiva a todos los usuarios o usuarios seleccionados.
    - **Ubicaciones**: aplique la directiva a las áreas seleccionadas en Microsoft 365.
    - **Condiciones**: establezca las condiciones de la directiva. Estas opciones varían en función del tipo de directiva.
    - **Resultados**: defina los resultados cuando se encuentre una coincidencia de directiva, como las notificaciones de usuario.
    - **Alertas**: decida la frecuencia de las alertas para los administradores cuando se encuentre una coincidencia de directiva.
    - **Modo**: elija si primero debe ejecutar la directiva en modo de prueba.
1. Cuando se completen todas las opciones, revise las opciones, realice las modificaciones deseadas y, a continuación, seleccione **Enviar** para crear la directiva.

## <a name="learn-about-key-settings-for-all-policies"></a>Más información sobre la configuración de claves para todas las directivas

### <a name="choose-data-to-monitor"></a>Elección de los datos que se van a supervisar

Al editar o configurar cualquier tipo de directiva personalizada, se le pedirá que seleccione qué tipos de datos debe supervisar la directiva. A continuación se indican las opciones posibles:

- **Grupos de clasificación**: una lista de conjuntos de datos que se pueden buscar en función de las normativas de privacidad clave, como RGPD o HIPAA. Vea los detalles de cualquier grupo para ver qué tipos de información confidencial trata. Seleccione uno o varios de estos conjuntos para usarlos tal y como están.
- **Tipos de información confidencial individuales**: si elige tipos de información confidencial específicos usted mismo, como números del Seguro Social o información de licencia de conducir, puede personalizar su propio grupo o grupos de datos para que lo busquen. Este asistente le permite seleccionar de la lista completa de tipos de información confidencial en Privacy Risk Management. Cada tipo de información tiene sus propias propiedades. Use el botón de información situado junto a cualquiera de ellos para obtener detalles y notas sobre la configuración recomendada. Si crea más de un grupo, el asistente le permite aplicar operadores booleanos para relacionarlos y definir su orden de operaciones.

Si selecciona entre los grupos de clasificación existentes, tampoco puede seleccionar tipos individuales ni crear sus propios grupos. Para obtener la mayor flexibilidad, elija tipos de información confidencial individuales. Para usar los estándares más comunes, elija entre los grupos de clasificación.

### <a name="set-user-email-notifications"></a>Establecimiento de notificaciones por correo electrónico de usuario

Con [las notificaciones por correo electrónico](risk-management-notifications.md), puede enviar notificaciones sobre coincidencias de directivas directamente a los propietarios de contenido. En estos correos electrónicos se resumen los datos que se deben revisar y las posibles acciones que se deben realizar, como hacer que los documentos sean privados, mantenerlos en el archivo, notificar las coincidencias de falsos positivos y agregar notas para futuras referencias. Estos correos electrónicos también incluyen vínculos para entrenar a los destinatarios sobre cómo controlar estos casos. Proporcionar estos vínculos es necesario y debe apuntar a su propia documentación interna sobre procesos y procedimientos recomendados.

Las notificaciones se pueden habilitar para directivas individuales durante la creación de directivas personalizadas o al editar cualquier directiva. Establezca sus preferencias en la sección **Resultados** .

La configuración necesaria incluye la frecuencia de las notificaciones y el vínculo al entrenamiento de privacidad.

La configuración opcional incluye determinados campos personalizables para los correos electrónicos. Seleccione la opción **Vista previa y edición del correo de notificación** para abrir un panel flotante que muestra una notificación de ejemplo. Aquí puede editar la línea de asunto del correo electrónico, el encabezado y el texto del cuerpo, y el nombre para mostrar y la dirección URL para el entrenamiento de privacidad.

Tenga en cuenta que la funcionalidad general de Privacy Risk Management para enviar notificaciones por correo electrónico se controla en **Configuración**. Está habilitada de forma predeterminada. Si desactiva esta configuración, se detendrán todos los correos electrónicos, incluso si las notificaciones se han configurado en un nivel de directiva individual.

## <a name="learn-about-settings-for-data-minimization-policies"></a>Más información sobre la configuración de las directivas de minimización de datos

Las directivas de minimización de datos se centran en la antigüedad del contenido y en cuánto tiempo ha pasado desde que se modificó por última vez. La supervisión de los datos personales que todavía se conservan en contenido antiguo sin usar puede ayudarle a administrar mejor los datos almacenados y a reducir los riesgos. Esta configuración se controla en la pantalla **Condiciones** .

De forma predeterminada, las directivas de minimización de datos buscan contenido que contenga datos personales que se crearon o modificaron por última vez hace al menos 30 días. Al editar o crear una directiva personalizada, puede seleccionar entre otros períodos de tiempo preestablecidos.

## <a name="learn-about-settings-for-data-transfer-policies"></a>Más información sobre la configuración de las directivas de transferencia de datos

Las directivas de transferencia de datos le permiten supervisar las transferencias de datos personales fuera de su organización, así como las transferencias internas entre diferentes departamentos, países o regiones. En la pantalla **Condiciones** , puede elegir qué tipos de transferencias debe buscar Privacy Risk Management.

De forma predeterminada, las directivas de transferencia de datos detectan cuándo se transfieren o comparten datos personales dentro de la organización a un destinatario o ubicación fuera de la organización. Al editar o crear una directiva personalizada, puede elegir el tipo de transferencia y, a continuación, realizar selecciones para las regiones o departamentos del remitente y del destinatario.

Las directivas de transferencia de datos también admiten el suministro de sugerencias y recomendaciones de directivas a los usuarios en Teams, de modo que puedan mantenerse informados sobre los procedimientos recomendados para controlar los datos. Esto se puede alternar en la pantalla **Resultados** .

## <a name="learn-about-settings-for-data-overexposure-policies"></a>Más información sobre la configuración de las directivas de sobreexposición de datos

Su organización puede almacenar contenido en varios niveles de acceso, incluidas las áreas a las que se puede acceder públicamente y otras que están restringidas. En la pantalla **Condiciones** , puede optar por que Privacy Risk Management busque posibles sobreexplotación de datos para el contenido almacenado en cualquiera de los siguientes niveles de acceso:

- **Público**: cualquier persona con un vínculo puede ver este contenido.
- **Externo**: las personas específicas fuera de la organización tienen acceso.
- **Interno**: los usuarios de la organización tienen acceso.

De forma predeterminada, las directivas de sobreexposición de datos evalúan los tres niveles de acceso. Al editar o crear una directiva personalizada, puede elegir todos o cualquiera de estos niveles.

## <a name="next-steps"></a>Siguientes pasos

Para obtener más información sobre cómo administrar las directivas y realizar cambios una vez creadas, consulte [Administrar directivas](risk-management-policies-manage.md).

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legal

[Declinación de responsabilidades legal de Microsoft Priva](priva-disclaimer.md)
