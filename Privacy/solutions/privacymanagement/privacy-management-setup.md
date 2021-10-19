---
title: Introducción a la administración de privacidad
f1.keywords:
- CSH
ms.author: v-jgriffee
author: jmgriffee
manager: laurawi
audience: Admin
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: medium
ms.collection:
- M365-security-compliance
- M365-privacy-management
search.appverid:
- MOE150
- MET150fcf
description: Obtenga información sobre cómo configurar la administración de privacidad para su organización, establecer roles y permisos y configurar opciones importantes.
ms.openlocfilehash: 0f64c581fbeb13726ee9ca2a0f695a5d4f55eb97
ms.sourcegitcommit: 85e085eb17af8b4efd1f45207445e1b3c3679600
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/19/2021
ms.locfileid: "60478322"
---
# <a name="get-started-with-privacy-management"></a>Introducción a la administración de privacidad

Si está listo para empezar a usar la administración de privacidad de Microsoft para obtener ayuda para identificar y mitigar los riesgos de privacidad, siga estos pasos para configurar los requisitos previos y empezar a explorar los conocimientos de privacidad.

## <a name="step-1-confirm-subscriptions-and-licensing"></a>Paso 1: Confirmar suscripciones y licencias

La administración de privacidad está disponible en [el Centro de cumplimiento de Microsoft 365](https://compliance.microsoft.com/) y las organizaciones pueden adquirirla con las siguientes licencias:

- Microsoft 365 E3, E5, A3, A5
- Office 365 E1, E3, E5, A1, A3, A5

La administración de privacidad ofrece opciones de licencias para dos módulos diferentes de la solución: solicitudes de riesgos y derechos de sujeto. Estos se pueden comprar individualmente o juntos. Al obtener licencias para solicitudes de derechos de sujeto, puede elegir el nivel de licencia adecuado para el número de solicitudes que necesita controlar. Puedes comprar solicitudes adicionales en cualquier momento.

Para una guía detallada sobre las licencias, vea: [Guía de licencias de Microsoft 365 para la seguridad y el cumplimiento](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-tenantlevel-services-licensing-guidance/microsoft-365-security-compliance-licensing-guidance#privacy-management).

> [!Note]
> La administración de privacidad no está disponible para los Community (GCC) moderados, GCC altos o del Departamento de Defensa (DoD).

### <a name="get-free-trial-license"></a>Obtener licencia de prueba gratuita

Hay una licencia de prueba gratuita disponible para empezar a usar la administración de privacidad. Para obtener más información sobre la elegibilidad y cómo unirse, consulte [Learn about the free privacy management trial](privacy-management-trial.md).

## <a name="step-2-enable-the-microsoft-365-audit-log"></a>Paso 2: Habilitar el registro Microsoft 365 auditoría

Microsoft 365 registros de auditoría son un resumen de todas las actividades dentro de la organización. Las directivas de administración de privacidad pueden usar estas actividades para generar información sobre directivas.

Es posible que su organización ya tenga los registros de auditoría activados. Si necesita empezar a usarlos por primera vez, vea [Activar](/microsoft-365/compliance/turn-audit-log-search-on-or-off) o desactivar la búsqueda del registro de auditoría para obtener instrucciones paso a paso para activar la auditoría. Después de activar la auditoría, se muestra un mensaje que dice que el registro de auditoría se está preparando y que puede ejecutar una búsqueda en un par de horas después de que se complete la preparación. Solo tiene que realizar esta acción una vez. Para obtener más información acerca del uso del Microsoft 365 de auditoría, vea [Buscar en el registro de auditoría](/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).

## <a name="step-3-set-user-permissions-and-assign-roles"></a>Paso 3: Establecer permisos de usuario y asignar roles

La administración de privacidad usa un modelo de permisos de control de acceso basado en roles (RBAC). Solo los usuarios a los que se asigna un rol pueden acceder a la administración de privacidad y las acciones permitidas por cada usuario están restringidas por tipo de función.

El administrador global tiene permisos para acceder a la administración de privacidad y asignar otros usuarios a roles. Pueden iniciar sesión y establecer permisos de usuario en [el](https://compliance.microsoft.com/) Centro de cumplimiento de Microsoft 365 administración de privacidad. Para un inicio rápido, el grupo de roles De administración de privacidad tiene permisos para tener acceso a todas las características de la administración de privacidad. Este grupo puede ser un buen ajuste para las organizaciones donde la misma persona puede realizar todas las tareas dentro de la solución de administración de privacidad. Otros roles de privacidad le permiten tomar un control más detallado y asignar usuarios a funciones o características seleccionadas.

Para obtener más información sobre los grupos de roles y cómo conceder acceso, vea [Set user permissions and assign roles](privacy-management-permissions.md).

## <a name="step-4-start-finding-and-visualizing-your-data"></a>Paso 4: Empezar a buscar y visualizar los datos

Después de iniciar sesión en la administración de privacidad, verá la página **Información** general. Esta página proporciona información dinámica sobre cómo evolucionan los datos personales en su entorno de Microsoft 365 para ayudarle a detectar rápidamente problemas, identificar indicadores de riesgo y tomar medidas para solucionar problemas. Su información general debe rellenarse con información inicial en las primeras 24 horas de registrarse. A medida que siga usando la administración de privacidad, la página de información general se actualizará para continuar con la información actual.

Para obtener más información sobre los  datos a lo largo del tiempo, la página perfil de datos proporcionará más visualizaciones y análisis y le proporcionará una vista holística de los datos de su organización por ubicación geográfica y por ubicación Microsoft 365 datos.

Para obtener más información sobre estas páginas, vea [Buscar y visualizar los datos](privacy-management-data-profile.md).

## <a name="step-5-start-managing-risks-with-default-policies"></a>Paso 5: Empezar a administrar riesgos con directivas predeterminadas

La administración de privacidad empezará a evaluar los datos y le dará una mirada a los escenarios de riesgo clave para la minimización de datos, la sobreexposición de datos y las transferencias de datos. Estas directivas están activadas de forma predeterminada. Puede usar estas directivas para evaluar dónde están sus riesgos y, a continuación, activar las notificaciones de correo electrónico de los usuarios para que los usuarios les presten atención y orientar la corrección de estos riesgos. Además, puede crear y personalizar sus propias directivas a partir de las plantillas de directiva proporcionadas. Puede adaptar sus directivas para satisfacer las necesidades legales y de cumplimiento normativo de su organización, tal como se puede identificar en consulta con el asesor jurídico. Para obtener más información, vea [Manage privacy risks with policies in privacy management](privacy-management-policies.md).

## <a name="step-6-get-started-with-subject-rights-requests"></a>Paso 6: Introducción a las solicitudes de derechos de sujeto

La administración de privacidad automatiza el proceso de cumplimiento de solicitudes de derechos del sujeto con un fácil acceso a los datos y flujos de trabajo personalizables que se ajustan a los procesos empresariales existentes. Puede encontrar fácilmente los datos relevantes, revisar los resultados y producir informes. En el camino, puede colaborar de forma segura con otros expertos de su organización para completar la solicitud de derechos del sujeto. También puede administrar y personalizar los flujos de trabajo de su empresa con plantillas integradas. Para obtener más información sobre el uso de estas características, vea [Manage subject rights requests](privacy-management-subject-rights-requests.md).

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legales

[Declinación de responsabilidades legales de administración de privacidad](privacy-management-disclaimer.md)
