---
title: Automatizar las tareas de solicitudes de derechos de sujeto en la administración de privacidad
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
- MET150
description: Descubra cómo usar Microsoft Power Automate para ayudarle a automatizar tareas esenciales para solicitudes de derechos de sujeto en la administración de privacidad.
ms.openlocfilehash: df76e87e3298b2ccc6c897d485e695d0f1ae35c9
ms.sourcegitcommit: 85e085eb17af8b4efd1f45207445e1b3c3679600
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/19/2021
ms.locfileid: "60478317"
---
# <a name="automate-subject-rights-requests-tasks"></a>Automatizar tareas de solicitudes de derechos de sujeto

Microsoft Power Automate es un servicio de flujo de trabajo que automatiza las acciones entre aplicaciones y servicios. Al habilitar los flujos de Power Automate para la administración de privacidad para Microsoft 365, puede automatizar tareas importantes para casos y usuarios, como crear vales en ServiceNow o agregar avisos de calendario sobre fechas de vencimiento. Para obtener más información sobre Power Automate, visite su [sitio de documentación](/power-automate/getting-started).

Los clientes con Microsoft 365 que incluyan la administración de privacidad no necesitan otras licencias de Power Automate para usar las plantillas de administración de privacidad Power Automate privacidad recomendadas. Estas plantillas se pueden personalizar para admitir su organización y cubrir los escenarios principales de administración de privacidad. Si elige usar características de Power Automate premium en estas plantillas, cree una plantilla personalizada con el conector de cumplimiento de Microsoft 365 o use plantillas de Power Automate para otras áreas de cumplimiento en Microsoft 365, puede que necesite más licencias de Power Automate.

## <a name="create-a-new-power-automate-flow-from-a-template"></a>Crear un nuevo flujo Power Automate de una plantilla

1. En el [Centro de cumplimiento de Microsoft 365](https://compliance.microsoft.com/), vaya a la sección de administración de privacidad de la navegación y seleccione **Solicitudes de derechos del sujeto**.
1. Abra la solicitud de derechos de sujeto con la que desea trabajar en la lista y seleccione **Automatizar** y, a continuación, administre **Power Automate flujos**. Se abre el panel desplegable Flujos.
1. Use la **opción** Nuevo y elija la plantilla que desea usar de las opciones disponibles. Desde aquí, sigue las indicaciones del asistente para completar la configuración. Las opciones variarán según el tipo de plantilla.

Después de guardar una instancia de la plantilla, debe ejecutarla desde la página de detalles de la solicitud de derechos de sujeto para que la instancia de flujo tenga el contexto y el identificador adecuados. Abra la solicitud, vuelva al menú **Automatizar,** seleccione la plantilla y seleccione **Ejecutar flujo**. Puede ver las actividades anteriores seleccionando **Ver actividad de ejecución de flujo**.

### <a name="power-automate-templates-in-privacy-management"></a>Power Automate plantillas de privacidad

- **Cree un registro para casos de administración** de privacidad en ServiceNow: esta plantilla es para las organizaciones que desean usar su solución ServiceNow para realizar un seguimiento de los casos de solicitud de derechos de sujeto. Se le pedirá que escriba los detalles de la instancia de ServiceNow, incluida una cuenta para conectarse a ServiceNow. Esta cuenta debe tener la capacidad de crear un incidente en ServiceNow y rellenar los detalles del incidente. Una vez conectado a la instancia, los administradores de solicitudes de derechos de sujeto podrán crear un registro para el caso en ServiceNow y, si es necesario, pueden personalizar lo que la plantilla rellenará en campos seleccionados. Para obtener más información sobre el conector, vea la página de referencia [de ServiceNow Connector](/connectors/service-now/).
- **Crear un aviso de calendario:** esta plantilla es para establecer avisos de fecha de vencimiento en el calendario de Outlook para solicitudes de derechos de sujeto. La herramienta rellenará determinados detalles de las propiedades de la solicitud, como el nombre de la solicitud y su fecha de vencimiento. Puede agregar detalles descriptivos, especificar destinatarios y ajustar otras configuraciones avanzadas.
- **Obtener archivos por etiqueta para una** solicitud de derechos de sujeto: esta plantilla le permite buscar archivos para la solicitud de derechos de sujeto a la que se le dio una etiqueta específica. Puede editar el flujo para realizar acciones personalizadas o ver la lista de archivos devueltos para aprovechar los procesos o herramientas internos.

## <a name="share-a-power-automate-flow"></a>Compartir un flujo Power Automate de datos

Al compartir un Power Automate, puede agregar otro propietario y permitirle editar, actualizar y eliminar el flujo. Todos los propietarios también pueden tener acceso al historial de ejecución y agregar o quitar otros propietarios. Para compartir un flujo, abra la solicitud de derechos de sujeto con la que desea trabajar, seleccione **Automatizar** y, a continuación, seleccione **Administrar Power Automate flujos**. En este panel puede seleccionar un flujo existente y, a continuación, usar la opción Compartir para agregar un usuario o un grupo.

Este panel también le ofrece la opción de administrar las conexiones incrustadas a los servicios que se usan en el Power Automate flujo. Cambiar esta configuración puede afectar a la capacidad de ejecutar el flujo.

## <a name="edit-or-delete-power-automate-flow"></a>Editar o eliminar Power Automate flujo

Para ajustar los detalles de un flujo Power Automate, abra la solicitud de derechos del sujeto, seleccione **Automatizar** y seleccione Administrar **Power Automate flujos**. En este panel, puede seleccionar un flujo existente para ver detalles. Use Editar en cualquier sección para cambiar las propiedades y, a continuación, guardar.

Para quitar el flujo por completo, use la **opción** Eliminar. Quitará el flujo de todos los propietarios y lo desinstalará para todos los usuarios. Las instancias de flujo anteriores seguirán en ejecución para evitar la pérdida de datos. Puedes confirmar tu elección antes de que la eliminación sea definitiva.

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legales

[Declinación de responsabilidades legales de administración de privacidad](privacy-management-disclaimer.md)
