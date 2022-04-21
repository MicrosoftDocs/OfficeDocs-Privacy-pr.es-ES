---
title: Directivas de minimización de datos en Privacy Risk Management
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
description: Obtenga información sobre cómo crear una directiva de minimización de datos en Microsoft Priva Privacy Risk Management para reducir la cantidad de datos personales no utilizados en su organización.
ms.openlocfilehash: c5a883de696923e4453ed28739e9bf68b618f8d1
ms.sourcegitcommit: b5f7dcb73c0e3f677981e80106769cb546d00af4
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/21/2022
ms.locfileid: "65014489"
---
# <a name="data-minimization-policies-in-privacy-risk-management"></a>Directivas de minimización de datos en Privacy Risk Management

Las directivas de minimización de datos se centran en la antigüedad del contenido y en cuánto tiempo ha pasado desde que se modificó por última vez. La supervisión de los datos personales que todavía se conservan en contenido antiguo sin usar puede ayudarle a administrar mejor los datos almacenados y a reducir los riesgos.

Privacy Risk Management le permite crear directivas para supervisar los datos que no se han modificado dentro de un período de tiempo que seleccione. Cuando se detecta una coincidencia de directiva, puede enviar notificaciones por correo electrónico a los usuarios con opciones de corrección que incluyen marcar elementos para su eliminación, notificar a los propietarios de contenido o etiquetar elementos para una revisión posterior.

Nuestro proceso de configuración de directivas facilita el establecimiento de condiciones de directiva. Tiene control total sobre el tiempo de las alertas y la frecuencia de los correos electrónicos que atraen la atención de los usuarios sobre las prácticas de control de datos seguras.

Hay dos maneras de crear una directiva: a partir de una **plantilla**, que es nuestra rápida opción "lista para usar" mediante la configuración predeterminada; o la opción **personalizada** , que es un proceso guiado para establecer condiciones, alertas y notificaciones.

## <a name="quick-setup-use-a-template-with-default-settings"></a>Configuración rápida: usar una plantilla con la configuración predeterminada

La directiva de minimización de datos predeterminada detecta el contenido que contiene datos personales que se crearon o modificaron hace al menos 30 días.

Siga estos pasos para crear una directiva de transferencia de datos predeterminada:

1. En el [Centro de cumplimiento de Microsoft 365](https://compliance.microsoft.com/), busque Priva Privacy Risk Management en el panel de navegación izquierdo y seleccione **Directivas**.

2. Seleccione **Crear una directiva** en la esquina superior derecha de la pantalla, que muestra un panel flotante que enumera todas las opciones de creación de directivas.

3. En el cuadro **Minimización de datos** , seleccione **Crear**.

4. Un panel flotante contiene detalles de directiva. Al seleccionar **Ver configuración** , se mostrarán los valores predeterminados. Puede editar la configuración desde aquí, lo que le lleva al proceso guiado que se describe a continuación. Para seguir creando la directiva con la configuración predeterminada, simplemente escriba un nombre descriptivo y, a continuación, seleccione **Crear directiva**.

La directiva se creará y la encontrará en la página **Policías** . Comienza en [modo de prueba](risk-management-policies.md#testing-a-policy) para que pueda supervisar cómo funciona antes de activarlo.

#### <a name="default-data-minimization-policy-settings"></a>Configuración predeterminada de la directiva de minimización de datos

Una directiva de minimización de datos creada a partir de la plantilla detectará:
- Elementos de contenido que contienen datos personales que no se han modificado en al menos los últimos 30 días.
- Datos almacenados en cualquiera de estas ubicaciones de la organización: Exchange, OneDrive, SharePoint, Teams.
- Tipos de datos basados en los siguientes [grupos de clasificación](risk-management-policies.md#classification-groups):
    - Reglamento general de protección de datos (RGPD) de la UE
    - Información de identificación personal de EE. UU.
    - Ley Patriota de EE. UU.
    - Ley de notificación de infracción de estado de EE. UU.
    - Ley Gramm-Leach-Bliley de EE. UU. (GLBA)
    - Ley de portabilidad y responsabilidad de seguros de salud de EE. UU. (HIPAA)
    - Ley de registros de salud de Australia (HRIP)
    - Ley de privacidad de Australia
    - Información de identificación personal de Japón
    - Protección de información personal de Japón

## <a name="custom-setup-guided-policy-creation-process"></a>Configuración personalizada: proceso de creación de directivas guiada

La opción de directiva personalizada es un proceso guiado para crear una nueva directiva mediante la configuración de condiciones, la designación de la gravedad y la frecuencia de las alertas y la activación de notificaciones por correo electrónico del usuario.

Complete los pasos siguientes para crear una nueva directiva de transferencia de datos:

1. En el [Centro de cumplimiento de Microsoft 365](https://compliance.microsoft.com/), busque Priva Privacy Risk Management en el panel de navegación izquierdo y seleccione **Directivas**.

2. Seleccione el botón **Crear una directiva** en la esquina superior derecha de la pantalla, que muestra un panel flotante que enumera todas las opciones de creación de directivas.

3. En el cuadro **Personalizado** , seleccione **Crear**.

4. En la página **Nombre y tipo** , seleccione la plantilla **Directiva de minimización de datos** . Escriba un nombre de directiva que le ayude a identificarla fácilmente en la lista en la página **Directivas** , escriba una descripción opcional y, a continuación, seleccione **Siguiente**.

5. En la página **Datos que se van a supervisar** , elija el tipo de datos personales que desea que supervise la directiva. Hay dos opciones:
    - **Grupos de clasificación**: agrupaciones de tipos de información confidencial que se usan para detectar contenido relacionado con datos personales o regulaciones específicas. Si selecciona esta opción, deberá seleccionar **+Agregar grupos de clasificación** para elegir uno o varios grupos de la lista proporcionada.
    - **Tipos de información confidencial individuales**: seleccione esta opción para elegir entre una lista de [tipos de información confidencial](/microsoft-365/compliance/sensitive-information-type-entity-definitions) individuales.

    Obtenga más información sobre [cómo elegir los datos que se van a supervisar](risk-management-policies.md#choose-data-to-monitor). Cuando haya terminado de seleccionar los datos que desea supervisar, seleccione **Siguiente**.

6. En la página **Usuarios y grupos** , elija a qué usuarios de su organización se aplicará la directiva. Puede seleccionar todos los usuarios individuales y todos los grupos de distribución Office 365, o puede seleccionar usuarios y grupos específicos. Obtenga más información sobre [cómo elegir usuarios y grupos](risk-management-policies.md#choose-users-and-groups). Cuando haya acabado, seleccione **Siguiente**.

7. En la página **Ubicaciones**, seleccione todas las ubicaciones de datos de Microsoft 365 que desea que la directiva cubra. Elija entre Exchange cuentas de correo electrónico, cuentas de OneDrive, mensajes de chat y canales de Teams y sitios de SharePoint.

    Dentro de SharePoint puede designar todos los sitios o sitios específicos. Si selecciona **Sitios de SharePoint específicos**, puede escribir la dirección URL del sitio en el campo URL. También puede seleccionar **+Elegir sitios** y, en el panel flotante, active la casilla situada a la izquierda del nombre del sitio que desea seleccionar.

    Obtenga más información sobre [cómo elegir ubicaciones](risk-management-policies.md#choose-locations). Cuando haya terminado de seleccionar ubicaciones, seleccione **Siguiente**.

8. En la página **Condiciones** , use el menú desplegable para elegir cuántos días desde que se modificó por última vez un elemento que la directiva detectará:
    - 30 días
    - 60 días
    - 90 días
    - 120 días
    
     Cuando haya acabado, seleccione **Siguiente**.

9. En la página **Resultados** , decida si desea notificar a los usuarios cuando coincidan con las condiciones establecidas por la directiva. Si marca la casilla de notificaciones por correo electrónico, los usuarios recibirán una notificación por correo electrónico cuando sus acciones coincidan con las condiciones de la directiva. Los correos electrónicos contendrán instrucciones para realizar acciones de corrección directamente desde el correo electrónico, junto con un vínculo al entrenamiento de privacidad. Designará la frecuencia de los correos electrónicos y la dirección URL para el entrenamiento de privacidad que prefiera.
     
    Obtenga más información sobre cómo configurar [las notificaciones de usuario](risk-management-notifications.md). Cuando haya terminado de seleccionar resultados, seleccione **Siguiente**.

10. En la página **Alertas** , use el modificador de alternancia para activar las alertas que un administrador verá en la página **Alertas** de la sección **Directivas** de Administración de riesgos de privacidad. Designará la frecuencia con la que se generan las alertas, los umbrales de coincidencias antes de que se generen las alertas y la gravedad de las alertas. Obtenga más información sobre [cómo establecer alertas para coincidencias de directivas](risk-management-policies.md#set-alerts). Cuando haya acabado, seleccione **Siguiente**.

11. En la página **Modo** , decida si desea ejecutar la directiva en modo de prueba cuando la cree por primera vez, lo que significa que no se enviarán alertas ni notificaciones. Para mantener la directiva en modo de prueba, que se recomienda, seleccione el modificador de alternancia en la posición **Activado** . Obtenga más información sobre [cómo probar una directiva](risk-management-policies.md#testing-a-policy).

> [!NOTE]
> Si cambia el modificador **Ejecutar en modo de prueba** a la posición **Desactivado** , *se activará la directiva* cuando haya terminado de crearla. Esto significa que las alertas o notificaciones de usuario que configure comenzarán a generarse una vez que se detecte una coincidencia.

12. En la página **Finalizar** , revise las opciones. Seleccione **Editar** debajo de cualquiera de las secciones para ajustar la configuración. Cuando esté satisfecho con la configuración de la directiva, seleccione **Enviar** para crear la directiva.

Después de unos segundos, verá una confirmación de que se creó la directiva. Seleccione **Listo** en la página de confirmación, que le llevará a la página **Directivas** , donde verá la nueva directiva en la parte superior de la tabla.

## <a name="next-steps"></a>Siguientes pasos

Visite las [directivas de administración de riesgos de privacidad](risk-management-policies.md) para obtener más información sobre cómo editar y administrar directivas.