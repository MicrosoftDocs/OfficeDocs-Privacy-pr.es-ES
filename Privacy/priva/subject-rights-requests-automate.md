---
title: 'Automatización de tareas en solicitudes de derechos de sujeto '
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
search.appverid:
- MOE150
- MET150
description: Obtenga información sobre cómo usar Microsoft Power Automate para ayudarle a automatizar tareas esenciales para las solicitudes de derechos de los sujetos en Priva.
ms.openlocfilehash: ec9edde16b60c2326ca899e587dfe5dc7a1e32f5
ms.sourcegitcommit: 09ecdaded9a9f8f79587f2acb978dc53b83e5c01
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/19/2022
ms.locfileid: "64930501"
---
# <a name="automate-tasks-in-subject-rights-requests"></a>Automatización de tareas en solicitudes de derechos de sujeto 

Microsoft Power Automate es un servicio de flujo de trabajo que automatiza las acciones entre aplicaciones y servicios. Al habilitar flujos de Power Automate para solicitudes de derechos de sujetos de Microsoft Priva, puede automatizar tareas importantes para casos y usuarios, como la creación de vales en ServiceNow o la adición de recordatorios de calendario sobre fechas de vencimiento. Para más información sobre Power Automate, visite su [sitio de documentación](/power-automate/getting-started).

Los clientes con suscripciones a solicitudes de derechos de sujeto no necesitan otra licencia de Power Automate para usar las plantillas de Power Automate recomendadas para Priva. Estas plantillas se pueden personalizar para admitir su organización y cubrir los escenarios principales de solicitud de derechos del sujeto. Si decide usar características de Power Automate Premium en estas plantillas, cree una plantilla personalizada con el conector de cumplimiento de Microsoft 365 o use plantillas de Power Automate para otras áreas de cumplimiento de Microsoft 365, es posible que necesite más licencias de Power Automate.

## <a name="create-a-new-power-automate-flow-from-a-template"></a>Creación de un nuevo flujo de Power Automate a partir de una plantilla

1. En el [portal de cumplimiento de Microsoft Purview](https://compliance.microsoft.com/), vaya a la sección Priva de la navegación y seleccione **Priva Subject Rights Requests (Priva Subject Rights Requests).**
1. Abra la solicitud de derechos de asunto con la que desea trabajar en la lista y seleccione **Automatizar** y, a continuación, **Administrar flujos de Power Automate**. Se abrirá el panel flotante Flujos.
1. Use la opción **Nuevo** y elija la plantilla que desea usar en las opciones disponibles. Desde aquí, siga las indicaciones del asistente para completar la configuración. Las opciones variarán en función del tipo de plantilla.

Después de guardar una instancia de la plantilla, debe ejecutarla desde la página de detalles de la solicitud de derechos del firmante para que la instancia de flujo tenga el contexto y el identificador correctos. Abra la solicitud, vuelva al menú **Automatizar** , seleccione la plantilla y seleccione **Ejecutar flujo**. Para ver las actividades anteriores, seleccione **Ver actividad de ejecución de flujo**.

### <a name="power-automate-templates-in-priva"></a>plantillas de Power Automate en Priva

- **Crear un registro para el caso de administración de privacidad en ServiceNow**: esta plantilla está destinada a las organizaciones que desean usar su solución ServiceNow para realizar un seguimiento de los casos de solicitud de derechos del sujeto. Se le pedirá que escriba los detalles de la instancia de ServiceNow, incluida una cuenta para conectarse a ServiceNow. Esta cuenta debe tener la capacidad de crear un incidente en ServiceNow y rellenar los detalles del incidente. Una vez conectado a la instancia, los administradores de solicitudes de derechos del firmante podrán crear un registro para el caso en ServiceNow y, si es necesario, pueden personalizar lo que la plantilla rellenará en los campos seleccionados. Para obtener más información sobre el conector, consulte la [página de referencia del conector de ServiceNow](/connectors/service-now/).
- **Crear un recordatorio de calendario**: esta plantilla es para establecer recordatorios de fecha de vencimiento en el calendario de Outlook para solicitudes de derechos del sujeto. La herramienta rellenará determinados detalles de las propiedades de la solicitud, como el nombre de la solicitud y su fecha de vencimiento. Puede agregar detalles descriptivos, especificar destinatarios y ajustar otras opciones avanzadas.
- **Obtener archivos por etiqueta para una solicitud de derechos de sujeto**: esta plantilla le permite buscar archivos para la solicitud de derechos del sujeto a la que se le dio una etiqueta específica. Puede editar el flujo para realizar acciones personalizadas o ver la lista de archivos devueltos para aprovechar los procesos o herramientas internos.

## <a name="share-a-power-automate-flow"></a>Compartir un flujo de Power Automate

Al compartir un flujo de Power Automate, puede agregar otro propietario y permitirle editar, actualizar y eliminar el flujo. Todos los propietarios también pueden acceder al historial de ejecución y agregar o quitar otros propietarios. Para compartir un flujo, abra la solicitud de derechos de asunto con la que desea trabajar, seleccione **Automatizar** y, a continuación, seleccione **Administrar flujos de Power Automate**. En este panel puede seleccionar un flujo existente y, a continuación, usar la opción Compartir para agregar un usuario o un grupo.

Este panel también ofrece la opción de administrar las conexiones incrustadas a los servicios que se usan en el flujo de Power Automate. Cambiar esta configuración puede afectar a la capacidad de ejecutar el flujo.

## <a name="edit-or-delete-power-automate-flow"></a>Editar o eliminar Power Automate flujo

Para ajustar los detalles de un flujo de Power Automate, abra la solicitud de derechos del firmante, seleccione **Automatizar** y seleccione **Administrar flujos de Power Automate**. En este panel, puede seleccionar un flujo existente para ver los detalles. Use Editar en cualquier sección para cambiar las propiedades y, a continuación, guarde.

Para quitar el flujo por completo, use la opción **Eliminar** . Quitará el flujo para todos los propietarios y lo desinstalará para todos los usuarios. Las instancias de flujo anteriores seguirán ejecutándose para evitar la pérdida de datos. Puede confirmar su elección antes de que la eliminación sea final.

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legal

[Declinación de responsabilidades legal de Microsoft Priva](priva-disclaimer.md)
