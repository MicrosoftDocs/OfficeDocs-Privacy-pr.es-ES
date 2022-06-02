---
title: Notificaciones de usuario en Administración de riesgos de privacidad
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
description: Obtenga información sobre cómo notificar a los propietarios de contenido las coincidencias de directivas encontradas por Gestión de riesgos de privacidad Microsoft Priva y cómo pueden usar estas notificaciones por correo electrónico para corregir problemas.
ms.openlocfilehash: ae02d3bca9c63f8645cd9671628de61d83cb6117
ms.sourcegitcommit: 9315064bf5bb9e889318e61ec5f082f36c815e1e
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/02/2022
ms.locfileid: "65851655"
---
# <a name="user-notifications-in-privacy-risk-management"></a>Notificaciones de usuario en Administración de riesgos de privacidad

Al configurar una directiva en Privacy Risk Management, puede optar por notificar a los usuarios cuando sus acciones cumplan las condiciones establecidas en la directiva. Hay dos tipos de notificaciones: correos electrónicos, que están disponibles para los tres tipos de directiva, y sugerencias que aparecen en Teams, que solo están disponibles para el tipo de directiva de transferencia de datos. Al crear o editar una directiva, puede decidir si activar estas notificaciones, con qué frecuencia enviarlas y personalizar su contenido.

El envío de notificaciones a los usuarios puede ser un componente importante para ayudar a su organización a cumplir sus objetivos de privacidad. Las notificaciones están diseñadas para:

- Dar a conocer inmediatamente a los usuarios cuándo sus acciones podrían exponer los datos personales a riesgos de privacidad.
- Proporcione métodos de corrección directamente dentro de los correos electrónicos para que los usuarios puedan tomar medidas rápidas para proteger los datos en riesgo.
- Dirija a los usuarios a las directrices de privacidad y los procedimientos recomendados de su organización.

Informar a los usuarios de posibles problemas en el momento y capacitarlos para corregir problemas y actualizar sus aptitudes, puede ser herramientas eficaces para crear prácticas de control de datos sólidas en toda la organización.

Revise las secciones siguientes para ayudarle a preparar y administrar las notificaciones de usuario para las coincidencias de directivas.

## <a name="prepare-training-content-for-notifications"></a>Preparación del contenido de entrenamiento para las notificaciones

Se requiere incluir un vínculo al entrenamiento de privacidad si decide enviar notificaciones de usuario cuando se detectan coincidencias de directivas. Proporcionar acceso a las directrices de privacidad de su organización le permite mantener informados a los usuarios sobre sus propios procedimientos recomendados y directivas. También puede dar contexto a las acciones de corrección sugeridas en el correo electrónico y ayudar a los usuarios a prepararse para tomar buenas decisiones de administración de datos en el futuro.

Antes de configurar la directiva, decida la dirección URL de entrenamiento que desea incluir. Se puede proporcionar un vínculo por directiva, por lo que se recomienda elegir referencias específicas para cada escenario.

## <a name="set-user-email-notifications"></a>Establecimiento de notificaciones por correo electrónico de usuario

Puede configurar notificaciones por correo electrónico para todos los tipos de directiva al crear una nueva directiva o editar una directiva existente. Esta configuración se encuentra en la página **Resultados** del Asistente para la creación de directivas. Visite [Definir resultados: notificaciones de usuario y sugerencias](risk-management-policies.md#define-outcomes-user-email-notifications-and-tips) para obtener las instrucciones completas.

> [!NOTE]
> La funcionalidad general de Privacy Risk Management para enviar notificaciones por correo electrónico se controla en Priva **Configuración**. Está habilitada de forma predeterminada. Si desactiva esta configuración, se detendrán todos los correos electrónicos, incluso si las notificaciones se han configurado en un nivel de directiva individual. Obtenga más información sobre la [configuración del correo electrónico de notificación de usuario](priva-settings.md#user-notification-emails).

## <a name="send-notifications-in-teams"></a>Envío de notificaciones en Teams

En el caso de las directivas de transferencia de datos, puede elegir que los usuarios reciban sugerencias y recomendaciones de directivas en canales de Teams seguros cuando se detecta una coincidencia de directiva. Estas sugerencias informan a los usuarios sobre el uso responsable de los datos personales. Sugerencias también incluirá vínculos a entrenamiento relacionado.

Para obtener más información sobre cómo configurar estas notificaciones, visite [Definir resultados: notificaciones y sugerencias de usuario](risk-management-policies.md#define-outcomes-user-email-notifications-and-tips).

## <a name="preview-and-customize-email-content"></a>Vista previa y personalización del contenido del correo electrónico

Cuando los usuarios reciben notificaciones por correo electrónico sobre coincidencias de directivas, pueden seguir las indicaciones de los correos electrónicos para realizar inmediatamente una acción correctiva. Por ejemplo, si una directiva de sobreexposición de datos encuentra una coincidencia para los datos personales que pueden ser demasiado accesibles, el correo electrónico de notificación incluye un vínculo al elemento de contenido para que el usuario pueda revisarlo y botones para que el usuario marque el elemento como privado o mantenga su nivel de acceso actual. Las acciones sugeridas serán pertinentes para cada tipo de directiva diferente.

Puede obtener una vista previa del contenido del correo electrónico y realizar sus propios cambios al ajustar esta configuración en el proceso de creación o edición de directivas. Para obtener una vista previa y editar el contenido del correo electrónico de notificación, siga estos pasos:

1. Cree o edite la directiva iniciando los pasos descritos en el [proceso de creación de directivas guiadas](risk-management-policies.md#custom-setup-guided-process-to-choose-all-settings).

2. En el paso **Resultados** del proceso, seleccione el cuadro situado junto a **Enviar un correo electrónico de notificación a los usuarios cuando se produzca una coincidencia de directiva**.

3. Seleccione el botón **Vista previa y editar correo electrónico de notificación** que aparece debajo de la casilla de correo electrónico de notificación.

4. Aparece un panel flotante con campos de texto rellenados previamente con el contenido de correo electrónico predeterminado. Puede editar cualquiera o todos los campos, entre los que se incluyen: la línea de asunto del correo electrónico, el encabezado del cuerpo, el contenido del cuerpo, el nombre para mostrar del entrenamiento de privacidad y la dirección URL de entrenamiento. La vista previa del correo electrónico se encuentra en la parte inferior del panel flotante y cambiará a medida que realice modificaciones en el texto predeterminado. Cuando esté satisfecho con el contenido del correo electrónico, seleccione **Guardar** para guardar la configuración. Para descartar los cambios en el correo electrónico predeterminado, seleccione la **X** en la esquina superior derecha del panel flotante para cerrarlo y volver al contenido predeterminado.

5. En la página **Resultados** , seleccione **Siguiente**. Continúe con el asistente y, cuando llegue a la página **Finalizar** final, revise la configuración y seleccione **Enviar**.

La configuración de notificación ahora estará en vigor para esta directiva. Si la directiva se está probando, no se enviarán notificaciones. Si la directiva está activada, se enviarán notificaciones. Vea más detalles sobre [cómo crear y administrar directivas](risk-management-policies.md).


## <a name="legal-disclaimer"></a>Declinación de responsabilidades legal

[Microsoft Priva declinación de responsabilidades legal](priva-disclaimer.md)
