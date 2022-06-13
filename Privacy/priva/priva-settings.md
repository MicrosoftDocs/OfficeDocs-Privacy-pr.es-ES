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
description: Obtenga información sobre las opciones de configuración global para Microsoft Priva.
ms.openlocfilehash: a6f2fe55600d6cc3018c9d15f05a6d9e459a1486
ms.sourcegitcommit: 3c83e8133a5a71f4e1d76a0b2981ab3ec9cd6602
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/13/2022
ms.locfileid: "66046604"
---
# <a name="configure-priva-settings"></a>Opciones de configuración en Priva

Puede administrar la configuración de Microsoft Priva seleccionando el icono de engranaje en la esquina superior derecha de la pantalla. Las opciones aquí le permiten establecer preferencias de alto nivel y personalizar las propiedades clave. En esta página se proporciona información general sobre las principales categorías de Configuración.

## <a name="anonymization"></a>Anonimización

Puede mostrar versiones anonimizadas de nombres de usuario dentro de las características de Privacy Risk Management a los usuarios de determinados roles. La característica de anonimización reemplaza los nombres para mostrar identificables por una etiqueta genérica con el fin de ayudar a enmascarar las identidades de los usuarios al revisar la información confidencial. Esta opción no se aplica a la solución Solicitudes de derechos del firmante.

## <a name="user-notification-emails"></a>Correos electrónicos de notificación de usuario  

Las directivas de Privacy Risk Management le permiten establecer parámetros para evaluar posibles riesgos de privacidad en su entorno. Cuando se detecta una coincidencia de directiva, Privacy Risk Management puede enviar un correo electrónico a los usuarios con recomendaciones sobre las acciones correctivas que se deben realizar y un vínculo al entrenamiento de privacidad. En **Configuración**, puede habilitar o deshabilitar la funcionalidad de notificación por correo electrónico de Privacy Risk Management en su conjunto. Si la funcionalidad de notificación está desactivada en Configuración, se deshabilitarán todos los correos electrónicos. Para más información sobre las directivas, consulte [Creación de directivas en Privacy Risk Management](risk-management-policies.md).

## <a name="teams-collaboration"></a>Colaboración de Teams  

Integre las funcionalidades de Microsoft Teams con Solicitudes de los interesados Priva para mejorar la colaboración con las partes interesadas. Al activar la casilla **Activar las capacidades de Microsoft Teams para las solicitudes de derechos de sujeto,** se creará automáticamente un canal de Teams asociado para cada solicitud. Los usuarios se pueden agregar al canal de Teams desde la pestaña **Colaboradores** de la solicitud.

Al activar esta característica, se aplicarán funcionalidades de Teams a todas las solicitudes. Al desactivar la casilla, se desactivarán estas funcionalidades para todas las solicitudes. Obtenga más información sobre [la colaboración durante el proceso de revisión de datos](subject-rights-requests-data-review.md#collaboration-for-data-review).

## <a name="data-matching"></a>Coincidencia de datos  

Use esta sección para cargar esquemas de datos que describen los atributos de los interesados, lo que ayudará a identificar al interesado correcto al buscar datos personales dentro de su entorno de Microsoft 365. Los esquemas y paquetes de reglas se crean y cargan en formato XML. En **Carga de datos personales**, también puede enviar datos personales que coincidan con un esquema proporcionado. Puede crear y cargar su propio archivo o elegir cargar datos personales de Azure. Obtenga más información sobre la [coincidencia de datos para solicitudes de derechos del interesado](subject-rights-requests-data-match.md).

## <a name="data-retention-periods"></a>Períodos de retención de datos

Esta configuración está relacionada con Solicitudes de los interesados Priva. Le permite controlar sus preferencias durante cuánto tiempo desea conservar los datos e informes recopilados generados después de cerrar la solicitud. Esto se puede establecer en 30 o 90 días y se aplica a todas las solicitudes de derechos de sujeto que cree. Se recomienda comprobar que los períodos de retención de datos cumplen con las directivas y obligaciones legales de su organización. Obtenga más información sobre la [retención de datos para solicitudes de derechos del interesado](subject-rights-requests-reports.md#retention-periods-for-reports-and-data).

## <a name="data-review-tags"></a>Etiquetas de revisión de datos

Las etiquetas de revisión de datos se pueden usar para marcar los elementos de contenido que se recuperan en una solicitud de derechos del interesado. Esta área de configuración le permite administrar las etiquetas. Priva proporciona tres etiquetas predeterminadas: **Seguimiento**, **Eliminar** y **Actualizar**. Estos nombres de etiquetas no se pueden editar, pero puede proporcionar una descripción para estas etiquetas que sea significativa para su organización.

Priva también proporciona dos etiquetas personalizadas que puede denominar y definir para el uso de su organización. Verá que aparecen como **Etiqueta personalizada 1** y **Etiqueta personalizada 2** hasta que edite los nombres.

Siga los pasos siguientes para editar nombres y descripciones de etiquetas:

- En la página **Configuración Priva**, seleccione **Etiquetas de revisión de datos**.
- Busque la etiqueta en la lista que desea editar y seleccione el icono **Editar** lápiz junto a su nombre.
- En el panel flotante, realice las modificaciones en los campos disponibles. En el caso de las etiquetas del sistema, solo puede editar la descripción. Para las etiquetas personalizadas, puede editar el nombre y la descripción.
- Cuando haya terminado, seleccione **Enviar** para guardar los cambios.

La configuración de etiquetas se aplica a todas las solicitudes de derechos del sujeto.

Obtenga más información sobre [cómo aplicar etiquetas al revisar los datos de una solicitud de derechos del interesado](subject-rights-requests-data-review.md#apply-tags).