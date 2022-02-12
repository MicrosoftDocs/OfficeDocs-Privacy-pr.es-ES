---
title: Opciones de configuración en Priva
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
description: Obtenga información sobre las opciones de configuración global de Microsoft Priva.
ms.openlocfilehash: 9b59dcd875f248dd4a15be47d2f4383e8f656155
ms.sourcegitcommit: 1f3f2757f456628ec904bc3df985b00ffba8f892
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 02/11/2022
ms.locfileid: "62542828"
---
# <a name="configure-priva-settings"></a>Opciones de configuración en Priva

Puedes administrar la configuración de Microsoft Priva seleccionando el icono de engranaje en la esquina superior derecha de la pantalla. Las opciones aquí le permiten establecer preferencias de alto nivel y personalizar las propiedades clave. En esta página se proporciona información general sobre las Configuración categorías principales.

## <a name="anonymization"></a>Anonimización

Esta característica permite mostrar versiones anonimizadas de nombres de usuario dentro de las características de administración de riesgos de privacidad a los usuarios en determinados roles. Reemplazará los nombres para mostrar identificables por una etiqueta genérica con el fin de ayudar a enmascarar las identidades de los usuarios al revisar los datos confidenciales. Esta opción no se aplica a la solución Solicitudes de derechos del sujeto.

## <a name="user-notification-emails"></a>Mensajes de correo electrónico de notificación de usuario  

Las directivas de administración de riesgos de privacidad permiten establecer parámetros para evaluar posibles riesgos de privacidad en su entorno. Cuando detectamos una coincidencia de directiva, la Administración de riesgos de privacidad puede enviar un correo electrónico a los usuarios con recomendaciones sobre las acciones correctivas que se deben tomar y un vínculo a la formación en privacidad. En Configuración, puede habilitar o deshabilitar la funcionalidad de notificación de correo electrónico de la Administración de riesgos de privacidad en su conjunto. Si la funcionalidad de notificación está desactivada en Configuración, se deshabilitarán todos los correos electrónicos. Para obtener más información acerca de las directivas, consulte [Create policies in Privacy Risk Management](risk-management-policies.md).

## <a name="teams-collaboration"></a>Colaboración de Teams  

Integre Microsoft Teams con solicitudes de derechos de sujeto priva para mejorar la colaboración con las partes interesadas. Cada vez que se crea una solicitud de derechos de sujeto, se crea un equipo asociado en Teams. Los usuarios se pueden agregar a un equipo desde la pestaña Colaboradores de la solicitud. Para obtener más información acerca de las solicitudes de derechos de sujeto, vea [Información sobre solicitudes](subject-rights-requests.md) de derechos de sujeto priva.

## <a name="data-matching"></a>Coincidencia de datos  

Use esta sección para cargar esquemas de datos que describen los atributos de los interesados, lo que le ayudará a identificar al interesado correcto al buscar datos personales en su entorno Microsoft 365 datos. Los esquemas y paquetes de reglas se crean y cargan en formato XML. En **Carga de datos personales**, también puede enviar datos personales que coincidan con un esquema proporcionado. Puede crear y cargar su propio archivo o elegir cargar datos personales de Azure. Para obtener más información acerca de las solicitudes de derechos de sujeto, vea [Información sobre solicitudes](subject-rights-requests.md) de derechos de sujeto priva.

## <a name="data-retention-periods"></a>Períodos de retención de datos

Esta configuración está relacionada con solicitudes de derechos de sujeto priva. Le permite controlar su preferencia durante cuánto tiempo desea conservar los datos recopilados y los informes generados después de cerrar la solicitud. Se puede establecer en 30 o 90 días y se aplica a todas las solicitudes de derechos de sujeto que cree. Se recomienda comprobar que los períodos de retención de datos cumplen con las directivas y las obligaciones legales de la organización. Obtenga más información sobre [cómo establecer la retención de datos para solicitudes de derechos de sujeto](subject-rights-requests-reports.md#manage-data-retention).

## <a name="data-review-tags"></a>Etiquetas de revisión de datos

Administre las etiquetas que usará para marcar los archivos recuperados en una solicitud de derechos de sujeto. Estas etiquetas se pueden usar para indicar el contenido que necesitará más atención, como el contenido que podría necesitar eliminarse manualmente. En esta sección de configuración, puede editar los nombres y descripciones de las etiquetas personalizadas. También puede editar las descripciones de etiquetas de las etiquetas integradas proporcionadas por el sistema. Los nombres de las etiquetas del sistema no se pueden cambiar. Para obtener más información acerca de las solicitudes de derechos del sujeto, vea [Revisar los datos de una solicitud de derechos de sujeto](subject-rights-requests-data-review.md#step-3-review-data).
