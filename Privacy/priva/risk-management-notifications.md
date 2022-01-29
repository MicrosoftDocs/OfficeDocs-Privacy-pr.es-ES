---
title: Enviar notificaciones de usuario en Administración de riesgos de privacidad
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
description: Obtenga información sobre cómo notificar a los propietarios de contenido sobre las coincidencias de directivas encontradas por la Administración de riesgos de privacidad y cómo pueden usar estas notificaciones de correo electrónico para corregir problemas.
ms.openlocfilehash: 2215224adf932f806f16429560d4a694cd47a859
ms.sourcegitcommit: f145dff5e387a8e26db2f3a2c7de125978fbacc9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/28/2022
ms.locfileid: "62249088"
---
# <a name="send-user-notifications-in-privacy-risk-management"></a>Enviar notificaciones de usuario en Administración de riesgos de privacidad

La administración de riesgos de privacidad en Microsoft Priva puede notificar directamente a los propietarios de contenido las coincidencias de las directivas de sobreexposición de datos, minimización de datos y transferencia de datos. Con las notificaciones por correo electrónico, los usuarios pueden averiguar fácilmente el contenido que necesitan revisar y pueden usar mensajes directamente en el correo electrónico para aplicar las acciones correctivas adecuadas. Estos correos electrónicos también incluyen vínculos a su propia formación en privacidad. Para las directivas de transferencia de datos, también puede compartir notificaciones y sugerencias de directivas en Teams canales.

## <a name="prepare-training-content-for-policy-notifications"></a>Preparar contenido de aprendizaje para notificaciones de directivas

Es necesario incluir un vínculo a la formación en privacidad para las directivas que generan notificaciones. Proporcionar acceso a las directrices de privacidad de su organización le permite mantener a los usuarios informados sobre sus propios procedimientos recomendados y directivas. También puede dar contexto a las acciones de corrección sugeridas en el correo electrónico y ayudar a los usuarios a prepararse para tomar buenas decisiones de administración de datos en el futuro.

Antes de configurar la directiva, decide la dirección URL de aprendizaje que quieras incluir. Se puede proporcionar un vínculo por directiva, por lo que se recomienda elegir referencias específicas para cada escenario.

## <a name="set-up-email-notifications-for-policies"></a>Configurar notificaciones de correo electrónico para directivas

Las notificaciones de correo electrónico se pueden configurar al crear una directiva personalizada o editar cualquier directiva. Consulta [Crear directivas en Administración de riesgos de privacidad](risk-management-policies.md) para obtener las instrucciones completas. La configuración de notificaciones por correo electrónico se encuentra en la **pestaña Resultados** del asistente para directivas. Aquí puede decidir la frecuencia con la que desea enviar notificaciones, establecer la dirección URL de aprendizaje de privacidad y escribir cualquier texto personalizado para el asunto o el cuerpo del correo electrónico.

## <a name="remediate-issues-from-email-notifications"></a>Corregir problemas de notificaciones de correo electrónico

Cuando los usuarios reciben notificaciones por correo electrónico sobre coincidencias de directiva, pueden seguir las indicaciones de los correos electrónicos para tomar inmediatamente medidas correctivas. Por ejemplo, si una directiva de sobreexposición de datos encuentra una coincidencia con los datos personales que pueden ser demasiado accesibles, el correo electrónico resultante puede proporcionar avisos de botón para que el elemento sea privado. Si el elemento indicado debe conservarse tal como está, los usuarios también pueden elegir conservar el elemento. Las acciones sugeridas serán relevantes para cada tipo de directiva.

## <a name="send-notifications-in-teams"></a>Enviar notificaciones en Teams

Para las directivas de transferencia de datos, los usuarios pueden recibir sugerencias y recomendaciones de directivas en canales de Teams seguros cuando se detecta una coincidencia de directiva. Estas sugerencias educan a los usuarios sobre el uso responsable de datos personales. Sugerencias también incluirá vínculos a cursos relacionados.

Para obtener más información sobre cómo configurar estas notificaciones, consulta [Crear directivas en Administración de riesgos de privacidad](risk-management-policies.md#set-user-email-notifications).

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legales

[Declinación de responsabilidades legales de Microsoft Priva](priva-disclaimer.md)
