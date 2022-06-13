---
title: Directivas de transferencia de datos en Privacy Risk Management
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
description: Obtenga información sobre cómo crear una directiva de control de datos en Gestión de riesgos de privacidad Microsoft Priva para detener las transferencias de datos personales dentro o fuera de su organización.
ms.openlocfilehash: eba53580365d1fee387c05a54093ab04e41cd15f
ms.sourcegitcommit: 3c83e8133a5a71f4e1d76a0b2981ab3ec9cd6602
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/13/2022
ms.locfileid: "66046654"
---
# <a name="data-transfer-policies-in-privacy-risk-management"></a>Directivas de transferencia de datos en Privacy Risk Management

## <a name="whats-new"></a>Novedades
Las directivas de transferencia de datos ahora pueden detectar cuándo se transfieren elementos que contienen datos personales fuera de su organización. Las transferencias externas serán el escenario de transferencia predeterminado al crear una nueva directiva de transferencia de datos mediante la [opción de configuración rápida](#quick-setup-use-a-template-with-default-settings). Esto no afectará ni cambiará la configuración de las directivas de transferencia de datos que ya haya creado.

## <a name="overview"></a>Información general

La transferencia de datos personales presenta riesgos, especialmente cuando se transfieren fuera de su organización o se envían entre determinados departamentos o ubicaciones geográficas dentro de la organización. Por ejemplo, si los datos se envían a través de correos electrónicos sin cifrar o a destinatarios no autorizados, es posible que los datos ya no sean seguros. Las actividades de transferencia de datos como estas pueden tener un impacto normativo o pueden infringir las prácticas de privacidad de la organización establecidas.

Las directivas de transferencia de datos de Privacy Risk Management le permiten supervisar las transferencias de datos personales fuera de su organización, así como las transferencias internas entre diferentes departamentos, países o regiones. Cuando se detecta una coincidencia de directiva, puede enviar a los usuarios notificaciones por correo electrónico que les permitan realizar acciones correctivas en el correo electrónico, como hacer que los elementos de contenido sean privados, notificar a los propietarios de contenido o etiquetar elementos para una revisión posterior.

Nuestro proceso de configuración de directivas facilita el establecimiento de condiciones de directiva. Tiene control total sobre el tiempo y la frecuencia de las alertas de los correos electrónicos y sugerencias en el momento en Microsoft Teams que atraen la atención de los usuarios sobre las prácticas de control de datos seguras.

Hay dos maneras de crear una directiva: a partir de una **plantilla**, que es nuestra rápida opción "lista para usar" mediante la configuración predeterminada; o la opción **personalizada** , que es un proceso guiado para establecer condiciones, alertas y notificaciones.

## <a name="quick-setup-use-a-template-with-default-settings"></a>Configuración rápida: usar una plantilla con la configuración predeterminada

La directiva de transferencia de datos predeterminada detecta cuándo se envían datos personales a destinatarios fuera de su organización. Por ejemplo, detecta cuándo un usuario de su organización envía un correo electrónico Exchange a un destinatario externo en los campos **To**, **Cc** o **Bcc**.

Siga estos pasos para crear una directiva de transferencia de datos predeterminada:

1. En el [portal de cumplimiento de Microsoft Purview](https://compliance.microsoft.com/), busque Administración de riesgo de privacidad Priva en el panel de navegación izquierdo y seleccione **Directivas**.

2. Seleccione **Crear una directiva** en la esquina superior derecha de la pantalla, que muestra un panel flotante que enumera todas las opciones de creación de directivas.

3. En el cuadro **Transferencias de datos** , seleccione **Crear**.

4. Un panel flotante contiene detalles de directiva. Al seleccionar **Ver configuración** , se mostrarán los [valores predeterminados](#default-data-transfer-policy-settings). Puede editar la configuración desde aquí, lo que le lleva al proceso guiado que se describe a continuación. Para seguir creando la directiva con la configuración predeterminada, simplemente escriba un nombre descriptivo y, a continuación, seleccione **Crear directiva**.

La directiva se creará y la encontrará en la página **Policías** . Comienza en [modo de prueba](risk-management-policies.md#testing-a-policy) para que pueda supervisar cómo funciona antes de activarlo.

#### <a name="default-data-transfer-policy-settings"></a>Configuración predeterminada de la directiva de transferencia de datos

Una directiva de transferencia de datos creada a partir de la plantilla detectará:
- Cuando los datos personales de su organización se transfieren o comparten con un destinatario o ubicación fuera de la organización.
- Cuando los datos personales se comparten externamente desde cualquiera de estas ubicaciones dentro de la organización:
    - **Exchange**. Ejemplo: enviar un correo electrónico que contiene datos personales a una dirección de correo electrónico de destinatario que está fuera de su organización.
    - **OneDrive** y **SharePoint**. Ejemplos: envío de un vínculo a un archivo o sitio que contiene datos personales a alguien fuera de su organización; copiar o mover un archivo a una ubicación OneDrive o SharePoint que se encuentra fuera de la organización.
    - **Microsoft Teams**. Ejemplo: enviar un Teams mensaje de chat que contiene datos personales a un destinatario que está fuera de su organización.
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

1. En el [portal de cumplimiento de Microsoft Purview](https://compliance.microsoft.com/), busque Administración de riesgo de privacidad Priva en el panel de navegación izquierdo y seleccione **Directivas**.

2. Seleccione el botón **Crear una directiva** en la esquina superior derecha de la pantalla, que muestra un panel flotante que enumera todas las opciones de creación de directivas.

3. En el cuadro **Personalizado** , seleccione **Crear**.

4. En la página **Nombre y tipo** , seleccione la plantilla **Directiva de transferencias de datos** . Escriba un nombre de directiva que le ayude a identificarla fácilmente en la lista en la página **Directivas** , escriba una descripción opcional y, a continuación, seleccione **Siguiente**.

5. En la página **Datos que se van a supervisar** , elija el tipo de datos personales que desea que supervise la directiva. Hay dos opciones:
    - **Grupos de clasificación**: agrupaciones de tipos de información confidencial que se usan para detectar contenido relacionado con datos personales o regulaciones específicas. Si selecciona esta opción, deberá seleccionar **+Agregar grupos de clasificación** para elegir uno o varios grupos de la lista proporcionada.
    - **Tipos de información confidencial individuales**: seleccione esta opción para elegir entre una lista de [tipos de información confidencial](/microsoft-365/compliance/sensitive-information-type-entity-definitions) individuales.

    Obtenga más información sobre [cómo elegir los datos que se van a supervisar](risk-management-policies.md#choose-data-to-monitor). Cuando haya terminado de seleccionar los datos que desea supervisar, seleccione **Siguiente**.

6. En la página **Usuarios y grupos** , elija a qué usuarios de su organización se aplicará la directiva. Puede seleccionar todos los usuarios individuales y todos los grupos de distribución Office 365, o puede seleccionar usuarios y grupos específicos. Obtenga más información sobre [cómo elegir usuarios y grupos](risk-management-policies.md#choose-users-and-groups). Cuando haya acabado, seleccione **Siguiente**.

7. En la página **Ubicaciones**, seleccione todas las ubicaciones de datos de Microsoft 365 que desea que la directiva cubra. Elija entre Exchange cuentas de correo electrónico, cuentas de OneDrive, mensajes de chat y canales de Teams y sitios de SharePoint.

    Dentro de SharePoint puede designar todos los sitios o sitios específicos. Si selecciona **Sitios de SharePoint específicos**, puede escribir la dirección URL del sitio en el campo URL. También puede seleccionar **+Elegir sitios** y, en el panel flotante, active la casilla situada a la izquierda del nombre del sitio que desea seleccionar.

    Obtenga más información sobre [cómo elegir ubicaciones](risk-management-policies.md#choose-locations). Cuando haya terminado de seleccionar ubicaciones, seleccione **Siguiente**.

8. En la página **Condiciones** , seleccione qué tipo de condición de transferencia de datos detectará la directiva:
    - **Transferencias fuera de la organización**: detecta las transferencias de usuarios o grupos dentro de la organización a usuarios externos o invitados fuera de la organización.
    - **Transferencias entre departamentos de la organización**: para esta opción, seleccionará un departamento remitente y un departamento de destinatarios. Elija departamentos en las listas de los paneles de control flotante que aparecen y, a continuación, seleccione **Agregar**.
    - **Transferencias entre límites de país o regiones**: para esta opción, seleccionará una región del remitente y una región de destinatario. Elija los países o regiones designados en los paneles de control flotante que aparecen y, a continuación, seleccione **Agregar**.

9. En la página **Resultados** , decida si desea notificar a los usuarios cuando coincidan con las condiciones establecidas por la directiva. Puede elegir una o ambas opciones, o bien no elegir ninguna si deja las casillas en blanco:
    - **Sugerencias enviar en Microsoft Teams**: las sugerencias de control de datos aparecerán en la instancia de Teams de un usuario cuando haya realizado una acción que coincida con las condiciones de la directiva. Tendrá que agregar una dirección URL para el entrenamiento de privacidad que prefiera, que también aparecerá en la sugerencia.
    - **Notificaciones por correo electrónico**: los usuarios recibirán una notificación por correo electrónico cuando sus acciones coincidan con las condiciones de la directiva. Los correos electrónicos contendrán instrucciones para realizar acciones de corrección directamente desde el correo electrónico, junto con un vínculo al entrenamiento de privacidad. Designará la frecuencia de los correos electrónicos y la dirección URL para el entrenamiento de privacidad que prefiera.
     
    Obtenga más información sobre cómo configurar [las notificaciones de usuario](risk-management-notifications.md). Cuando haya terminado de seleccionar resultados, seleccione **Siguiente**.

10. En la página **Alertas** , use el modificador de alternancia para activar las alertas que un administrador verá en la página **Alertas** de la sección **Directivas** de Administración de riesgos de privacidad. Designará la frecuencia con la que se generan las alertas, los umbrales de coincidencias antes de que se generen las alertas y la gravedad de las alertas. Obtenga más información sobre [cómo establecer alertas para coincidencias de directivas](risk-management-policies.md#set-alerts). Cuando haya acabado, seleccione **Siguiente**.

11. En la página **Modo** , decida si desea ejecutar la directiva en modo de prueba cuando la cree por primera vez, lo que significa que no se enviarán alertas ni notificaciones. Para mantener la directiva en modo de prueba, que se recomienda, seleccione el modificador de alternancia en la posición **Activado** . Obtenga más información sobre [cómo probar una directiva](risk-management-policies.md#testing-a-policy).

> [!NOTE]
> Si cambia el modificador **Ejecutar en modo de prueba** a la posición **Desactivado** , *se activará la directiva* cuando haya terminado de crearla. Esto significa que las alertas o notificaciones de usuario que configure comenzarán a generarse una vez que se detecte una coincidencia.

12. En la página **Finalizar** , revise las opciones. Seleccione **Editar** debajo de cualquiera de las secciones para ajustar la configuración. Cuando esté satisfecho con la configuración de la directiva, seleccione **Enviar** para crear la directiva.

Después de unos segundos, verá una confirmación de que se creó la directiva. Seleccione **Listo** en la página de confirmación, que le llevará a la página **Directivas** , donde verá la nueva directiva en la parte superior de la tabla.

## <a name="next-steps"></a>Pasos siguientes

Visite las [directivas de administración de riesgos de privacidad](risk-management-policies.md) para obtener más información sobre cómo editar y administrar directivas.
