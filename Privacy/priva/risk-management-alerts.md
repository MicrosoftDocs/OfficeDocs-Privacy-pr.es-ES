---
title: Investigar y corregir alertas en La administración de riesgos de privacidad
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
description: Obtenga información sobre cómo administrar las alertas y los problemas que plantean las coincidencias de directivas en la administración de riesgos de privacidad.
ms.openlocfilehash: 26b30082d4f7122e113d38e8357af26b3850fda2
ms.sourcegitcommit: f145dff5e387a8e26db2f3a2c7de125978fbacc9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/28/2022
ms.locfileid: "62249096"
---
# <a name="investigate-and-remediate-alerts-in-privacy-risk-management"></a>Investigar y corregir alertas en La administración de riesgos de privacidad

Microsoft Priva puede ayudar a dar visibilidad a los descubrimientos importantes de las directivas de sobreexposición de datos, minimización de datos o transferencia de datos. Dentro de la solución de administración de riesgos de privacidad, los administradores **pueden revisar** alertas sobre contenido que coincida con las condiciones de la directiva. Revisar alertas le permite identificar los casos que necesitan seguimiento. Puede hacerlo creando **problemas**. Los problemas dan a los usuarios una forma estructurada de revisar el contenido, asignar la gravedad del problema y colaborar en la corrección de problemas.

Si la directiva se ha configurado para enviar notificaciones a los usuarios, los propietarios de contenido también pueden realizar determinadas acciones correctivas directamente desde estos correos electrónicos o desde Teams. Para obtener más información, consulta [Enviar notificaciones de usuario en Privacy Risk Management](risk-management-notifications.md).

## <a name="view-current-alerts-and-issues"></a>Ver alertas y problemas actuales

La página **Información general de** Priva proporciona una vista de los resultados recientes con actualizaciones sobre áreas clave de interés, como las directivas con más coincidencias y las alertas de directivas activas actualmente. Para obtener más información sobre la información que proporciona esta vista, vea [Buscar y visualizar datos personales en Priva](priva-data-profile.md).

También puede obtener acceso a visualizaciones y detalles sobre las alertas y problemas a través de la página **directivas** principal. Seleccione **Ver alertas** **y Ver problemas** para ver detalles.

## <a name="manage-alerts"></a>Administrar alertas

Para evaluar las alertas activas y especificar cuáles requieren seguimiento, accede a la página **Alertas** . Proporciona una lista filtrable de alertas generadas por las directivas. Puede revisarlos individualmente para determinar las circunstancias en las que se desencadenaron.

Al seleccionar cualquier alerta, se abrirá un panel de sobrevía con detalles adicionales, como el número de elementos que coinciden y la gravedad según la configuración de la directiva. En la **pestaña Contenido** , puede revisar qué archivos participan en esta alerta. Esta información puede proporcionar información adicional sobre el evento específico que desencadenó la alerta, dónde residen los archivos y qué tipos de datos personales están implicados. Los desencadenadores de las alertas se determinan según las condiciones específicas de cada directiva. Por ejemplo, una alerta puede desencadenarse en una directiva de transferencia de datos si Priva detecta una transferencia entre los departamentos o regiones especificados de la directiva.

Después de evaluar cualquier alerta de la lista, puede seleccionar **Crear problema** para solicitar más investigación y acción por parte de los usuarios. Se le pedirá que asigne un nombre al problema y agregue cualquier comentario relevante para el contexto. También puede descartar alertas aquí si no requieren un seguimiento.

## <a name="manage-issues"></a>Administrar problemas

Los administradores crean problemas al evaluar las alertas sobre las coincidencias de directivas. Para realizar un seguimiento y resolver los problemas indicados, los usuarios pueden visitar la **página** Problemas. Desde aquí puede revisar los problemas individuales, investigar las condiciones de incitación, revisar los datos y realizar los pasos necesarios para cerrar el caso.

Esta página proporciona una lista de todos los problemas abiertos. Se enumeran por nombre y se ordenan por gravedad para ayudarle a priorizar los casos, incluidas las categorías alta, mediana y baja, junto con las categorías sin asignar. Seleccione cualquier problema de la lista para revisar su contenido y tomar medidas para resolverlo. Puede proporcionar a los problemas sin signo una clasificación de gravedad durante la revisión.

### <a name="review-issue-details"></a>Revisar detalles de problemas

Las páginas de detalles de problemas le guían a través del proceso de abordar los riesgos de privacidad identificados y controlar los archivos indicados.

Las pestañas de las páginas de detalles del problema proporcionan información sobre las alertas y el contenido asociados, incluidos:

- **Información** general: muestra información esencial sobre el problema. Consulta el estado actual del problema y las siguientes acciones recomendadas que se deben realizar. También puede ver información general sobre el contenido, la directiva asociada, los detalles sobre la alerta y la escala de tiempo. La escala de tiempo mostrará dónde está recuperando contenido. El contenido descargado se conservará temporalmente para su revisión.
- **Alertas**: una lista detallada de alertas asociadas con el problema.
- **Contenido**: una lista filtrable de elementos de contenido asociados. Seleccione cualquier elemento para ver detalles sobre él, incluidas las actividades que se han producido y su historial de corrección, si alguien ya ha realizado acciones en Priva para administrar los datos. También puede elegir realizar nuevas acciones de corrección.
- **Notas**: seleccione para agregar o ver las notas de su equipo sobre el problema.
- **Colaboradores**: ver y administrar la lista de colaboradores que pueden contribuir a resolver este problema.

### <a name="share-the-issue"></a>Compartir el problema

Agregar personas como colaboradores le permite compartir el problema con miembros adicionales de su empresa a través de un canal de Microsoft Teams seguro, correo electrónico de la empresa o mediante el uso compartido de un vínculo directamente a la página del problema en Priva. Estas opciones están disponibles en el **botón** Compartir. Al compartir a través de Teams, se le pedirá que seleccione entre los equipos disponibles de su organización, seleccione el canal específico y deje un mensaje sobre el problema, que se compartirá con el canal especificado.

## <a name="review-content-and-remediate-issues"></a>Revisar el contenido y corregir problemas

Para revisar el contenido asociado a un problema, elija la acción Revisar **contenido** si se le solicita o abra la **pestaña** Contenido. Seleccione cualquier archivo de la lista para verlo en su totalidad. Aquí puede ver detalles sobre el archivo, cualquier actividad en el registro y su historial de corrección, si se han realizado pasos anteriores para administrar este archivo.

Use el **botón Corregir** para tomar sus propias decisiones de control de datos para este contenido en Priva. Si selecciona el botón, puede elegir entre una o varias acciones de corrección. Entre las opciones se incluyen:

**Todas las directivas**

- **Notificar al propietario**: notificar al propietario del contenido sobre el problema detectado.
- **Aplicar etiqueta de retención**: agregue una etiqueta sobre la retención de datos para este elemento. [Obtenga más información sobre las etiquetas de retención](/microsoft-365/compliance/create-apply-retention-labels).
- **Aplicar etiqueta de** confidencialidad: agregue una etiqueta sobre la confidencialidad de los datos de este elemento. [Obtenga más información sobre las etiquetas de confidencialidad](/microsoft-365/compliance/sensitivity-labels).
- **Marcar como no coincidir**: identifique un resultado de búsqueda como un falso positivo para quitar el elemento de contenido de consideración.

**Minimización de datos**

- **Eliminar**: use esta opción para eliminar los datos de forma suave. El contenido se mueve a la carpeta de elementos eliminados o a la papelera de reciclaje (Exchange, SharePoint, OneDrive) o se elimina con una opción para recuperar (Teams mensajes). La eliminación puede revertirse en un período de tiempo establecido, según la configuración del servicio.

**Sobreexposición de datos y transferencia de datos**

- **Hacer privado**: quite el acceso abierto para este elemento de contenido.

Cada opción le pedirá que deje comentarios y cualquier otra información de soporte necesaria para el propietario del contenido antes de confirmar su elección.

Una vez que se hayan realizado todos los pasos de corrección (incluidas las acciones que considere aconsejables además de las opciones disponibles en Priva) y el problema esté listo para cerrarse,  use el botón Resolver y agregue sus comentarios finales antes de enviarlo.

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legales

[Declinación de responsabilidades legales de Microsoft Priva](priva-disclaimer.md)
