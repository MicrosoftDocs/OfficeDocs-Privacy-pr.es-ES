---
title: Flujo de trabajo para solicitudes de derechos de sujeto
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
description: Comprenda los pasos del flujo de trabajo y la página de detalles de la solicitud en Solicitudes de datos personales Microsoft Priva.
ms.openlocfilehash: 794176260f6377862d34a66dc71cef1e811188b9
ms.sourcegitcommit: fe651dab4c89e67b21d37531c04e3996b7af1138
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/14/2022
ms.locfileid: "66060104"
---
# <a name="understand-the-workflow-and-request-details-pages"></a>Descripción de las páginas de detalles del flujo de trabajo y la solicitud

**En este artículo**: Obtenga información sobre los pasos de progreso a medida que crea y trabaja a través de una solicitud. Comprenda cómo trabajar con las conclusiones y características de la página de detalles de cada solicitud.

Al [crear una solicitud](subject-rights-requests-create.md) en la solución Solicitudes de derechos del sujeto, la información que proporcione se usa para buscar coincidencias sobre el interesado en el entorno de Microsoft 365 de la organización. Se cumplen los elementos coincidentes para que revise, tome decisiones sobre lo que debe incluir y redacte la información según sea necesario. Varios usuarios pueden colaborar en estos pasos dentro de la interfaz Solicitudes de derechos del sujeto. En la página [Información general](#overview-tab) de la solicitud se proporciona el estado de las fases de progreso y las instrucciones sobre los pasos siguientes que se van a realizar.

## <a name="progress-stages-for-requests"></a>Fases de progreso de las solicitudes

Cada solicitud pasa por varias fases. Algunas fases progresan automáticamente y otras se avanzan manualmente después de completar ciertos pasos, como la revisión de archivos.

- **Estimación de datos**: antes de recuperar los datos, Priva calcula la cantidad de datos que espera encontrar. En función de la cantidad de datos, la solicitud puede o no moverse automáticamente a la siguiente fase de recuperación de datos. Puede establecer una solicitud para pausar en la fase de estimación antes de recopilar datos; obtenga más información en [la estimación y recuperación de datos](subject-rights-requests-data-retrieval.md).

- **Recuperar datos**: se reúnen todos los archivos, correos electrónicos, chats, imágenes y otros elementos de contenido. Una vez completada esta fase, la solicitud pasa automáticamente a la siguiente fase de revisión de datos. Obtenga más información en [estimación y recuperación de datos](subject-rights-requests-data-retrieval.md).

- **Revisar datos**: los colaboradores revisan todos los datos recopilados, deciden cuáles pertenecen a la solicitud y realizan tareas como redactar archivos y agregar notas de casos. Obtenga más información sobre [cómo revisar los datos de una solicitud de derechos del interesado](subject-rights-requests-data-review.md). Después de finalizar la revisión de datos, avanzará manualmente a la siguiente fase para generar informes.

- **Generar informes**: cuando se realiza la revisión de datos, un usuario avanza manualmente a este paso. Priva genera los informes finales, que incluyen el paquete de datos que se va a compartir con el interesado, y los informes internos de los registros de la organización. Obtenga más información sobre [la generación de informes](subject-rights-requests-reports.md).

- **Cerrar la solicitud**: cuando se complete todo el trabajo, cierre la solicitud para indicar que se considera completada. Obtenga más información sobre [la generación de informes](subject-rights-requests-reports.md) para que pueda satisfacer y cerrar la solicitud.

## <a name="understanding-the-request-details-page"></a>Descripción de la página de detalles de la solicitud

Seleccione **Solicitudes de los interesados Priva** en el panel de navegación izquierdo del portal de cumplimiento de Microsoft Purview para acceder a las solicitudes creadas por su organización y ver su estado. Las tarjetas de estado de la página principal solicitudes de derechos del sujeto, que se muestran a continuación, muestran el número de solicitudes activas, cerradas y vencidas, y los tipos de solicitud principales. En la tabla debajo de las tarjetas de estado se enumeran todas las solicitudes creadas por su organización, con la solicitud creada más recientemente en la parte superior.

**Página principal solicitudes de derechos del sujeto:** 
![ Página principal solicitudes de derechos del sujeto.](../media/priva-srr-overview.png)

Para abrir la página de detalles de una solicitud, seleccione el nombre de la solicitud de la tabla. Aquí puede obtener más información sobre las propiedades de la solicitud, los resultados de la búsqueda y el estado de la solicitud. La página de detalles, que se muestra a continuación, se convertirá en el centro para trabajar y colaborar en la administración de los archivos encontrados, la creación de informes y exportaciones y la finalización de la solicitud.

**Página de detalles de una solicitud:**
![ Página de detalles de la solicitud de derechos del firmante.](../media/priva-srr-detailspage.png)

### <a name="overview-tab"></a>Pestaña Información general

La pestaña **Información general** de la página de detalles de la solicitud proporciona detalles sobre la solicitud, un indicador de progreso que muestra el paso actual e información clave sobre los datos encontrados. Esta página tiene tarjetas de estado individuales que se explican a continuación.

##### <a name="details"></a>Detalles

La tarjeta **Detalles** muestra información básica para orientarla a la solicitud, como su fecha límite, la fecha de creación, la descripción y la regulación de privacidad relacionada.

##### <a name="progress"></a>Progress

La tarjeta **Progreso** enumera cada paso del proceso: Estimación de datos, Recuperar datos, Revisar datos, Generar informes y Cerrar la solicitud. Un círculo azul relleno junto al paso indica el paso en el que se encuentra actualmente. Una marca de verificación dentro del círculo azul significa que el paso está completo. Un círculo vacío en blanco significa que el paso aún no se ha iniciado.

##### <a name="data-estimate-summary"></a>Resumen de la estimación de datos

La tarjeta **Resumen de estimación** de datos se muestra cuando la solicitud está en pausa en la [fase de estimación de datos](subject-rights-requests-data-retrieval.md#data-estimate). Muestra la ubicación y el número de elementos que se espera que recupere la búsqueda.

##### <a name="total-number-of-items-found"></a>Número total de elementos encontrados

La tarjeta **Número total de elementos encontrados** muestra el número de elementos de contenido encontrados y sus ubicaciones en Microsoft 365.

##### <a name="priority-items-to-review"></a>Elementos prioritarios que se van a revisar

El icono **Elementos prioritarios para revisar** muestra los elementos que puede que desee priorizar al iniciar la revisión. El icono muestra un recuento de elementos que pertenecen a las categorías siguientes:
- **Confidencial**: estos elementos tienen una [etiqueta de confidencialidad de Microsoft](/microsoft-365/compliance/sensitivity-labels) aplicada a ellos. Por ejemplo, un documento de Word con una etiqueta "Extremadamente confidencial". 
- **Datos de varias personas**: estos elementos contienen los datos personales de más de una persona. Si desea incluir estos elementos como parte del paquete de datos final, deberá redactar los datos irrelevantes en los archivos. Obtenga [detalles sobre la revisión de datos](subject-rights-requests-data-review.md). Para que Priva identifique elementos con datos de varias personas, su organización debe configurar la [coincidencia de datos para las solicitudes de derechos del interesado](subject-rights-requests-data-match.md).

**Cómo localizar los elementos de prioridad:**

En primer lugar, asegúrese de que ha habilitado la vista de ellos en la tabla De datos **recopilados** de elementos siguiendo estos pasos:

- En la pestaña **Datos recopilados** , seleccione **Personalizar columnas** en la parte superior de la lista de elementos.
- En el panel flotante **Editar columnas** , coloque una comprobación junto a **Tipos de prioridad**.
- Seleccione **Aplicar**. La lista de elementos ahora tendrá una columna **Tipos de prioridad** .

Ahora puede identificar los elementos de prioridad y buscarlos mediante la ordenación de la columna **Tipo de prioridad** para agrupar tipos similares.

### <a name="data-collected-tab"></a>Pestaña Datos recopilados

Cuando se identifican todos los elementos que coinciden con la configuración de búsqueda, se recopilan y se presentan en la pestaña **Datos recopilados** . Junto a la lista de elementos hay una pantalla de vista previa para revisar cada elemento, realizar censuras y marcar elementos como incluidos o excluidos como parte de la solicitud. Obtenga más detalles sobre el [paso de revisión y colaboración de datos](subject-rights-requests-data-review.md).

### <a name="notes-tab"></a>Pestaña Notas

La pestaña **Notas** permite a los colaboradores escribir notas sobre el trabajo realizado en la solicitud. Estas notas son visibles para todos los usuarios que trabajan en la solicitud, pero no se incluirán en el informe final ni se compartirán con el interesado.

### <a name="collaborators-tab"></a>Pestaña Colaboradores

La pestaña Colaboradores muestra todos los usuarios a los que se ha invitado a colaborar en los datos recopilados y cualquier canal de Teams asociado para la solicitud. El creador de la solicitud se muestra automáticamente como colaborador. Para invitar a nuevos colaboradores, seleccione el comando **Agregar colaborador** y escriba el nombre de un usuario para seleccionarlos de una lista. Más información sobre la [colaboración para la revisión de datos](subject-rights-requests-data-review.md#collaboration-for-data-review)

### <a name="reports-tab"></a>Ficha Informes

La pestaña **Informes** muestra todos los informes que se generan automáticamente al avanzar a la fase **Generar informes** . Los informes se dividen en dos categorías: informes para que pueda compartir con el interesado e informes destinados al uso interno de la organización. Obtenga detalles sobre [cómo trabajar con informes](subject-rights-requests-reports.md).

### <a name="history-tab"></a>Pestaña Historial

La pestaña **Historial** resume los eventos de nivel superior de la solicitud, incluidos los cambios en la fase de progreso y los agregados para el número de elementos incluidos, excluidos y redactados.

## <a name="next-steps"></a>Siguientes pasos

Visite [Create a subject rights request (Crear una solicitud de derechos de sujeto](subject-rights-requests-create.md) ) para obtener información sobre cómo se indica con su primera solicitud.

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legal

[Microsoft Priva declinación de responsabilidades legal](priva-disclaimer.md)