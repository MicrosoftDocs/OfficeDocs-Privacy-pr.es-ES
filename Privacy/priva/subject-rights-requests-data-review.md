---
title: Revisar los datos de una solicitud de derechos del sujeto
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
description: Obtenga información sobre cómo revisar los datos de solicitud de derechos del sujeto recopilados por Microsoft Priva y colaborar en la finalización de la solicitud.
ms.openlocfilehash: cac4064a1e0dc2860d061748793a91c0b86e0896
ms.sourcegitcommit: f145dff5e387a8e26db2f3a2c7de125978fbacc9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/28/2022
ms.locfileid: "62249201"
---
# <a name="review-data-for-a-subject-rights-request"></a>Revisar los datos de una solicitud de derechos del sujeto

Después de crear una solicitud de derechos de [sujeto (más](subject-rights-requests-create.md) información) en Microsoft Priva, la solución Solicitudes de derechos de sujeto usará sus entradas para buscar coincidencias sobre el interesado en el entorno de Microsoft 365 de su organización. Una vez compilados estos datos, puede revisar los resultados, elegir qué incluir y redactar la información según sea necesario. Varios usuarios pueden colaborar en estos pasos a través de la interfaz Priva.

## <a name="step-1-review-request-details-and-monitor-progress"></a>Paso 1: Revisar los detalles de la solicitud y supervisar el progreso

Para ver los resultados iniciales de la búsqueda, vaya al área Priva del [Centro de cumplimiento de Microsoft 365 y abra](https://compliance.microsoft.com/) **Solicitudes de derechos de sujeto**. En esta página principal se puede encontrar una lista de todas las solicitudes de derechos de sujeto abiertas.

Seleccione la solicitud en la lista para ver los detalles de la solicitud. Aquí puede obtener más información sobre las propiedades de la solicitud, los resultados de la búsqueda y el estado de la solicitud. Esta página se convertirá en el centro para trabajar y colaborar en la administración de los archivos encontrados, la creación de informes y exportaciones y la finalización de la solicitud.

Los iconos de la página de detalles de la solicitud incluyen:

- **Detalles**: los detalles esenciales sobre la solicitud, incluida la fecha límite y la fecha de solicitud, su descripción y el reglamento de privacidad relacionado.
- **Progreso**: escala de tiempo que indica los pasos completados y las tareas pendientes de finalizar.
- Estadísticas sobre la fase de progreso actual. Este icono puede mostrar información como un resumen de estimación de datos, cuántos elementos se encontraron en la búsqueda y sus ubicaciones en Microsoft 365, o el estado de las exportaciones.
- **Elementos prioritarios que se revisarán**: este icono mostrará información sobre los elementos importantes que Priva haya detectado por usted. Por ejemplo, esto podría incluir información confidencial que ya lleva una etiqueta de confidencialidad de Microsoft o elementos con datos sobre varias personas que pueden requerir una redacción. Esto ayudará a los administradores a saber dónde empezar a revisar. Los elementos de prioridad se pueden encontrar en Datos recopilados mediante el filtrado por la columna "Tipos de prioridad".

### <a name="understand-progress-stages"></a>Comprender las fases de progreso

Las solicitudes de derechos de sujeto pasan por varias fases. Algunos progresan automáticamente a medida que Priva realiza su evaluación de datos y otros avanzan cuando los administradores y colaboradores de solicitudes de derechos de sujeto completan pasos esenciales como revisar, seleccionar y redactar archivos.

Dado que es posible que las solicitudes deban trabajarse con el tiempo o con varios colaboradores, Priva proporciona actualizaciones continuas sobre el estado y las instrucciones sobre los siguientes pasos a seguir. Estas actualizaciones se pueden ver en la página de información general de la solicitud de derechos del sujeto.

1. **Estimación de** datos: después de crear una solicitud, Priva identifica elementos que incluyen posibles coincidencias con el interesado y toma notas de sus ubicaciones en Microsoft 365. Cuando se haya realizado la estimación de datos, avanzará automáticamente para recuperar **datos, a** menos que haya errores o que la solicitud se ponga en pausa aquí para la revisión de administradores.
   - Es posible que la solicitud esté configurada para requerir una revisión de administrador en esta fase. Si el administrador determina que los resultados iniciales de la consulta de búsqueda son satisfactorios, puede continuar con la recuperación de datos. Si desea realizar cambios antes de continuar, puede elegir editar primero la consulta de búsqueda. Vea el paso 2 para obtener más información. No podrá editar la consulta de búsqueda una vez que inicie la fase de recuperación de datos.
   - Si la consulta de búsqueda devuelve una estimación de datos grande, lo que significa que está por encima del umbral recomendado de Priva para el tamaño o recuento de archivos, puede intentar revisar la búsqueda para refinar su ámbito. Tenga en cuenta que los archivos asociados con un elemento que coincida (por ejemplo, los datos adjuntos de archivos en un correo electrónico) pueden contar para el total. Las estimaciones de datos superiores al máximo de cálculo de datos grandes requerirán una revisión de búsqueda para continuar.
1. **Recuperar datos**: esta fase indica que Priva está en proceso de recuperar los datos. Una vez completado, avanzará automáticamente para revisar **los datos**.
1. **Revisar datos**: en esta fase, los colaboradores deben revisar los resultados en la  pestaña Datos recopilados y realizar todas las tareas aplicables, como la redacción, la aplicación de etiquetas y la adición de notas. Cuando haya terminado con la revisión, seleccione **Completar revisión**.
1. **Generar informes**: los informes se están generando en esta fase. Una vez completados, se pueden encontrar en la **pestaña** Informes. Los archivos terminados se pueden exportar para su revisión final y entrega al interesado que realizó la solicitud.

## <a name="step-2-optional-view-and-edit-search-queries"></a>Paso 2 (opcional): Ver y editar consultas de búsqueda

Para ver información detallada sobre la búsqueda de datos detrás de una solicitud de derechos de sujeto, seleccione **Ver detalles de consulta de búsqueda**. Se abre un panel que resume la consulta y muestra más detalles sobre lo que se encontró.

Aquí tiene la opción de Obtener una **vista previa** de los resultados de la búsqueda para ver qué tipo de contenido se devolverá para esta consulta. Si desea cambiar las propiedades de esta búsqueda y no ha iniciado la fase Recuperar datos, puede usar la opción **Editar consulta de** búsqueda.

El asistente para editar consultas de búsqueda ofrece la posibilidad de cambiar o agregar propiedades para la identificación del interesado, los filtros y condiciones de búsqueda y las ubicaciones en las que buscar datos (incluidos Exchange, SharePoint, OneDrive o Teams). Usa estas opciones para alcanzar el nivel de especificidad deseado. Puedes revisar la versión final de la nueva consulta antes de presionar **Guardar**.

Cuando termine de editar la consulta de búsqueda, se ejecutará una nueva búsqueda para reemplazar los resultados de búsqueda anteriores. Esto restablece el estado de la sección **Progreso** al primer paso, **Estimación de datos**. La nueva búsqueda puede tardar hasta 60 minutos en completarse. Una vez hecho esto, verá los resultados actualizados en la página de detalles de la solicitud.

## <a name="step-3-review-data"></a>Paso 3: Revisar datos

En esta fase, los colaboradores deben revisar los resultados en la **pestaña Datos recopilados** . Entre las tareas esenciales se incluyen:

1. Revise la lista de elementos identificados y elija si desea incluir cada archivo en los resúmenes o exportaciones. Si no necesita incluir una coincidencia notificada, seleccione la opción "Excluir". Si el contenido parece ser un falso positivo, puedes elegir "No coincidir" para excluir el archivo de los informes finales y marcar el elemento como algo que no debería haber sido recogido por la solicitud. Para establecer el estado de un elemento, use el menú de acción (puntos suspensivos verticales) junto a su nombre y seleccione la opción que desee. Si se le pide, agregue una nota de referencia interna para explicar su decisión. Las notas son necesarias al excluir archivos.
1. Use la **opción Aplicar etiquetas** para ayudarle a identificar los elementos que necesitan atención. Las etiquetas disponibles incluyen opciones proporcionadas por el sistema, por ejemplo, etiquetar un elemento para seguimiento y pueden incluir etiquetas personalizadas según se define en la configuración global.
1. Use **Anotación para** crear marcas en línea o redactar datos en un archivo seleccionado. Por ejemplo, si necesita incluir un archivo para una persona que también contiene la información personal de otros, puede usar la redacción **Área (** debajo del botón Dibujo de la barra de comandos) para cerrar toda la información que no pertenezca a la persona que realizó la solicitud. Una vez completadas las ediciones, seleccione **Incluir** para agregar el archivo redactado a la solicitud. La anotación crea una copia del archivo, de modo que no se modifica nada en el archivo original y permanecerá en su ubicación original. La copia se almacena en el blob de Azure.
1. Para revisar las notas de un elemento, selecciónelo y vaya a la pestaña **Notas del** archivo. También puede usar la opción **Agregar nota de archivo** para crear un nuevo comentario. Para revisar o agregar notas en un nivel de caso general, vaya a la pestaña **Notas** principal anterior y use **Agregar nota de caso**. Estas notas serán visibles para los usuarios que trabajen en la solicitud, pero no se incluirán en el informe final ni se compartirán con el interesado.
1. Cuando se hayan revisado todos los elementos y se hayan establecido sus estados, seleccione **Completar revisión**. Se abrirá un panel de sobrevía donde puede revisar un resumen de los datos y agregar las notas relevantes. Estas notas son para el mantenimiento de registros internos y no se comparten con el interesado.
1. Seleccione Completar revisión de nuevo para continuar. Los resúmenes de sus decisiones se proporcionan más adelante en la **pestaña** Informes.

### <a name="collaborate-on-data-review"></a>Colaborar en la revisión de datos

Priva admite la colaboración a Microsoft Teams para permitir que el grupo colabore en solicitudes de derechos de sujeto. Al crear una nueva solicitud, se crea automáticamente un canal Teams y se asocia a la solicitud de forma predeterminada. Aquí puede analizar la solicitud y compartir de forma segura la entrada y las contribuciones. Para unirse a la conversación, abra la solicitud y use la **opción Chat with collaborators** . Esto abrirá Microsoft Teams y lo colocará en el canal General del sitio de grupo de la solicitud de derechos de sujeto.

Para revisar la lista de colaboradores activos que pueden ver y contribuir a su sitio de grupo, dentro de su solicitud de derechos de asunto, abra la **pestaña Colaboradores** . Para agregar usuarios adicionales para colaborar en esta solicitud, seleccione la opción **Agregar un colaborador**.

Para cambiar el comportamiento predeterminado de generar sitios Teams al crear una solicitud de derechos de sujeto, vaya a **Configuración** en la navegación superior y seleccione Teams colaboración para  modificar la configuración.

También puede usar la opción  Compartir en la parte superior derecha dentro de una solicitud de derecho de asunto para hacer que los usuarios entren en bucle a través de Teams o correo electrónico, o para copiar el vínculo a la página en Priva. Compartir a través de Teams permite seleccionar un sitio y un canal de Teams existentes disponibles para su cuenta, donde se mostrará un vínculo a este caso junto con cualquier mensaje que proporcione.

## <a name="step-4-close-the-request"></a>Paso 4: Cerrar la solicitud

Cuando haya realizado todas las acciones necesarias para resolver la solicitud de derechos de sujeto, seleccione **Cerrar la solicitud**. Esto crea el informe final, que se cifrará y estará disponible en la **pestaña Informes**. La finalización puede tardar un tiempo en función del número de archivos de la solicitud.

## <a name="next-steps"></a>Pasos siguientes
Para obtener más información sobre cómo trabajar con informes y completar solicitudes de derechos de sujeto, vea [Generar informes y cumplir una solicitud de derechos de sujeto](subject-rights-requests-reports.md).

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legales

[Declinación de responsabilidades legales de Microsoft Priva](priva-disclaimer.md)
