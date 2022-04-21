---
title: Directivas de sobreexposición de datos en Privacy Risk Management
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
description: Obtenga información sobre cómo crear una directiva de sobreexposición de datos en Microsoft Priva Privacy Risk Management para identificar y proteger los datos personales que pueden ser demasiado accesibles.
ms.openlocfilehash: a0c87a84a78206862d9a79e1c16d17a90de5f040
ms.sourcegitcommit: b5f7dcb73c0e3f677981e80106769cb546d00af4
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/21/2022
ms.locfileid: "65014510"
---
# <a name="data-overexposure-policies-in-privacy-risk-management"></a>Directivas de sobreexposición de datos en Privacy Risk Management

Su organización puede almacenar contenido en varios niveles de acceso, incluidas las áreas a las que se puede acceder públicamente y otras que están restringidas. Las directivas de sobreexposición de datos pueden ayudarle a detectar y controlar situaciones en las que los datos almacenados por su organización no son suficientemente seguros. Por ejemplo, si el acceso a un sitio interno está abierto a demasiadas personas o no se ha mantenido la configuración de permisos, los datos personales almacenados en ese sitio pueden ser vulnerables a una vulneración. Las directivas de sobreexposición de datos pueden evaluar los datos de estos riesgos y alertarle de posibles problemas.

Cuando se detecta una coincidencia de directiva, puede enviar a los usuarios notificaciones por correo electrónico que incluyan opciones de corrección para resolver problemas. Para la sobreexposición de datos, estos incluyen hacer que los elementos de contenido sean privados, notificar a los propietarios de contenido o etiquetar elementos para su revisión posterior.

Nuestro proceso de configuración de directivas facilita el establecimiento de condiciones de directiva. Tiene control total sobre el tiempo de las alertas y la frecuencia de los correos electrónicos que atraen la atención de los usuarios sobre las prácticas de control de datos seguras.

Hay dos maneras de crear una directiva: a partir de una **plantilla**, que es nuestra rápida opción "lista para usar" mediante la configuración predeterminada; o la opción **personalizada** , que es un proceso guiado para establecer condiciones, alertas y notificaciones.

## <a name="quick-setup-use-a-template-with-default-settings"></a>Configuración rápida: usar una plantilla con la configuración predeterminada

La directiva de sobreexposición de datos predeterminada evalúa los datos personales en los tres niveles de acceso: público, externo e interno.

Siga estos pasos para crear una directiva de transferencia de datos predeterminada:

1. En el [Centro de cumplimiento de Microsoft 365](https://compliance.microsoft.com/), busque Priva Privacy Risk Management en el panel de navegación izquierdo y seleccione **Directivas**.

2. Seleccione **Crear una directiva** en la esquina superior derecha de la pantalla, que muestra un panel flotante que enumera todas las opciones de creación de directivas.

3. En el cuadro **Sobreexposición de datos** , seleccione **Crear**.

4. Un panel flotante contiene detalles de directiva. Al seleccionar **Ver configuración** , se mostrarán los valores predeterminados. Puede editar la configuración desde aquí, lo que le lleva al proceso guiado que se describe a continuación. Para seguir creando la directiva con la configuración predeterminada, simplemente escriba un nombre descriptivo y, a continuación, seleccione **Crear directiva**.

La directiva se creará y la encontrará en la página **Policías** . Comienza en [modo de prueba](risk-management-policies.md#testing-a-policy) para que pueda supervisar cómo funciona antes de activarlo.

#### <a name="default-data-overexposure-policy-settings"></a>Configuración de directiva de sobreexposición de datos predeterminada

Una directiva de sobreexposición de datos creada a partir de la plantilla detectará:

- Cuando un usuario proporciona acceso demasiado amplio a los elementos que contienen datos personales almacenados en el OneDrive o SharePoint de su organización. Por ejemplo, la directiva detectará el uso compartido de datos personales de las siguientes maneras:
    - A través de un vínculo al que cualquier usuario del público puede acceder
    - A través de un vínculo o debido a permisos que permiten que todos los usuarios de la organización accedan
    - Concesión de derechos de acceso a usuarios externos o invitados para OneDrive o SharePoint archivos
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

Complete los pasos siguientes para crear una nueva directiva de sobreexposición de datos:

1. En el [Centro de cumplimiento de Microsoft 365](https://compliance.microsoft.com/), busque Priva Privacy Risk Management en el panel de navegación izquierdo y seleccione **Directivas**.

2. Seleccione el botón **Crear una directiva** en la esquina superior derecha de la pantalla, que muestra un panel flotante que enumera todas las opciones de creación de directivas.

3. En el cuadro **Personalizado** , seleccione **Crear**.

4. En la página **Nombre y tipo** , seleccione la plantilla **Directiva de sobreexposición de datos** . Escriba un nombre de directiva que le ayude a identificarla fácilmente en la lista en la página **Directivas** , escriba una descripción opcional y, a continuación, seleccione **Siguiente**.

5. En la página **Datos que se van a supervisar** , elija el tipo de datos personales que desea que supervise la directiva. Hay dos opciones:
    - **Grupos de clasificación**: agrupaciones de tipos de información confidencial que se usan para detectar contenido relacionado con datos personales o regulaciones específicas. Si selecciona esta opción, deberá seleccionar **+Agregar grupos de clasificación** para elegir uno o varios grupos de la lista proporcionada.
    - **Tipos de información confidencial individuales**: seleccione esta opción para elegir entre una lista de [tipos de información confidencial](/microsoft-365/compliance/sensitive-information-type-entity-definitions) individuales.

    Obtenga más información sobre [cómo elegir los datos que se van a supervisar](risk-management-policies.md#choose-data-to-monitor). Cuando haya terminado de seleccionar los datos que desea supervisar, seleccione **Siguiente**.

6. En la página **Usuarios y grupos** , elija a qué usuarios de su organización se aplicará la directiva. Puede seleccionar todos los usuarios individuales y todos los grupos de distribución Office 365, o puede seleccionar usuarios y grupos específicos. Obtenga más información sobre [cómo elegir usuarios y grupos](risk-management-policies.md#choose-users-and-groups). Cuando haya acabado, seleccione **Siguiente**.

7. En la página **Ubicaciones**, seleccione todas las ubicaciones de datos de Microsoft 365 que desea que la directiva cubra. Elija entre cuentas de OneDrive y sitios de SharePoint.

    Dentro de SharePoint puede designar todos los sitios o sitios específicos. Si selecciona **Sitios de SharePoint específicos**, puede escribir la dirección URL del sitio en el campo URL. También puede seleccionar **+Elegir sitios** y, en el panel flotante, active la casilla situada a la izquierda del nombre del sitio que desea seleccionar.

    Obtenga más información sobre [cómo elegir ubicaciones](risk-management-policies.md#choose-locations). Cuando haya terminado de seleccionar ubicaciones, seleccione **Siguiente**.

8. En la página **Condiciones** , seleccione qué tipo de condición de sobreexposición de datos detectará la directiva:
    - **Público**: cualquier persona con un vínculo puede acceder al contenido.
    - **Externo**: las personas específicas fuera de la organización tienen acceso.
    - **Interno**: todos los usuarios de la organización tienen acceso.
    
    La selección de más de un nivel de acceso ampliará el ámbito de los datos y podría producir cantidades significativamente mayores de alertas y notificaciones de usuario.

    Active la casilla situada junto a las opciones y, a continuación, seleccione **Siguiente**.

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