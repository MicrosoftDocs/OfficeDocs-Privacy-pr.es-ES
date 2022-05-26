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
description: Obtenga información sobre cómo configurar Microsoft Priva para su organización, establecer roles y permisos y configurar valores importantes.
ms.openlocfilehash: 945cbfd2625be50cb89eeaa8fe09e0effaea79d5
ms.sourcegitcommit: 3c27ecf7c86c8a3db38cae8819fc090eed192b4f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/25/2022
ms.locfileid: "65678217"
---
# <a name="get-started-with-priva"></a>Introducción a Priva

Si está listo para empezar a usar Microsoft Priva para ayudar a su organización a identificar y mitigar los riesgos de privacidad, siga estos pasos para ayudarle a configurarse.

## <a name="confirm-subscriptions-and-licensing"></a>Confirmación de suscripciones y licencias

Priva está disponible en el [portal de cumplimiento Microsoft Purview](https://compliance.microsoft.com/) y las organizaciones pueden adquirirla con las siguientes licencias:

- Microsoft 365 E3, E5, A3, A5
- Office 365 E1, E3, E5, A1, A3, A5

Priva ofrece opciones de licencia para dos soluciones diferentes: Administración de riesgo de privacidad Priva y Solicitudes de los interesados Priva. Estos se pueden comprar individualmente o juntos. Al obtener licencias para solicitudes de derechos de sujeto, puede elegir el nivel de licencia adecuado para el número de solicitudes que necesita controlar. Puede comprar solicitudes adicionales en cualquier momento.

Para una guía detallada sobre las licencias, vea: [Guía de licencias de Microsoft 365 para la seguridad y el cumplimiento](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-tenantlevel-services-licensing-guidance/microsoft-365-security-compliance-licensing-guidance#microsoft-priva).

> [!Note]
> Priva no está disponible para los clientes de Community (GCC) moderados, GCC altos o del Departamento de Defensa (DoD).

### <a name="start-a-free-trial"></a>Iniciar una prueba gratuita

Use una suscripción de prueba gratuita para explorar todas las características y funcionalidades de ambas soluciones de Priva. Obtenga información sobre cómo registrarse para la [prueba de Priva](priva-trial.md).

## <a name="enable-the-microsoft-365-audit-log"></a>Habilitación del registro de auditoría de Microsoft 365

Microsoft 365 registros de auditoría son un resumen de todas las actividades dentro de la organización. Las directivas de administración de riesgos de privacidad pueden usar estas actividades para generar información sobre directivas.

Es posible que la organización ya tenga activados los registros de auditoría. Si necesita empezar a usarlos por primera vez, consulte [Activar o desactivar la búsqueda de registros de auditoría](/microsoft-365/compliance/turn-audit-log-search-on-or-off) para obtener instrucciones paso a paso para activar la auditoría. Después de activar la auditoría, se muestra un mensaje que dice que el registro de auditoría se está preparando y que puede ejecutar una búsqueda en un par de horas después de que se complete la preparación. Solo tiene que realizar esta acción una vez. Para obtener más información sobre cómo usar el registro de auditoría de Microsoft 365, vea [Buscar en el registro de auditoría](/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).

## <a name="set-user-permissions-and-assign-roles"></a>Establecimiento de permisos de usuario y asignación de roles

Priva usa un modelo de permisos de control de acceso basado en rol (RBAC). Solo los usuarios a los que se les asigna un rol pueden acceder a Priva y las acciones permitidas por cada usuario están restringidas por tipo de rol.

El administrador global tiene permisos para acceder a Priva y asignar otros usuarios a roles. Pueden iniciar sesión y establecer permisos de usuario en el [portal de cumplimiento Microsoft Purview](https://compliance.microsoft.com/) para Priva. Para un inicio rápido, el grupo de roles Administración de privacidad tiene permisos para acceder a todas las características de Priva. Este grupo puede ser una buena opción para las organizaciones en las que la misma persona puede realizar todas las tareas. Otros roles de privacidad le permiten tomar un control más pormenorizado y asignar usuarios a características o funciones seleccionadas.

Para obtener más información sobre los grupos de roles y cómo conceder acceso, consulte [Establecimiento de permisos de usuario y asignación de roles en Priva](priva-permissions.md).

## <a name="start-finding-and-visualizing-your-data"></a>Empezar a buscar y visualizar los datos

Después de iniciar sesión en Priva, verá la página **Información general**. En esta página se proporciona información dinámica sobre cómo evolucionan los datos personales en el entorno de Microsoft 365 para ayudarle a detectar problemas rápidamente, identificar indicadores de riesgo y tomar medidas para corregir problemas. La información general debe rellenarse con información inicial en las primeras 24 horas después de registrarse. A medida que siga usando Priva, la página de información general se actualizará para continuar proporcionando información actual.

Para obtener más información sobre los datos a lo largo del tiempo **, la página** Perfil de datos proporcionará más visualizaciones y análisis y le proporcionará una vista holística de los datos de su organización por ubicación geográfica y por ubicación Microsoft 365.

Para más información sobre estas páginas, consulte [Búsqueda y visualización de datos personales en Priva](priva-data-profile.md).

## <a name="start-managing-risks-with-default-policies"></a>Inicio de la administración de riesgos con directivas predeterminadas

Privacy Risk Management comenzará a evaluar los datos y le dará un vistazo a los escenarios de riesgo clave para la minimización de datos, la sobreexposición de datos y las transferencias de datos. Estas directivas están activadas de forma predeterminada. Puede usar estas directivas para evaluar dónde están los riesgos y, a continuación, activar las notificaciones por correo electrónico del usuario para que los usuarios puedan plantear problemas a su atención y guiar la corrección de estos riesgos. Además, puede crear y personalizar sus propias directivas a partir de las plantillas de directiva proporcionadas. Puede adaptar las directivas para satisfacer las necesidades legales y de cumplimiento normativo de su organización, tal como se puede identificar en consulta con el asesor legal. Para más información, consulte [Creación de directivas en Privacy Risk Management](risk-management-policies.md).

## <a name="get-started-with-subject-rights-requests"></a>Comenzar con solicitudes de derechos del sujeto

Solicitudes de los interesados Priva automatiza el proceso de cumplimiento de solicitudes de derechos del interesado, lo que proporciona un fácil acceso a los datos y flujos de trabajo personalizables que encajan en los procesos empresariales existentes. Puede encontrar fácilmente los datos pertinentes, revisar los resultados y generar informes. En el camino, puede colaborar de forma segura con otros expertos de su organización para completar la solicitud de derechos del sujeto. También puede administrar y personalizar los flujos de trabajo empresariales con plantillas integradas. Para más información sobre el uso de estas características, consulte [Más información sobre Solicitudes de los interesados Priva](subject-rights-requests.md).

## <a name="priva-availability"></a>disponibilidad de Priva

Microsoft Priva está disponible para clientes de todo el mundo. Si su organización aprovisionó su inquilino en uno de los centros de datos locales que se enumeran a continuación para cumplir los requisitos de residencia de datos, las soluciones de Priva no estarán disponibles en el panel de navegación izquierdo del portal de cumplimiento Microsoft Purview:

- Noruega
- Polonia
- Catar
- Singapur
- Sudáfrica
- Corea del Sur
- España
- Suecia
- Suiza
- Emiratos Árabes Unidos

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legal

[Microsoft Priva declinación de responsabilidades legal](priva-disclaimer.md)
