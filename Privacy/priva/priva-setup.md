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
ms.openlocfilehash: e88145dc999e210f36a8dc82e1bc9996bc15bb88
ms.sourcegitcommit: 09ecdaded9a9f8f79587f2acb978dc53b83e5c01
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/19/2022
ms.locfileid: "64930561"
---
# <a name="get-started-with-priva"></a>Introducción a Priva

Si está listo para empezar a usar Microsoft Priva para obtener ayuda para identificar y mitigar los riesgos de privacidad, siga estos pasos para configurar los requisitos previos y empezar a explorar la información de privacidad.

## <a name="step-1-confirm-subscriptions-and-licensing"></a>Paso 1: Confirmar suscripciones y licencias

Priva está disponible en el [portal de cumplimiento de Microsoft Purview](https://compliance.microsoft.com/) y las organizaciones pueden comprarla con las siguientes licencias:

- Microsoft 365 E3, E5, A3, A5
- Office 365 E1, E3, E5, A1, A3, A5

Priva ofrece opciones de licencia para dos soluciones diferentes: Priva Privacy Risk Management y Priva Subject Rights Requests. Estos se pueden comprar individualmente o juntos. Al obtener licencias para solicitudes de derechos de sujeto, puede elegir el nivel de licencia adecuado para el número de solicitudes que necesita controlar. Puede comprar solicitudes adicionales en cualquier momento.

Para una guía detallada sobre las licencias, vea: [Guía de licencias de Microsoft 365 para la seguridad y el cumplimiento](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-tenantlevel-services-licensing-guidance/microsoft-365-security-compliance-licensing-guidance#microsoft-priva).

> [!Note]
> Priva no está disponible para los clientes moderados, GCC altos o del Departamento de Defensa (DoD) del Community Gobierno de EE. UU. (GCC).

### <a name="get-free-trial-license"></a>Obtención de una licencia de prueba gratuita

Hay disponible una licencia de prueba gratuita para empezar a trabajar con Priva. Para obtener información sobre la elegibilidad y cómo unirse, consulte [Información sobre la evaluación gratuita de Priva](priva-trial.md).

## <a name="step-2-enable-the-microsoft-365-audit-log"></a>Paso 2: Habilitar el registro de auditoría de Microsoft 365

Microsoft 365 registros de auditoría son un resumen de todas las actividades dentro de la organización. Las directivas de administración de riesgos de privacidad pueden usar estas actividades para generar información sobre directivas.

Es posible que la organización ya tenga activados los registros de auditoría. Si necesita empezar a usarlos por primera vez, consulte [Activar o desactivar la búsqueda de registros de auditoría](/microsoft-365/compliance/turn-audit-log-search-on-or-off) para obtener instrucciones paso a paso para activar la auditoría. Después de activar la auditoría, se muestra un mensaje que dice que el registro de auditoría se está preparando y que puede ejecutar una búsqueda en un par de horas después de que se complete la preparación. Solo tiene que realizar esta acción una vez. Para obtener más información sobre cómo usar el registro de auditoría de Microsoft 365, vea [Buscar en el registro de auditoría](/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).

## <a name="step-3-set-user-permissions-and-assign-roles"></a>Paso 3: Establecer permisos de usuario y asignar roles

Priva usa un modelo de permisos de control de acceso basado en rol (RBAC). Solo los usuarios a los que se les asigna un rol pueden acceder a Priva y las acciones permitidas por cada usuario están restringidas por tipo de rol.

El administrador global tiene permisos para acceder a Priva y asignar otros usuarios a roles. Pueden iniciar sesión y establecer permisos de usuario en el [portal de cumplimiento de Microsoft Purview](https://compliance.microsoft.com/) para Priva. Para un inicio rápido, el grupo de roles Administración de privacidad tiene permisos para acceder a todas las características de Priva. Este grupo puede ser una buena opción para las organizaciones en las que la misma persona puede realizar todas las tareas. Otros roles de privacidad le permiten tomar un control más pormenorizado y asignar usuarios a características o funciones seleccionadas.

Para obtener más información sobre los grupos de roles y cómo conceder acceso, consulte [Establecer permisos de usuario y asignar roles en Priva](priva-permissions.md).

## <a name="step-4-start-finding-and-visualizing-your-data"></a>Paso 4: Empezar a buscar y visualizar los datos

Después de iniciar sesión en Priva, verá la página **Información general** . En esta página se proporciona información dinámica sobre cómo evolucionan los datos personales en el entorno de Microsoft 365 para ayudarle a detectar problemas rápidamente, identificar indicadores de riesgo y tomar medidas para corregir problemas. La información general debe rellenarse con información inicial en las primeras 24 horas después de registrarse. A medida que siga usando Priva, la página de información general se actualizará para continuar proporcionando información actual.

Para obtener más información sobre los datos a lo largo del tiempo **, la página** Perfil de datos proporcionará más visualizaciones y análisis y le proporcionará una vista holística de los datos de su organización por ubicación geográfica y por ubicación Microsoft 365.

Para obtener más información sobre estas páginas, consulte [Búsqueda y visualización de datos personales en Priva](priva-data-profile.md).

## <a name="step-5-start-managing-risks-with-default-policies"></a>Paso 5: Inicio de la administración de riesgos con directivas predeterminadas

Privacy Risk Management comenzará a evaluar los datos y le dará un vistazo a los escenarios de riesgo clave para la minimización de datos, la sobreexposición de datos y las transferencias de datos. Estas directivas están activadas de forma predeterminada. Puede usar estas directivas para evaluar dónde están los riesgos y, a continuación, activar las notificaciones por correo electrónico del usuario para que los usuarios puedan plantear problemas a su atención y guiar la corrección de estos riesgos. Además, puede crear y personalizar sus propias directivas a partir de las plantillas de directiva proporcionadas. Puede adaptar las directivas para satisfacer las necesidades legales y de cumplimiento normativo de su organización, tal como se puede identificar en consulta con el asesor legal. Para más información, consulte [Creación de directivas en Privacy Risk Management](risk-management-policies.md).

## <a name="step-6-get-started-with-subject-rights-requests"></a>Paso 6: Comenzar con solicitudes de derechos del sujeto

Priva Subject Rights Requests automatiza el proceso de cumplimiento de solicitudes de derechos del sujeto, lo que proporciona un fácil acceso a los datos y flujos de trabajo personalizables que encajan en los procesos empresariales existentes. Puede encontrar fácilmente los datos pertinentes, revisar los resultados y generar informes. En el camino, puede colaborar de forma segura con otros expertos de su organización para completar la solicitud de derechos del sujeto. También puede administrar y personalizar los flujos de trabajo empresariales con plantillas integradas. Para obtener más información sobre el uso de estas características, consulte [Información sobre las solicitudes de derechos de los sujetos privados](subject-rights-requests.md).

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legal

[Declinación de responsabilidades legal de Microsoft Priva](priva-disclaimer.md)
