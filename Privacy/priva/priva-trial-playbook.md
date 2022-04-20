---
title: 'Cuaderno de estrategias de prueba: Microsoft Priva'
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
- MET150
description: Obtenga información sobre la evaluación de Microsoft Priva, consulte las acciones recomendadas que debe realizar durante el período de prueba y revise los vínculos a documentación importante.
ms.openlocfilehash: 567901cf75440b76fc5c3b755894cada188d6505
ms.sourcegitcommit: 09ecdaded9a9f8f79587f2acb978dc53b83e5c01
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/19/2022
ms.locfileid: "64930531"
---
# <a name="trial-playbook-microsoft-priva"></a>Cuaderno de estrategias de prueba: Microsoft Priva

Bienvenido al cuaderno de estrategias de prueba de Microsoft Priva.

Este cuaderno de estrategias le ayudará a sacar el máximo partido a su evaluación gratuita de 90 días, ya que le ayudará a proteger sus datos personales y a crear un área de trabajo resistente a la privacidad.

Con las recomendaciones de Microsoft, aprenderá cómo Priva puede ayudarle a identificar y proteger de forma proactiva los riesgos de privacidad, como la acumulación de datos, las transferencias de datos y el uso compartido excesivo de datos, ayudar a su organización a automatizar y administrar solicitudes de sujetos a escala y capacitar a los empleados para tomar decisiones inteligentes sobre el control de datos.

## <a name="getting-started"></a>Introducción

*Estas acciones son recomendaciones sobre características clave para probar en la versión de prueba de 90 días.*

Inicie la prueba mediante la configuración de los requisitos previos. Tenga en cuenta que Priva consta de dos soluciones clave, Priva Privacy Risk Management y Priva Subject Rights Requests, que se pueden probar y comprar por separado. Los detalles de licencias y compras se pueden encontrar en [Microsoft.com](https://www.microsoft.com/security/business/privacy/privacy-management-software?rtc=1#office-ContentAreaHeadingTemplate-8x0pmkp).

### <a name="privacy-risk-management"></a>Administración de riesgos de privacidad

Con la solución **Privacy Risk Management** , puede explorar cómo proteger los datos personales de su organización y crear un área de trabajo resistente a la privacidad.

- Identificar y proteger de forma proactiva frente a riesgos de privacidad, como la acumulación de datos, las transferencias de datos y el uso compartido excesivo de datos
- Obtener visibilidad sobre el almacenamiento y el movimiento de datos personales
- Capacitar a los trabajadores de la información para tomar decisiones inteligentes sobre el control de estos datos
- Permitir a los usuarios administrar datos de forma eficaz y tomar medidas para cumplir con las regulaciones de privacidad en constante evolución

### <a name="subject-rights-requests"></a>Solicitudes de derechos del interesado

Con la solución **Solicitudes de derechos del firmante** , puede aprender a controlar las consultas desde la solicitud inicial hasta la generación de informes.

- Administración de solicitudes de derechos de sujeto a escala

## <a name="start-your-microsoft-priva-trial"></a>Inicio de la prueba de Microsoft Priva

Si está listo para empezar a usar Microsoft Priva, siga estos pasos para configurar los requisitos previos y empezar a explorar la información de privacidad.

1. [Confirmación de suscripciones y licencias](priva-setup.md#step-1-confirm-subscriptions-and-licensing)
1. [Establecimiento de permisos de usuario y asignación de roles](priva-setup.md#step-3-set-user-permissions-and-assign-roles)
1. Seleccione "Iniciar prueba" y lo siguiente se realizará automáticamente:
    - Las licencias de prueba priva están habilitadas (esto sucede en tiempo real)
    - Se generan conclusiones de privacidad (esto tarda 24 horas)

![Captura de pantalla de la pantalla de bienvenida.](../media/priva-insights.png)

## <a name="start-finding-and-visualizing-privacy-risks"></a>Empezar a buscar y visualizar riesgos de privacidad

Priva le ayuda a comprender los datos que almacena su organización mediante la automatización de la detección de recursos de datos personales y la visualización de información esencial.

Para empezar, vaya a la sección Priva del [portal de cumplimiento de Microsoft Purview](https://compliance.microsoft.com/) y vea estas páginas:

1. [Información general](priva-data-profile.md#explore-the-overview-page): proporciona una vista agregada de la posición de privacidad, incluido el volumen, la categoría, la ubicación y el movimiento de datos personales en el entorno de Microsoft 365. Además, obtendrá visibilidad sobre el estado actual y las tendencias de los riesgos de privacidad asociados derivados de que los datos personales se compartan, transfieran o no se usen en exceso.
1. [Perfil de datos](priva-data-profile.md#explore-the-data-profile-page): proporciona una instantánea de los datos personales que la organización almacena en Microsoft 365, incluidos el volumen, el tipo y la ubicación (almacenamiento y geografía).

## <a name="learn-about-policies"></a>Más información sobre las directivas

Privacy Risk Management le ofrece la capacidad de configurar directivas que identifiquen los riesgos de privacidad en su entorno de Microsoft 365 y permitan una fácil corrección.

1. [Más información sobre los escenarios de riesgo clave](risk-management.md#learn-about-key-risk-scenarios)
1. [Limitación de la sobreexposición de datos](risk-management.md#limit-data-overexposure)
1. [Búsqueda y mitigación de transferencias de datos](risk-management.md#find-and-mitigate-data-transfers)
1. [Minimizar los datos almacenados](risk-management.md#minimize-stored-data)

![Captura de pantalla de la página de directivas principal.](../media/priva-policies-page.png)

## <a name="create-and-customize-policies"></a>Crear y personalizar directivas

Cree nuevas directivas en Privacy Risk Management para abordar los escenarios de riesgo de privacidad importantes para su organización. Para un inicio rápido, use las plantillas predeterminadas para crear nuevas directivas para la sobreexposición de datos, las transferencias de datos y la minimización de datos y escenarios.

1. [Creación de una directiva a partir de una plantilla](risk-management-policies.md#create-a-policy-from-a-template)
1. [Crear una directiva personalizada](risk-management-policies.md#create-a-custom-policy)
1. [Más información sobre la configuración de claves para todas las directivas](risk-management-policies.md#learn-about-key-settings-for-all-policies)
1. [Más información sobre la configuración de las directivas de minimización de datos](risk-management-policies.md#learn-about-settings-for-data-minimization-policies)
1. [Más información sobre la configuración de las directivas de transferencia de datos](risk-management-policies.md#learn-about-settings-for-data-transfer-policies)
1. [Más información sobre la configuración de las directivas de sobreexposición de datos](risk-management-policies.md#learn-about-settings-for-data-overexposure-policies)

## <a name="manage-policies"></a>Administrar directivas

Una vez que haya creado directivas en Privacy Risk Management para controlar escenarios de minimización de datos, transferencia de datos o sobreexposición de datos, es posible que desee revisar o actualizar la configuración de la directiva. También puede probar una nueva directiva antes de implementarla completamente para su uso continuo.

1. [Visualización de los detalles de la directiva](risk-management-policies-manage.md#view-policy-details)
1. [Prueba de la directiva](risk-management-policies-manage.md#test-your-policy)
1. [Eliminar una directiva](risk-management-policies-manage.md#delete-a-policy)

## <a name="understand-policy-alerts-and-issues"></a>Descripción de las alertas y problemas de directivas

La revisión de alertas le permite identificar casos que necesitan seguimiento. Para ello, cree problemas que proporcionen a los usuarios una manera estructurada de revisar el contenido, asignar la gravedad del problema y trabajar de forma colaborativa para corregir los problemas.

1. [Visualización de alertas y problemas actuales](risk-management-alerts.md#view-current-alerts-and-issues)
1. [Administrar alertas](risk-management-alerts.md#manage-alerts)
1. [Administrar problemas](risk-management-alerts.md#manage-issues)
1. [Revisión del contenido y corrección de problemas](risk-management-alerts.md#review-content-and-remediate-issues)

## <a name="send-users-policy-notifications"></a>Enviar notificaciones de directiva a usuarios

Privacy Risk Management puede notificar directamente a los propietarios de contenido las coincidencias de las directivas de sobreexposición, minimización de datos y transferencia de datos. Con las notificaciones por correo electrónico, los usuarios pueden averiguar fácilmente el contenido que necesitan revisar.

1. [Preparación del contenido de entrenamiento para notificaciones de directivas](risk-management-notifications.md#prepare-training-content-for-policy-notifications)
1. [Configuración de notificaciones por correo electrónico para directivas](risk-management-notifications.md#set-up-email-notifications-for-policies)
1. [Corrección de problemas de las notificaciones por correo electrónico](risk-management-notifications.md#remediate-issues-from-email-notifications)
1. [Envío de notificaciones en Teams](risk-management-notifications.md#send-notifications-in-teams)

## <a name="learn-about-subject-rights-requests"></a>Información acerca de las solicitudes de derechos del interesado

De acuerdo con ciertas regulaciones de privacidad en todo el mundo, las personas (o los interesados) pueden hacer solicitudes para revisar o administrar los datos personales sobre sí mismos que las empresas han recopilado. Estas solicitudes también se conocen como solicitudes de derechos del interesado (DSR), solicitudes de acceso a datos del interesado (DSARs) o solicitudes de derechos del consumidor. Priva Subject Rights Requests puede ayudarle a controlar estas consultas.

1. [Creación de solicitudes y recopilación de datos](subject-rights-requests-create.md)
1. [Coincidencia de datos](subject-rights-requests-data-match.md)
1. [Revisión de datos y colaboración en solicitudes](subject-rights-requests-data-review.md)
1. [Satisfacer solicitudes](subject-rights-requests-reports.md)
1. [Automatizar tareas](subject-rights-requests-automate.md)

![Flujo de trabajo para solicitudes de derechos de sujeto.](../media/priva-srr-cycle.png)

## <a name="create-subject-rights-requests"></a>Crear solicitudes de derechos del interesado

Los administradores de administración de derechos del sujeto pueden abrir nuevas solicitudes de derechos de sujeto a través de la página principal solicitudes de derechos del sujeto. Un asistente le guiará a través del proceso de búsqueda de datos personales sobre un interesado e iniciar el proceso de satisfacer su solicitud.

1. [Uso del Asistente para solicitudes de derechos del firmante](subject-rights-requests-create.md#use-the-subject-rights-request-creation-wizard) : creación de una solicitud
1. [Definición de la configuración de búsqueda](subject-rights-requests-create.md#define-search-settings)
1. [Refinar la configuración de búsqueda](subject-rights-requests-create.md#refine-your-search)

## <a name="manage-data-matching-for-subject-rights-requests"></a>Administración de la coincidencia de datos para solicitudes de derechos del interesado

Con la coincidencia de datos, las organizaciones pueden permitir que Priva identifique a los interesados en función de los valores de datos proporcionados exactamente.

1. [Preparación para la importación de datos](subject-rights-requests-data-match.md#prepare-for-data-import)
1. [Definición del esquema de datos personales](subject-rights-requests-data-match.md#define-the-personal-data-schema)
1. [Upload datos personales](subject-rights-requests-data-match.md#upload-personal-data)

## <a name="review-data-and-collaborate-on-subject-rights-requests"></a>Revisar datos y colaborar en solicitudes de derechos del interesado

Después de crear una solicitud de derechos de sujeto, Priva usará sus entradas sobre el sujeto para buscar coincidencias en el entorno de Microsoft 365 de la organización. Una vez compilados estos datos, puede revisar los resultados, tomar decisiones sobre qué incluir y redactar la información según sea necesario.

1. [Revisar los detalles de la solicitud y supervisar el progreso](subject-rights-requests-data-review.md#step-1-review-request-details-and-monitor-progress)
1. [Visualización y edición de consultas de búsqueda](subject-rights-requests-data-review.md#step-2-optional-view-and-edit-search-queries)  (opcional)
1. [Revisar datos](subject-rights-requests-data-review.md#step-3-review-data)
1. [Cerrar la solicitud](subject-rights-requests-data-review.md#step-4-close-the-request)

## <a name="manage-subject-rights-requests-reports-and-fulfill-requests"></a>Administrar informes de solicitudes de derechos del interesado y completar solicitudes

Después de completar la revisión de datos para una solicitud de derechos del interesado, puede pasar a solicitar el cumplimiento.

1. [Preparación de informes finales para el interesado](subject-rights-requests-reports.md)
1. [Integración con soluciones de asociados](subject-rights-requests-reports.md#integrate-with-partner-solutions)
1. [Administración de la retención de datos](subject-rights-requests-reports.md#retention-periods-for-reports-and-data)

## <a name="automate-subject-rights-requests-tasks"></a>Automatizar tareas de solicitudes de derechos del interesado

Habilite Power Automate flujos para Priva para automatizar tareas importantes para casos y usuarios, como la creación de vales en ServiceNow o la adición de recordatorios de calendario sobre fechas de vencimiento.

1. [Creación de un nuevo flujo de Power Automate a partir de una plantilla](subject-rights-requests-automate.md#create-a-new-power-automate-flow-from-a-template)
1. [Compartir un flujo de Power Automate](subject-rights-requests-automate.md#share-a-power-automate-flow)
1. [Editar o eliminar Power Automate flujo](subject-rights-requests-automate.md#edit-or-delete-power-automate-flow)

## <a name="additional-resources"></a>Recursos adicionales

**Microsoft Docs**: obtenga información detallada sobre cómo funciona Microsoft Priva y cómo implementarla mejor para su organización. [Visite Docs](priva-overview.md).

**Por qué Microsoft Priva**: obtenga más información sobre las funcionalidades de Priva en este [vídeo](https://www.youtube.com/watch?v=6OLky1biPIQ).

**Obtenga más información sobre Microsoft Priva**: blogs, planes, precios [aquí](https://aka.ms/privacymgmt/web).

**Comprar Microsoft Priva**: la administración de riesgos de privacidad y las solicitudes de derechos del sujeto se venden por separado. Los detalles de licencias y compras se pueden encontrar en [Microsoft.com](https://www.microsoft.com/en-us/security/business/privacy/privacy-management-software?rtc=1#office-ContentAreaHeadingTemplate-8x0pmkp).
