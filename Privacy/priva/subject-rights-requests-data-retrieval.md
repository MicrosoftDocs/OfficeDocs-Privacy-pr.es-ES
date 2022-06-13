---
title: Estimación y recuperación de datos en solicitudes de derechos del interesado
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
description: Comprenda cómo se recuperan los datos y cómo modificar la configuración de búsqueda en Solicitudes de datos personales Microsoft Priva.
ms.openlocfilehash: 9d35a7f37861d7d3ecc5d1bac7db92c75939b4c3
ms.sourcegitcommit: 3c83e8133a5a71f4e1d76a0b2981ab3ec9cd6602
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/13/2022
ms.locfileid: "66046750"
---
# <a name="data-estimate-and-retrieval"></a>Estimación y recuperación de datos

**En este artículo**: Descripción de las fases de estimación y recuperación de datos de una solicitud de derechos del interesado. Obtenga información sobre cómo ver la consulta de búsqueda de una solicitud y realizar modificaciones para refinar la búsqueda.

## <a name="data-estimate"></a>Estimación de datos
Una vez creada una solicitud, Priva comienza inmediatamente a buscar coincidencias con el interesado en el contenido del entorno de Microsoft 365. Una vez que hayamos identificado todos los elementos que creemos que coinciden con sus criterios, verá la estimación en la tarjeta **Resumen de la estimación de datos** en la página **Información general** de la solicitud. La cantidad de datos dentro del ámbito de la búsqueda afectará al tiempo que se tarda en completar la estimación.

La solicitud pasará automáticamente a la siguiente fase de **recuperación de datos**, donde todos los elementos de contenido se reúnen para que las partes interesadas colaboren en la revisión de los datos. En algunos casos, pausaremos la estimación de datos antes de pasar a la recuperación y le notificaremos los pasos siguientes que se deben seguir antes de continuar.

### <a name="pause-in-data-estimate"></a>Pausar en la estimación de datos

Hay dos motivos por los que una solicitud se pausará en la fase **De estimación de datos** :

1. Cuando cree una solicitud por primera vez, puede elegir obtener primero una estimación. Consulte el paso 5 en [Creación de una solicitud](subject-rights-requests-create.md#create-a-request) para obtener más información.

2. Si se proyecta que la estimación devuelve un gran número de elementos que se van a revisar (más de 10 000 elementos), el flujo de trabajo se pausa. En este punto, puede obtener una vista previa de los resultados y decidir si [desea editar la consulta de búsqueda](subject-rights-requests-create.md#refining-your-search) o continuar recuperando los elementos identificados.

Cuando la solicitud se pausa en **Estimación de datos**, verá una tarjeta en la página de detalles de la solicitud con información de resumen sobre el número de elementos, el volumen, su ubicación y un vínculo que le permite **ver los detalles de la consulta de búsqueda**.

![Tarjeta de estimación de datos.](../media/priva-srr-data-estimate.png)

## <a name="view-and-edit-search-queries"></a>Visualización y edición de consultas de búsqueda

Para ver información detallada sobre la búsqueda de la solicitud, seleccione **Ver detalles de la consulta de búsqueda** en la tarjeta **Resumen de estimación de datos** . Se abre un panel flotante que resume la consulta y muestra más detalles sobre lo que se encontró. Desde aquí, tiene las siguientes opciones:

- Seleccione **Vista previa de los resultados** para obtener una vista previa del tipo de contenido que se devolverá en la configuración de búsqueda actual.
- Seleccione **Editar consulta de búsqueda** para cambiar la configuración de búsqueda.

Al seleccionar **Editar consulta de búsqueda**, se le guiará a través de un proceso guiado para cambiar o agregar propiedades para identificar al interesado, cambiar las condiciones y ajustar las ubicaciones que desea que cubra la búsqueda. Siga las instrucciones de [Refinamiento de la búsqueda](subject-rights-requests-create.md#refining-your-search) para obtener información más detallada. Puede revisar la versión final de la nueva consulta de búsqueda y, a continuación, seleccionar **Guardar** para volver a iniciar la búsqueda.

Se generará una nueva estimación y el estado de la solicitud volverá a **Estimación de datos**. La nueva búsqueda puede tardar hasta 60 minutos en completarse. Una vez hecho esto, verá los resultados actualizados en la página de detalles de la solicitud.

Cuando esté listo para continuar, seleccione **recuperar datos** en la esquina superior derecha de la pantalla para avanzar a la fase de recuperación de datos.

## <a name="retrieve-data"></a>Recuperar datos

La fase de recuperación de datos es cuando se recuperan todos los archivos, correos electrónicos, chats, imágenes y otros elementos de contenido que contienen los datos personales del interesado. Los elementos se combinan en un contenedor de Azure Blob Storage para su revisión. La recuperación de datos puede tardar unos minutos o mucho más en función del volumen de datos.

Una vez completada esta fase, la solicitud se mueve automáticamente a la siguiente fase de **Revisar datos**.

## <a name="next-steps"></a>Pasos siguientes

Visite [Revisar los datos de una solicitud de derechos del interesado](subject-rights-requests-data-review.md) para obtener información sobre las tareas clave y colaborar con las partes interesadas en el paso **Revisar datos** .

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legal

[Microsoft Priva declinación de responsabilidades legal](priva-disclaimer.md)