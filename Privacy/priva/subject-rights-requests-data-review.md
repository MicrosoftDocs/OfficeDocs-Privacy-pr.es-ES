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
ms.openlocfilehash: 5a72208894ff699675dcde230a7413b20c0b0a1e
ms.sourcegitcommit: a9ad5185174a9e8a7eea7583d257e8535c96a2ed
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/23/2022
ms.locfileid: "63746767"
---
# <a name="review-data-for-a-subject-rights-request"></a>Revisar los datos de una solicitud de derechos del sujeto

Después de crear una solicitud de derechos de [sujeto (más](subject-rights-requests-create.md) información) en Microsoft Priva, la solución Solicitudes de derechos de sujeto usará sus entradas para buscar coincidencias sobre el interesado en el entorno de Microsoft 365 de su organización. Una vez compilados estos datos, puede revisar los resultados, elegir qué incluir y redactar la información según sea necesario. Varios usuarios pueden colaborar en estos pasos a través de la interfaz Priva.

## <a name="step-1-review-request-details-and-monitor-progress"></a>Paso 1: Revisar los detalles de la solicitud y supervisar el progreso

Para ver los resultados iniciales de la búsqueda, vaya al área Priva del [Centro de cumplimiento de Microsoft 365 y abra](https://compliance.microsoft.com/) **Solicitudes de derechos de sujeto**. En esta página principal se puede encontrar una lista de todas las solicitudes de derechos de sujeto abiertas.

Seleccione la solicitud en la lista para ver los detalles de la solicitud. Aquí puede obtener más información sobre las propiedades de la solicitud, los resultados de la búsqueda y el estado de la solicitud. Esta página se convertirá en el centro para trabajar y colaborar en la administración de los archivos encontrados, la creación de informes y exportaciones y la finalización de la solicitud.

Los iconos de la página de detalles de la solicitud incluyen:

- **Detalles**: los detalles esenciales sobre la solicitud, incluida la fecha límite y la fecha de solicitud, su descripción y el reglamento de privacidad relacionado.
- **Progreso**: escala de tiempo que indica los pasos completados y las tareas pendientes de finalizar.
- Estadísticas sobre la fase de progreso actual. Este icono puede mostrar información como un resumen de estimación de datos, cuántos elementos se encontraron en la búsqueda y sus ubicaciones en Microsoft 365 o el estado de las exportaciones.
- **Elementos prioritarios que se revisarán**: este icono mostrará información sobre los elementos importantes que Priva haya detectado por usted. Por ejemplo, esto podría incluir información confidencial que ya lleva una etiqueta de confidencialidad de Microsoft o elementos con datos sobre varias personas que pueden requerir una redacción. Esto ayudará a los administradores a saber dónde empezar a revisar. Los elementos de prioridad se pueden encontrar en Datos recopilados mediante el filtrado por la columna "Tipos de prioridad".

### <a name="understand-progress-stages"></a>Comprender las fases de progreso

Las solicitudes de derechos de sujeto pasan por varias fases. Algunos estados progresan automáticamente y otras fases avanzan cuando los administradores y colaboradores de solicitudes de derechos de sujeto completan pasos esenciales como revisar archivos.

Dado que es posible que las solicitudes deban trabajarse con el tiempo o con varios colaboradores, Priva proporciona actualizaciones continuas sobre el estado y las instrucciones sobre los siguientes pasos a seguir. Estas actualizaciones se pueden ver en la pestaña **Información** general de la página de detalles de una solicitud de derechos de sujeto.

#### <a name="data-estimate"></a>Estimación de datos
Una vez que cree una solicitud, Priva empezará inmediatamente a buscar posibles coincidencias con el interesado en su Microsoft 365 de datos. Una vez identificados todos los elementos que creemos que coinciden con sus criterios, verá la estimación en la tarjeta  de resumen de estimación de datos en la página **Información general de** la solicitud. La cantidad de datos dentro del ámbito de la búsqueda afectará al tiempo que se necesitará para completar la estimación.

La solicitud se moverá automáticamente a la siguiente fase de recuperación de datos, donde se recopilan todos los elementos de contenido para que las partes interesadas puedan colaborar en la revisión de datos. En algunos casos, pausaremos la estimación de datos antes de pasar a la recuperación y le notificaremos los siguientes pasos a seguir antes de continuar.

También puede elegir pausar automáticamente en la fase de estimación de datos cuando cree por primera vez una solicitud de derechos de sujeto. Durante el proceso de creación, seleccione la **opción Obtener una estimación en primer** lugar durante el **paso Configuración de** búsqueda. Revise los detalles sobre el [paso de configuración de búsqueda](subject-rights-requests-create.md#define-search-settings).

#### <a name="pause-in-data-estimate-for-large-search-results"></a>Pausar en la estimación de datos para resultados de búsqueda grandes

Priva observará si se proyecta que la estimación de datos devolverá un gran número de elementos para revisar (más de 10.000 elementos). La estimación se pausará para que pueda obtener una vista previa de los [](subject-rights-requests-create.md#refine-your-search) resultados y decidir si desea editar la consulta de búsqueda para dirigirse a ubicaciones o condiciones más específicas, o bien seguir recuperando los elementos identificados.  Le mostraremos en pantalla el número de elementos y el volumen de datos que coinciden con la búsqueda. Tendrás una o ambas opciones en una barra de mensajes en la parte superior de la pantalla:

- Un **botón Editar consulta de** búsqueda le llevará directamente a la configuración de búsqueda de la solicitud para establecer parámetros más estrictos y generar una nueva estimación.
- Siempre que la consulta de búsqueda no supere los 300.000 elementos, también verá una opción para **Recuperar datos**. Esto le permite elegir no editar la búsqueda y seguir recopilando los datos.

#### <a name="retrieve-data"></a>Recuperar datos
La fase de recuperación de datos es cuando todos los archivos, correos electrónicos, chats, imágenes y otros elementos de contenido que contienen los datos personales del interesado se recuperan y se juntan en un contenedor de almacenamiento de blobs de Azure para su revisión. La recuperación de datos puede tardar unos minutos o mucho más en función del volumen de datos. Una vez completada esta fase, la solicitud se mueve automáticamente a la siguiente fase de **Revisar datos**.

#### <a name="review-data"></a>Revisar datos
 En esta fase, los colaboradores deben revisar los resultados en la  pestaña Datos recopilados y realizar todas las tareas aplicables, como la redacción, la aplicación de etiquetas y la adición de notas. Cuando haya terminado con la revisión, seleccione **Completar revisión**.

#### <a name="generate-reports"></a>Genere informes
Los informes se están generando en esta fase. Una vez completados, se pueden encontrar en la **pestaña** Informes. Los archivos terminados se pueden exportar para su revisión final y entrega al interesado que realizó la solicitud.

#### <a name="close-the-request"></a>Cerrar la solicitud
Una solicitud cerrada indica que se ha completado todo el trabajo para cumplir con esta solicitud de derechos de sujeto. Todos los datos recopilados y los informes se conservarán según la configuración [de retención de datos](priva-settings.md#data-retention-periods).

## <a name="step-2-optional-view-and-edit-search-queries"></a>Paso 2 (opcional): Ver y editar consultas de búsqueda

Para ver información detallada sobre la búsqueda de datos detrás de una solicitud de derechos de sujeto, seleccione **Ver detalles de consulta de búsqueda**. Se abre un panel que resume la consulta y muestra más detalles sobre lo que se encontró.

Aquí tiene la opción de Obtener una **vista previa** de los resultados de la búsqueda para ver qué tipo de contenido se devolverá para esta consulta. Si desea cambiar las propiedades de esta búsqueda y no ha iniciado la fase Recuperar datos, puede usar la opción **Editar consulta de** búsqueda.

El proceso de consulta de búsqueda de edición le permite cambiar o agregar propiedades para la identificación del interesado, los filtros y condiciones de búsqueda y las ubicaciones en las que buscar datos (incluidos Exchange, SharePoint, OneDrive o Teams). Usa estas opciones para alcanzar el nivel de especificidad deseado. Puedes revisar la versión final de la nueva consulta antes de presionar **Guardar**.

Cuando termine de editar la consulta de búsqueda, se ejecutará una nueva búsqueda para reemplazar los resultados de búsqueda anteriores. Esto restablece el estado de la sección **Progreso** al primer paso, **Estimación de datos**. La nueva búsqueda puede tardar hasta 60 minutos en completarse. Una vez hecho esto, verá los resultados actualizados en la página de detalles de la solicitud.

## <a name="step-3-review-data"></a>Paso 3: Revisar datos

En esta fase, los colaboradores deben revisar los resultados en la **pestaña Datos recopilados**. Se configurará Teams canal de contenido automáticamente para facilitar la revisión de contenido por parte de todas las partes interesadas. Consulta [Colaborar en la revisión de datos](#collaborate-on-data-review) para obtener más información. A continuación se describen las tareas esenciales para el paso de revisión de datos.

#### <a name="mark-items-as-include-or-exclude-and-add-notes"></a>Marcar elementos como Incluir o Excluir y agregar notas

Revise la lista de elementos identificados para determinar si los datos personales del interesado están en cada elemento. Si el elemento contiene la información del interesado y pertenece como parte del informe final al interesado, marca el elemento como Incluir seleccionando Incluir en la  barra de comandos en  la parte superior de la lista de elementos. También puede seleccionar el botón azul **Incluir** en el área de revisión de contenido a la derecha de la lista de elementos. Al seleccionar **Incluir**, aparece un panel desplegable con una opción para agregar notas. Cuando haya terminado, seleccione **Enviar para** guardar el estado de revisión del elemento como **Incluir**.

Si no necesita incluir un elemento como parte de la solicitud, seleccione **Excluir** en la barra de comandos o el botón Excluir en  el área de revisión de contenido. Excluir un elemento significa que no es relevante para la solicitud de derechos del sujeto y el elemento no se incluirá en los informes [finales](subject-rights-requests-reports.md) que se generan para el interesado.

> [!NOTE]
> Si marca un elemento **Exclude**, debe agregar una nota como justificación de por qué no pertenece a la solicitud de derechos del sujeto. Las notas son para fines internos y no se incluyen en los informes finales.

Si el contenido parece ser un falso positivo, seleccione No  coincidir para excluir el archivo de los informes finales y marcar el elemento como algo que no debería haber sido detectado en la búsqueda. En el **panel desplegable Marcar como** no coincidir, seleccione Confirmar para  que sepamos que el elemento no coincide con los criterios de búsqueda.

#### <a name="apply-tags"></a>Apply tags

Las etiquetas se pueden usar para ayudarle a identificar elementos que necesitan más atención. Priva proporciona tres etiquetas predeterminadas ( **Seguimiento**, **Eliminar** y **Actualizar** ) para las que puede establecer una descripción. Priva también proporciona dos etiquetas personalizadas que puede nombrar y describir.

Por ejemplo, si durante la revisión de datos determina que la organización no necesita conservar un elemento de contenido, puede aplicar la etiqueta **Eliminar** y, a continuación, exportar una lista de todos los archivos etiquetados para que pueda volver atrás y eliminar los elementos identificados cuando haya terminado con la solicitud.

Las cinco etiquetas que se establecen y administran en [Configuración](priva-settings.md#data-review-tags) se aplican a todas las solicitudes de derechos de sujeto.

**Para agregar o quitar etiquetas:**

- Seleccione el elemento de la lista en la **pestaña Datos recopilados** de la solicitud.
- En el área de vista previa del elemento a la derecha de la lista, seleccione el **botón Aplicar etiquetas** en la fila inferior. También puede seleccionar los tres puntos a la derecha del nombre del elemento y seleccionar la **opción Aplicar etiquetas** .
- Aparece un panel desplegable con la lista de etiquetas. Active la casilla situada junto a cualquiera de las etiquetas que desea aplicar al elemento. Si se desaproteba una casilla, se quitará la etiqueta.
- Cuando esté satisfecho con las selecciones, seleccione **Guardar**, que guarda las selecciones de etiqueta y cierra el panel desplegable.

**Para agregar etiquetas personalizadas o actualizar descripciones de etiquetas:**
- En la página Solicitudes de derechos de sujeto, seleccione **Configuración** en la esquina superior derecha de la pantalla para llegar a la configuración de Priva.
- Vaya a la **página Etiquetas de revisión de** datos y seleccione la etiqueta para introducir una descripción y, para las etiquetas personalizadas, un nombre. Obtenga más información sobre [la configuración de etiquetas](priva-settings.md#data-review-tags).

**Para exportar una lista de elementos etiquetados:**
- Vaya a la **página Datos recopilados** en una solicitud de derechos del sujeto.
- Encima de la lista de elementos, seleccione el icono de flecha abajo que indica **Exportar** al pasar el mouse sobre él.
- Se Excel un archivo de Excel se descargará. Abra el archivo cuando termine de descargar.

El archivo Excel muestra las propiedades de todos los elementos recopilados por la búsqueda de la solicitud. Busque la **columna Etiquetas** para identificar y ordenar los elementos por etiqueta.

#### <a name="use-the-annotate-command-to-redact-text"></a>Usar el comando Anotar para redactar texto
Use **Anotación para** crear marcas en línea o redactar datos en un archivo seleccionado. Por ejemplo, si necesita incluir un archivo para una persona que también contiene la información personal de otros, puede usar la redacción **Área (** debajo del botón Dibujo de la barra de comandos) para cerrar toda la información que no pertenezca a la persona que realizó la solicitud. Una vez completadas las ediciones, seleccione **Incluir** para agregar el archivo redactado a la solicitud. La anotación crea una copia del archivo, de modo que no se modifica nada en el archivo original y permanecerá en su ubicación original. La copia se almacena en el blob de Azure.

#### <a name="enter-notes-about-a-file"></a>Escribir notas sobre un archivo
Para agregar o revisar notas en un elemento, seleccione el elemento de su fila y vaya a la pestaña Notas **del** archivo del área de revisión de contenido a la derecha. También puede usar la opción **Agregar nota de archivo** para crear un nuevo comentario. Para revisar o agregar notas en un nivel de caso general, vaya a la pestaña **Notas** principal anterior y use **Agregar nota de caso**. Estas notas serán visibles para los usuarios que trabajen en la solicitud, pero no se incluirán en el informe final ni se compartirán con el interesado.

#### <a name="complete-the-review"></a>Completar la revisión

Cuando se hayan revisado todos los elementos y haya establecido su estado como **Incluir****, Excluir** o No coincidir **,** es el momento de cerrar el paso de revisión seleccionando el botón Revisar completo en la  esquina superior derecha dentro de la solicitud. Un panel desplegable mostrará un resumen de los datos y agregará las notas relacionadas. Estas notas son para el mantenimiento de registros internos y no se comparten con el interesado.

Seleccione **Completar revisión** en el panel desplegable para finalizar el paso de revisión. Los resúmenes de sus decisiones se proporcionan más adelante en la **pestaña** Informes.

### <a name="collaborate-on-data-review"></a>Colaborar en la revisión de datos

Priva admite la colaboración Microsoft Teams para permitir que el grupo trabaje conjuntamente en solicitudes de derechos de sujeto. Al crear una nueva solicitud, se crea automáticamente un canal de Teams y se asocia a la solicitud de forma predeterminada. Aquí puede analizar la solicitud y compartir de forma segura la entrada y las contribuciones. Para unirse a la conversación, abra la solicitud y use la **opción Chat with collaborators** . Esto abrirá Microsoft Teams y lo colocará dentro del canal General para el sitio de grupo de la solicitud de derechos de sujeto.

Para revisar la lista de colaboradores activos que pueden ver y contribuir a su sitio de grupo, dentro de su solicitud de derechos de asunto, abra la **pestaña Colaboradores** . Para agregar usuarios adicionales para colaborar en esta solicitud, seleccione la opción **Agregar un colaborador**.

Para cambiar el comportamiento predeterminado de generar sitios Teams al crear una solicitud de derechos de sujeto, vaya a **Configuración** en la navegación superior y seleccione Teams colaboración para  modificar la configuración.

También puede usar la opción  Compartir en la parte superior derecha dentro de una solicitud de derecho de asunto para hacer que los usuarios entren en bucle a través de Teams o correo electrónico, o para copiar el vínculo a la página en Priva. Compartir a través de Teams permite seleccionar un sitio y canal de Teams existentes disponibles para su cuenta, donde se mostrará un vínculo a este caso junto con cualquier mensaje que proporcione.

## <a name="step-4-close-the-request"></a>Paso 4: Cerrar la solicitud

Cuando haya realizado todas las acciones necesarias para resolver la solicitud de derechos de sujeto, seleccione **Cerrar la solicitud**. Esto crea el informe final, que se puede encontrar en la **pestaña Informes**. La finalización puede tardar un tiempo en función del número de archivos de la solicitud.

## <a name="next-steps"></a>Siguientes pasos
Para obtener más información sobre cómo trabajar con informes y completar solicitudes de derechos de sujeto, vea [Generar informes y cumplir una solicitud de derechos de sujeto](subject-rights-requests-reports.md).

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legales

[Declinación de responsabilidades legales de Microsoft Priva](priva-disclaimer.md)
