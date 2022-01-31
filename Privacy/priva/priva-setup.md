---
title: Introducción a Priva
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
- M365-priva-privacy-risk-management
search.appverid:
- MOE150
- MET150fcf
description: Obtenga información sobre cómo configurar Microsoft Priva para su organización, establecer roles y permisos y configurar opciones importantes.
ms.openlocfilehash: 8df9367bd88fe9a8feecdbb00110345aae7a3d79
ms.sourcegitcommit: a76dec53605c963d9bc134a26b7e09f600d6e940
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/31/2022
ms.locfileid: "62280252"
---
# <a name="get-started-with-priva"></a>Introducción a Priva

Si está listo para empezar a usar Microsoft Priva para obtener ayuda para identificar y mitigar los riesgos de privacidad, siga estos pasos para configurar los requisitos previos y empezar a explorar la información de privacidad.

## <a name="step-1-confirm-subscriptions-and-licensing"></a>Paso 1: Confirmar suscripciones y licencias

Priva está disponible en el [Centro de cumplimiento de Microsoft 365](https://compliance.microsoft.com/) y las organizaciones pueden comprar con las siguientes licencias:

- Microsoft 365 E3, E5, A3, A5
- Office 365 E1, E3, E5, A1, A3, A5

Priva ofrece opciones de licencias para dos soluciones diferentes: Priva Privacy Risk Management y Priva Subject Rights Requests. Estos se pueden comprar individualmente o juntos. Al obtener licencias para solicitudes de derechos de sujeto, puede elegir el nivel de licencia adecuado para el número de solicitudes que necesita controlar. Puedes comprar solicitudes adicionales en cualquier momento.

Para una guía detallada sobre las licencias, vea: [Guía de licencias de Microsoft 365 para la seguridad y el cumplimiento](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-tenantlevel-services-licensing-guidance/microsoft-365-security-compliance-licensing-guidance#microsoft-priva).

> [!Note]
> Priva no está disponible para los Community (GCC) moderados, GCC altos o del Departamento de Defensa (DoD).

### <a name="get-free-trial-license"></a>Obtener licencia de prueba gratuita

Hay una licencia de prueba gratuita disponible para empezar a trabajar con Priva. Para obtener información sobre la elegibilidad y cómo unirse, consulte [Learn about the free Priva trial](priva-trial.md).

## <a name="step-2-enable-the-microsoft-365-audit-log"></a>Paso 2: Habilitar el registro Microsoft 365 auditoría

Microsoft 365 registros de auditoría son un resumen de todas las actividades dentro de la organización. Las directivas de administración de riesgos de privacidad pueden usar estas actividades para generar información sobre directivas.

Es posible que su organización ya tenga los registros de auditoría activados. Si necesita empezar a usarlos por primera vez, vea [Activar](/microsoft-365/compliance/turn-audit-log-search-on-or-off) o desactivar la búsqueda del registro de auditoría para obtener instrucciones paso a paso para activar la auditoría. Después de activar la auditoría, se muestra un mensaje que dice que el registro de auditoría se está preparando y que puede ejecutar una búsqueda en un par de horas después de que se complete la preparación. Solo tiene que realizar esta acción una vez. Para obtener más información acerca del uso del Microsoft 365 de auditoría, vea [Buscar en el registro de auditoría](/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).

## <a name="step-3-set-user-permissions-and-assign-roles"></a>Paso 3: Establecer permisos de usuario y asignar roles

Priva usa un modelo de permisos de control de acceso basado en roles (RBAC). Solo los usuarios a los que se asigna un rol pueden tener acceso a Priva y las acciones permitidas por cada usuario están restringidas por tipo de función.

El administrador global tiene permisos para tener acceso a Priva y asignar otros usuarios a roles. Pueden iniciar sesión y establecer permisos de usuario en el [Centro de cumplimiento de Microsoft 365](https://compliance.microsoft.com/) para Priva. Para un inicio rápido, el grupo de roles De administración de privacidad tiene permisos para tener acceso a todas las características de Priva. Este grupo puede ser un buen ajuste para las organizaciones donde la misma persona puede realizar todas las tareas. Otros roles de privacidad le permiten tomar un control más detallado y asignar usuarios a funciones o características seleccionadas.

Para obtener más información sobre los grupos de roles y cómo conceder acceso, consulte [Establecer permisos de usuario y asignar roles en Priva](priva-permissions.md).

## <a name="step-4-start-finding-and-visualizing-your-data"></a>Paso 4: Empezar a buscar y visualizar los datos

Después de iniciar sesión en Priva, verá la página **Información** general. Esta página proporciona información dinámica sobre cómo evolucionan los datos personales en su entorno de Microsoft 365 para ayudarle a detectar rápidamente problemas, identificar indicadores de riesgo y tomar medidas para solucionar problemas. Su información general debe rellenarse con información inicial en las primeras 24 horas de registrarse. A medida que siga usando Priva, la página de información general se actualizará para continuar con la información actual.

Para obtener más información sobre los datos con el tiempo,  la página perfil de datos proporcionará más visualizaciones y análisis y le proporcionará una vista holística de los datos de su organización por ubicación geográfica y por ubicación Microsoft 365 datos.

Para obtener más información sobre estas páginas, vea [Buscar y visualizar datos personales en Priva](priva-data-profile.md).

## <a name="step-5-start-managing-risks-with-default-policies"></a>Paso 5: Empezar a administrar riesgos con directivas predeterminadas

La Administración de riesgos de privacidad empezará a evaluar los datos y le dará una mirada a escenarios de riesgo clave para la minimización de datos, la sobreexposición de datos y las transferencias de datos. Estas directivas están activadas de forma predeterminada. Puede usar estas directivas para evaluar dónde están sus riesgos y, a continuación, activar las notificaciones de correo electrónico de los usuarios para que los usuarios les presten atención y orientar la corrección de estos riesgos. Además, puede crear y personalizar sus propias directivas a partir de las plantillas de directiva proporcionadas. Puede adaptar sus directivas para satisfacer las necesidades legales y de cumplimiento normativo de su organización, tal como se puede identificar en consulta con el asesor jurídico. Para obtener más información, consulte [Create policies in Privacy Risk Management](risk-management-policies.md).

## <a name="step-6-get-started-with-subject-rights-requests"></a>Paso 6: Introducción a las solicitudes de derechos de sujeto

Priva Subject Rights Requests automatiza el proceso de cumplimiento de solicitudes de derechos de sujeto, lo que proporciona un fácil acceso a los datos y flujos de trabajo personalizables que se ajustan a los procesos empresariales existentes. Puede encontrar fácilmente los datos relevantes, revisar los resultados y producir informes. En el camino, puede colaborar de forma segura con otros expertos de su organización para completar la solicitud de derechos del sujeto. También puede administrar y personalizar los flujos de trabajo de su empresa con plantillas integradas. Para obtener más información sobre el uso de estas características, consulte [Información sobre solicitudes de derechos del sujeto priva](subject-rights-requests.md).

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legales

[Declinación de responsabilidades legales de Microsoft Priva](priva-disclaimer.md)
