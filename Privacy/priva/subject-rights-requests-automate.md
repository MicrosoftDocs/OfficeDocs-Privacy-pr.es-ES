---
title: Integración con Microsoft Graph API y Power Automate
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
description: Obtenga información sobre cómo ampliar las funcionalidades de Solicitudes de los interesados Priva mediante la integración con Microsoft Graph API y Power Automate.
ms.openlocfilehash: e4fcad2067ece3d1a6338e6d4891c59d91205a33
ms.sourcegitcommit: 9315064bf5bb9e889318e61ec5f082f36c815e1e
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/02/2022
ms.locfileid: "65851645"
---
# <a name="integrate-and-extend-through-microsoft-graph-api-and-power-automate"></a>Integración y ampliación a través de Microsoft Graph API y Power Automate

Puede integrar Solicitudes de los interesados Priva con sus procesos y herramientas empresariales existentes mediante microsoft Graph Subject Rights Request API. También puede ampliar las funcionalidades de automatización de las solicitudes de derechos del sujeto mediante flujos de Power Automate integrados para tareas como la configuración de recordatorios de calendario y la creación de casos en ServiceNow.

## <a name="microsoft-graph-subject-rights-requests-api"></a>API de solicitudes de derechos de los interesados de Microsoft Graph

La API Microsoft 365 Subject Rights Request ofrece una manera sencilla pero eficaz de introducir la automatización en la estrategia de derechos del sujeto existente. Cuando una persona solicita información a su organización, nuestras API le permiten crear esas solicitudes dentro de Microsoft 365 en función de los criterios para esa solicitud. Puede crear la solicitud de derechos del sujeto en Microsoft 365, realizar un seguimiento de su progreso y confirmar cuándo se ha completado el procesamiento de la solicitud y si el contenido está listo para recuperarse.

Nuestras API están disponibles para que cualquier usuario pueda usar para que sus soluciones sean más extensibles, como ISV, asociados que buscan dar cabida a Microsoft 365 en sus soluciones y organizaciones que buscan usar las API con su línea de aplicaciones empresariales.

Consulte la documentación completa en [Uso de la API de solicitud de derechos de firmante de Microsoft Graph](/graph/api/resources/subjectrightsrequest-subjectrightsrequestapioverview).

## <a name="power-automate-templates-for-subject-rights-requests"></a>plantillas de Power Automate para solicitudes de derechos del sujeto

Microsoft Power Automate es un servicio de flujo de trabajo que automatiza las acciones entre aplicaciones y servicios. Subject Rights Requests incluye plantillas de Power Automate integradas para ayudar a los usuarios a administrar las solicitudes de derechos del sujeto. Los usuarios pueden configurar flujos de automatización para procesos como la creación de vales en ServiceNow y la adición de recordatorios de calendario sobre fechas de vencimiento. Para más información sobre Power Automate, visite la [documentación de Power Automate](/power-automate/getting-started).

Si ha adquirido una suscripción a Subject Rights Requests, no necesita una licencia de Power Automate independiente para usar las plantillas de Power Automate recomendadas. Estas plantillas se pueden personalizar para admitir su organización y cubrir los escenarios principales de solicitud de derechos del sujeto. Sin embargo, es posible que necesite licencias adicionales para usar características de Power Automate premium en estas plantillas o para crear su propia plantilla.

### <a name="available-templates"></a>Plantillas disponibles

- **Crear un registro para Priva caso de administración de privacidad en ServiceNow**: esta plantilla es para las organizaciones que desean usar su solución ServiceNow para realizar un seguimiento de los casos de solicitud de derechos del sujeto. Se le pedirá que escriba los detalles de la instancia de ServiceNow, incluida una cuenta para conectarse a ServiceNow. Esta cuenta debe tener la capacidad de crear un incidente en ServiceNow y rellenar los detalles del incidente. Una vez conectado a la instancia, los administradores de solicitudes de derechos del firmante podrán crear un registro para el caso en ServiceNow y, si es necesario, pueden personalizar lo que la plantilla rellenará en los campos seleccionados. Para obtener más información sobre el conector, consulte la [documentación del conector de ServiceNow](/connectors/service-now/).

- **Agregue un recordatorio de calendario para realizar un seguimiento de un caso de administración de privacidad de Priva**: esta plantilla es para establecer recordatorios de fecha de vencimiento en el calendario de Outlook para solicitudes de derechos del sujeto. La herramienta rellenará determinados detalles de las propiedades de la solicitud, como el nombre de la solicitud y su fecha de vencimiento. Puede agregar detalles descriptivos, especificar destinatarios y ajustar otras opciones avanzadas.

- **Obtener archivos por etiqueta para una solicitud de derechos de asunto de Priva**: esta plantilla le permite buscar archivos para la solicitud de derechos del sujeto a la que se le ha dado una etiqueta específica. Puede editar el flujo para realizar acciones personalizadas o ver la lista de archivos devueltos que se van a usar para procesos o herramientas internos.

### <a name="create-a-new-power-automate-flow-from-a-template"></a>Creación de un nuevo flujo de Power Automate a partir de una plantilla

1. En el [portal de cumplimiento Microsoft Purview](https://compliance.microsoft.com/), seleccione **Solicitudes de los interesados Priva** en el panel de navegación izquierdo.

2. Busque la solicitud de derechos del asunto en la que desea trabajar y selecciónela de la lista para abrir su página de detalles.

3. En la esquina superior derecha, seleccione **Automatizar** y, a continuación, seleccione **Administrar flujos Power Automate** para abrir el panel flotante flujos.

4. Seleccione **Nuevo** y elija la plantilla que desea usar en las opciones disponibles. Desde aquí, siga las indicaciones para personalizar y agregar pasos para terminar de compilar el flujo. Las opciones variarán en función de la plantilla que use (consulte los tipos de plantilla a continuación).

5. Cuando haya acabado, seleccione **Guardar**.

Después de guardar una instancia de la plantilla, debe ejecutarla desde la página de detalles de la solicitud para que la instancia de flujo tenga el contexto y el identificador correctos. Abra la solicitud, vuelva al menú **Automatizar** , seleccione la plantilla y seleccione **Ejecutar flujo**. Para ver las actividades anteriores, seleccione **Ver actividad de ejecución de flujo**.

### <a name="share-a-power-automate-flow"></a>Compartir un flujo de Power Automate

Compartir un flujo de Power Automate le permite agregar otro propietario y permitirle editar, actualizar y eliminar el flujo. Todos los propietarios pueden acceder al historial de ejecución y agregar o quitar otros propietarios. 

Para compartir un flujo, abra la solicitud de derechos de asunto con la que desea trabajar, seleccione **Automatizar** y, a continuación, seleccione **Administrar flujos de Power Automate**. En este panel puede seleccionar un flujo existente y, a continuación, usar la opción **Compartir** para agregar un usuario o un grupo.

Este panel también ofrece la opción de administrar las conexiones incrustadas a los servicios que se usan en el flujo de Power Automate. Cambiar esta configuración puede afectar a la capacidad de ejecutar el flujo.

### <a name="edit-or-delete-power-automate-flow"></a>Editar o eliminar Power Automate flujo

Para ajustar los detalles de un flujo de Power Automate, seleccione **Automatizar** en la esquina superior derecha de la página de detalles de una solicitud y, a continuación, seleccione **Administrar flujos de Power Automate**.

En el panel **Power Automate flujos**, seleccione el flujo que desea editar y seleccione **Editar** en la barra de comandos para editar o agregar pasos. Cuando haya terminado, seleccione **Guardar**.

Para eliminar un flujo, selecciónelo en la lista del panel **flujos de Power Automate** y seleccione **Eliminar** en la barra de comandos. El flujo se quitará para todos los propietarios y se desinstalará para todos los usuarios. Las instancias de flujo anteriores seguirán ejecutándose para evitar la pérdida de datos. Se le pedirá que confirme antes de que la eliminación sea definitiva.

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legal

[Microsoft Priva declinación de responsabilidades legal](priva-disclaimer.md)
