---
title: Investigación y corrección de alertas en Privacy Risk Management
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
description: Obtenga información sobre cómo administrar las alertas y los problemas generados por las coincidencias de directivas en Microsoft Priva Privacy Risk Management.
ms.openlocfilehash: a770a7b8d77e2d7792fc4ea8c68914dc62b48a27
ms.sourcegitcommit: 0e68501654f702d8b8b694ae696bb8bd7fa7cea6
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/07/2022
ms.locfileid: "65268333"
---
# <a name="investigate-and-remediate-alerts-in-privacy-risk-management"></a>Investigación y corrección de alertas en Privacy Risk Management

Microsoft Priva puede ayudar a proporcionar visibilidad sobre las detecciones importantes de la sobreexposición de datos, la minimización de datos o las directivas de transferencia de datos. Dentro de la solución Privacy Risk Management, los administradores pueden revisar **las alertas** sobre el contenido que coincide con las condiciones de la directiva. La revisión de alertas le permite identificar casos que necesitan seguimiento. Para ello, cree **problemas**. Los problemas proporcionan a los usuarios una manera estructurada de revisar el contenido, asignar la gravedad del problema y trabajar de forma colaborativa para corregir los problemas.

Si la directiva se ha configurado para enviar notificaciones a los usuarios, los propietarios de contenido también pueden realizar ciertas acciones correctivas directamente desde estos correos electrónicos o desde Teams. Para más información, consulte [Envío de notificaciones de usuario en Administración de riesgos de privacidad](risk-management-notifications.md).

## <a name="view-current-alerts-and-issues"></a>Visualización de alertas y problemas actuales

**La página Información general** de Priva proporciona una vista de los resultados recientes con actualizaciones sobre áreas clave de interés, como las directivas con más coincidencias y las alertas de directivas actualmente activas. Para obtener más información sobre la información que proporciona esta vista, consulte [Búsqueda y visualización de datos personales en Priva](priva-data-profile.md).

También puede acceder a visualizaciones y detalles sobre las alertas y los problemas a través de la página principal **Directivas** . Seleccione **Ver alertas** y **Ver problemas** para ver los detalles.

## <a name="manage-alerts"></a>Administrar alertas

Para evaluar las alertas activas y especificar las que requieren seguimiento, acceda a la página **Alertas** . Proporciona una lista filtrable de alertas generadas por las directivas. Puede revisarlos individualmente para determinar las circunstancias en las que se desencadenaron.

Al seleccionar cualquier alerta, se abrirá un panel flotante con detalles adicionales, como el número de elementos coincidentes y la gravedad que juzgue la configuración de la directiva. En la pestaña **Contenido** , puede revisar qué archivos están implicados en esta alerta. Esta información puede proporcionar información adicional sobre el evento específico que desencadenó la alerta, dónde residen los archivos y qué tipos de datos personales están implicados. Los desencadenadores de las alertas están determinados por las condiciones específicas de cada directiva. Por ejemplo, es posible que se desencadene una alerta en una directiva de transferencia de datos si Priva detecta una transferencia entre los departamentos o regiones especificados de la directiva.

Después de evaluar cualquier alerta de la lista, puede seleccionar **Crear problema** para solicitar más investigación y acción por parte de los usuarios. Se le pedirá que asigne un nombre al problema y agregue los comentarios pertinentes para el contexto. También puede descartar las alertas aquí si no requieren un seguimiento.

## <a name="manage-issues"></a>Administrar problemas

Los administradores crean problemas al evaluar alertas sobre coincidencias de directivas. Para realizar un seguimiento y resolver los problemas indicados, los usuarios pueden visitar la página **Problemas** . Desde aquí puede revisar problemas individuales, investigar las condiciones de instigación, revisar los datos y tomar los pasos necesarios para cerrar el caso.

Esta página proporciona una lista de todos los problemas abiertos. Se enumeran por nombre y se ordenan por gravedad para ayudarle a priorizar los casos, incluidas las categorías alta, media y baja, junto con sin asignar. Seleccione cualquier problema de la lista para revisar su contenido y tomar medidas para resolverlo. Puede conceder a los problemas sin asignar una clasificación de gravedad durante la revisión.

### <a name="review-issue-details"></a>Revisión de los detalles del problema

Las páginas de detalles del problema le ayudan a abordar los riesgos de privacidad identificados y a controlar los archivos indicados.

Las pestañas de las páginas de detalles del problema proporcionan información sobre las alertas y el contenido asociados, entre las que se incluyen:

- **Información general**: muestra información esencial sobre el problema. Consulte el estado actual del problema y las siguientes acciones recomendadas que debe realizar. También puede ver información general sobre el contenido, la directiva asociada, detalles sobre la alerta y la escala de tiempo. La escala de tiempo mostrará dónde está recuperando contenido. El contenido descargado se conservará temporalmente para su revisión.
- **Alertas**: una lista detallada de las alertas asociadas al problema.
- **Contenido**: lista filtrable de elementos de contenido asociados. Seleccione cualquier elemento para ver detalles sobre él, incluidas las actividades que se han producido y su historial de corrección, si alguien ya ha realizado acciones en Priva para administrar los datos. También puede optar por realizar nuevas acciones de corrección.
- **Notas**: seleccione para agregar o ver las notas del equipo sobre el problema.
- **Colaboradores**: vea y administre la lista de colaboradores que pueden contribuir a resolver este problema.

### <a name="share-the-issue"></a>Compartir el problema

Agregar personas como colaboradores le permite compartir el problema con miembros adicionales de su empresa a través de un canal de Microsoft Teams seguro, correo electrónico de la empresa o mediante el uso compartido de un vínculo directamente a la página del problema en Priva. Estas opciones están disponibles en el botón **Compartir** . Al compartir a través de Teams, se le pedirá que seleccione entre los equipos disponibles de su organización, seleccione el canal específico y deje un mensaje sobre el problema, que se compartirá con el canal especificado.

## <a name="review-content-and-remediate-issues"></a>Revisión del contenido y corrección de problemas

Para revisar el contenido asociado a un problema, elija la acción **Revisar contenido** si se le solicita o abra la pestaña **Contenido** . Seleccione cualquier archivo de la lista para verlo en su totalidad. Aquí puede ver detalles sobre el archivo, las actividades del registro y su historial de corrección, si se han realizado pasos anteriores para administrar este archivo. Seleccione **Corregir** para realizar una o varias de las acciones que se enumeran a continuación.

- **Notificar al propietario**: notifique al propietario del contenido sobre el problema detectado.

- **Aplicar etiqueta de retención**: agregue una etiqueta para este elemento que pueda conservar, eliminar o conservar y, a continuación, eliminarla después de una hora especificada. [Obtenga más información sobre las etiquetas de retención](/microsoft-365/compliance/retention).

- **Aplicar etiqueta de confidencialidad**: agregue una etiqueta para este elemento que identifique su confidencialidad y, opcionalmente, agregue protección que incluya marcas visuales y cifrado. [Obtenga más información sobre las etiquetas de confidencialidad](/microsoft-365/compliance/sensitivity-labels).

- **Marcar como no una coincidencia**: identifique un resultado de búsqueda como falso positivo para quitar el elemento de contenido de la consideración.

- **Eliminar** (solo para directivas de minimización de datos): use esta opción para una eliminación temporal de los datos. El elemento se mueve a la carpeta de elementos eliminados o a la papelera de reciclaje (Exchange, SharePoint, OneDrive) o se elimina con una opción para recuperar (Teams mensajes). La eliminación se puede invertir en un período de tiempo establecido, en función de la configuración del servicio.

- **Hacer privado** (solo para las directivas de sobreexposición y transferencia de datos): quite el acceso abierto para este elemento de contenido.

Cada opción le pedirá que deje los comentarios y cualquier otra información auxiliar necesaria para el propietario del contenido antes de confirmar su elección.

Una vez que se hayan realizado todos los pasos de corrección (incluidas las acciones que considere aconsejables además de las opciones disponibles en Priva) y que el problema esté listo para cerrarse, use el botón **Resolver** y agregue los comentarios finales antes de enviarlos.

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legal

[Declinación de responsabilidades legal de Microsoft Priva](priva-disclaimer.md)
