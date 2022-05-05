---
title: Revisión de los datos de una solicitud de derechos del interesado
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
description: Obtenga información sobre cómo revisar los datos de solicitudes de derechos del interesado recopilados por Microsoft Priva y colaborar en la finalización de la solicitud.
ms.openlocfilehash: 3a1211d391ee196ad431fe19ab9134386c9803a4
ms.sourcegitcommit: 6b88d22d0250cbb9a4ba1f71665f29cb67939851
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/05/2022
ms.locfileid: "65059764"
---
# <a name="review-data-for-a-subject-rights-request"></a>Revisión de los datos de una solicitud de derechos del interesado

Después de crear una solicitud de derechos del interesado ([más información](subject-rights-requests-create.md)) en Microsoft Priva, la solución Solicitudes de derechos del sujeto usará sus entradas para buscar coincidencias sobre el interesado en el entorno de Microsoft 365 de su organización. Una vez compilados estos datos, puede revisar los resultados, tomar decisiones sobre qué incluir y redactar la información según sea necesario. Varios usuarios pueden colaborar en estos pasos a través de la interfaz Priva.

## <a name="step-1-review-request-details-and-monitor-progress"></a>Paso 1: Revisar los detalles de la solicitud y supervisar el progreso

Para ver los resultados iniciales de la búsqueda, vaya al área Priva del [portal de cumplimiento de Microsoft Purview](https://compliance.microsoft.com/) y abra **Solicitudes de derechos del sujeto**. Puede encontrar una lista de todas las solicitudes de derechos de asunto abiertas en esta página principal.

Seleccione la solicitud en la lista para ver los detalles de la solicitud. Aquí puede obtener más información sobre las propiedades de la solicitud, los resultados de la búsqueda y el estado de la solicitud. Esta página se convertirá en el centro para trabajar y colaborar en la administración de los archivos encontrados, la creación de informes y exportaciones y la finalización de la solicitud.

En la pestaña **Información general** de la página de detalles de la solicitud se proporcionan detalles sobre la solicitud, un indicador de progreso que muestra el paso actual e información clave sobre los datos encontrados. Los iconos de esta página incluyen lo siguiente:

##### <a name="details"></a>Detalles

La tarjeta **Detalles** muestra información básica para orientarlo a la solicitud, como su fecha límite, la fecha de creación, la descripción y el reglamento de privacidad relacionados con la solicitud.

##### <a name="progress"></a>Progress

La tarjeta **Progreso** enumera cada paso del proceso: Estimación de datos, Recuperar datos, Revisar datos, Generar informes y Cerrar la solicitud. Un círculo azul relleno junto al paso indica el paso en el que se encuentra actualmente. Una marca de verificación dentro del círculo azul significa que el paso está completo y el círculo sin rellenar significa que el paso aún no se ha iniciado.

##### <a name="total-number-of-items-found"></a>Número total de elementos encontrados

Estadísticas sobre la fase de progreso actual. Este icono puede mostrar información como un resumen de estimación de datos, cuántos elementos se encontraron en la búsqueda y sus ubicaciones en Microsoft 365, o el estado de las exportaciones.

##### <a name="priority-items-to-review"></a>Elementos prioritarios que se van a revisar

El icono **Elementos prioritarios para revisar** muestra los elementos que puede que desee priorizar al iniciar la revisión. El icono muestra un recuento de elementos que pertenecen a las categorías siguientes:
- **Confidencial**: se trata de elementos que tienen aplicada una [etiqueta de confidencialidad de Microsoft](/microsoft-365/compliance/sensitivity-labels) . Por ejemplo, un documento de Word con una etiqueta "Extremadamente confidencial". 
- **Datos de varias personas**: estos elementos contienen los datos personales de más de una persona. Si desea incluir estos elementos como parte del paquete de datos final, deberá redactar los datos irrelevantes en los archivos. Consulte [Paso 3: Revisar los datos](#step-3-review-data) a continuación para obtener más información. Tenga en cuenta que, para que Priva identifique elementos con datos de varias personas, su organización debe configurar la [coincidencia de datos para las solicitudes de derechos del interesado](subject-rights-requests-data-match.md).

**Cómo localizar los elementos de prioridad:**

En primer lugar, asegúrese de que ha habilitado la vista de ellos en la tabla De datos **recopilados** de elementos siguiendo estos pasos:

- En la pestaña **Datos recopilados** , seleccione **Personalizar columnas** en la parte superior de la lista de elementos.
- En el panel flotante **Editar columnas** , coloque una comprobación junto a **Tipos de prioridad**.
- Seleccione **Aplicar**. La lista de elementos ahora tendrá una columna **Tipos de prioridad** .

Ahora puede identificar los elementos de prioridad y buscarlos mediante la ordenación de la columna **Tipo de prioridad** para agrupar tipos similares.

### <a name="understand-progress-stages"></a>Descripción de las fases de progreso

Las solicitudes de derechos del sujeto pasan por varias fases. Algunos estados progresan automáticamente y otras fases avanzan cuando los derechos del sujeto solicitan a los administradores y colaboradores que completen pasos esenciales, como revisar archivos.

Dado que es posible que las solicitudes deban ser trabajadas con el tiempo o por varios colaboradores, Priva proporciona actualizaciones continuas sobre el estado e instrucciones sobre los pasos siguientes que se deben seguir. Estas actualizaciones se pueden ver en la pestaña **Información general** de la página de detalles de una solicitud de derechos del sujeto.

#### <a name="data-estimate"></a>Estimación de datos
Una vez creada una solicitud, Priva comienza inmediatamente a buscar posibles coincidencias con el interesado en el entorno de Microsoft 365. Una vez que hayamos identificado todos los elementos que creemos que coinciden con sus criterios, verá la estimación en la tarjeta **Resumen de la estimación de datos** en la página **Información general** de la solicitud. La cantidad de datos dentro del ámbito de la búsqueda afectará al tiempo que tardará en completarse la estimación.

La solicitud se moverá automáticamente a la siguiente fase de recuperación de datos, donde todos los elementos de contenido se reúnen para que las partes interesadas puedan colaborar en la revisión de datos. En algunos casos, pausaremos la estimación de datos antes de pasar a la recuperación y le notificaremos los pasos siguientes que se deben seguir antes de continuar.

También puede optar por pausar automáticamente en la fase de estimación de datos cuando cree por primera vez una solicitud de derechos de sujeto. Durante el proceso de creación, seleccione la opción **Obtener una estimación en primer** lugar durante el paso **Buscar configuración** . Revise los detalles sobre el [paso de configuración de búsqueda](subject-rights-requests-create.md#define-search-settings).

#### <a name="pause-in-data-estimate-for-large-search-results"></a>Pausar en la estimación de datos para resultados de búsqueda grandes

Priva observará si la estimación de datos se proyecta para devolver un gran número de elementos que se van a revisar (más de 10 000 elementos). La estimación se pausará para que pueda obtener una vista previa de los resultados y decidir si [desea editar la consulta de búsqueda](subject-rights-requests-create.md#refine-your-search) para establecer como destino ubicaciones o condiciones más específicas, o bien continuar recuperando los elementos identificados.  Le mostraremos en pantalla el número de elementos y el volumen de datos que coinciden con la búsqueda. Tendrá una o ambas opciones en una barra de mensajes en la parte superior de la pantalla:

- Un botón **Editar consulta de búsqueda** le llevará directamente a la configuración de búsqueda de la solicitud para establecer parámetros más estrictos y generar una nueva estimación.
- Siempre que la consulta de búsqueda no supere los 300 000 elementos, también verá una opción para **Recuperar datos**. Esto le permite elegir no editar la búsqueda y seguir recopilando los datos.

#### <a name="retrieve-data"></a>Recuperar datos
La fase de recuperación de datos es cuando todos los archivos, correos electrónicos, chats, imágenes y otros elementos de contenido que contienen los datos personales del interesado se recuperan y se reúnen en un contenedor de Azure Blob Storage para su revisión. La recuperación de datos puede tardar unos minutos o mucho más en función del volumen de datos. Una vez completada esta fase, la solicitud se mueve automáticamente a la siguiente fase de **Revisar datos**.

#### <a name="review-data"></a>Revisar datos
 En esta fase, los colaboradores deben revisar los resultados en la pestaña **Datos recopilados** y realizar todas las tareas aplicables, como la censura, la aplicación de etiquetas y la adición de notas. Cuando haya terminado con la revisión, seleccione **Completar revisión**.

#### <a name="generate-reports"></a>Genere informes
Los informes se generan en esta fase. Cuando haya terminado, se pueden encontrar en la pestaña **Informes** . Los archivos terminados se pueden exportar para su revisión final y entrega al interesado que realizó la solicitud.

#### <a name="close-the-request"></a>Cerrar la solicitud
Una solicitud cerrada indica que se ha completado todo el trabajo para cumplir con esta solicitud de derechos de sujeto. Todos los datos recopilados e informes se conservarán según la [configuración de retención de datos](priva-settings.md#data-retention-periods).

## <a name="step-2-optional-view-and-edit-search-queries"></a>Paso 2 (opcional): Ver y editar consultas de búsqueda

Para ver información detallada sobre la búsqueda de datos detrás de una solicitud de derechos del interesado, seleccione **Ver detalles de la consulta de búsqueda**. Se abre un panel que resume la consulta y muestra más detalles sobre lo que se encontró.

Tiene la opción aquí para **obtener una vista previa de los resultados de la búsqueda** para ver qué tipo de contenido se devolverá para esta consulta. Si desea cambiar las propiedades de esta búsqueda y no ha iniciado la fase Recuperar datos, puede usar la opción **Editar consulta de búsqueda** .

El proceso guiado de edición de consultas de búsqueda permite cambiar o agregar propiedades para la identificación del interesado, los filtros y condiciones de búsqueda y las ubicaciones en las que buscar datos (incluidos Exchange, SharePoint, OneDrive o Teams). Use estas opciones para alcanzar el nivel de especificidad deseado. Puede revisar la versión final de la nueva consulta antes de presionar **Guardar**.

Cuando termine de editar la consulta de búsqueda, se ejecutará una nueva búsqueda para reemplazar los resultados de búsqueda anteriores. Esto restablece el estado de la sección **Progreso** al primer paso, **Estimación de datos**. La nueva búsqueda puede tardar hasta 60 minutos en completarse. Una vez hecho esto, verá los resultados actualizados en la página de detalles de la solicitud.

## <a name="step-3-review-data"></a>Paso 3: Revisión de datos

En esta fase, los colaboradores deben revisar los resultados en la pestaña **Datos recopilados**. Se configurará automáticamente un canal Teams para facilitar la revisión de contenido por parte de todas las partes interesadas. Consulte [Colaborar en la revisión de datos](#collaborate-on-data-review) para obtener más detalles. A continuación se describen las tareas esenciales para el paso de revisión de datos.

#### <a name="mark-items-as-include-or-exclude-and-add-notes"></a>Marcar elementos como Incluir o Excluir y agregar notas

Revise la lista de elementos identificados devueltos por la búsqueda. Si decide que el elemento debe incluirse como parte del informe final al interesado, seleccione **Incluir** en la barra de comandos de la parte superior de la lista de elementos. También puede seleccionar el botón **azul Incluir** en el área de revisión de contenido situada a la derecha de la lista de elementos. Al seleccionar **Incluir**, aparece un panel flotante con una opción para agregar notas. Cuando haya terminado, seleccione **Enviar** para guardar el estado de revisión del elemento como **Incluir**.

Si el elemento no pertenece como parte de la solicitud, seleccione **Excluir** en la barra de comandos o el botón **Excluir** del área de revisión de contenido. Excluir un elemento significa que no se incluirá en los [informes finales que se generan para el interesado](subject-rights-requests-reports.md).

> [!NOTE]
> Si marca un elemento como **Excluir**, debe agregar una nota como justificación para por qué no pertenece a la solicitud de derechos del sujeto. Las notas son para fines internos y no se incluyen en los informes finales.

Si el contenido parece ser un falso positivo, seleccione **No una coincidencia** y, en el panel flotante, seleccione **Confirmar**. Esta acción excluirá el archivo de los informes finales y marcará el elemento como algo que no debería haberse detectado en la búsqueda.

#### <a name="apply-tags"></a>Apply tags

Las etiquetas se pueden usar para ayudarle a identificar elementos que necesitan más atención. Priva proporciona tres etiquetas predeterminadas ( **Seguimiento**, **Eliminar** y **Actualizar** ) para las que puede establecer una descripción. Priva también proporciona dos etiquetas personalizadas que puede denominar y describir.

Por ejemplo, si determina durante la revisión de datos que su organización no necesita conservar un elemento de contenido, puede aplicar la etiqueta **Eliminar** y, a continuación, exportar una lista de todos los archivos etiquetados para que pueda volver atrás y eliminar los elementos identificados cuando haya terminado con la solicitud.

Las cinco etiquetas que administra en **Configuración** se aplican a todas las solicitudes de derechos del sujeto.

**Para agregar o quitar etiquetas:**

- Seleccione el elemento de la lista en la pestaña **Datos recopilados** de la solicitud.
- En el área de vista previa del elemento situada a la derecha de la lista, seleccione el botón **Aplicar etiquetas** en la fila inferior. También puede seleccionar los tres puntos situados a la derecha del nombre del elemento y seleccionar la opción **Aplicar etiquetas** .
- Aparece un panel flotante con la lista de etiquetas. Active la casilla situada junto a cualquiera de las etiquetas que desea aplicar al elemento. Si no se activa una casilla, se quitará la etiqueta.
- Cuando haya terminado, seleccione **Guardar**, que guarda las selecciones de etiqueta y cierra el panel flotante.

**Para agregar etiquetas personalizadas o actualizar descripciones de etiquetas:**
- En la página Solicitudes de derechos del sujeto, seleccione **Configuración** en la esquina superior derecha de la pantalla para acceder a la configuración de Priva.
- Vaya a la página **Etiquetas de revisión de datos** y seleccione la etiqueta para escribir una descripción y, para las etiquetas personalizadas, un nombre. Obtenga más información sobre [la configuración de etiquetas](priva-settings.md#data-review-tags).

**Para exportar una lista de elementos etiquetados:**
- Vaya a la página **Datos recopilados** en una solicitud de derechos del interesado.
- Encima de la lista de elementos, seleccione el icono de flecha abajo que indica **Exportar** al mantener el puntero sobre él.
- Se descargará un archivo Excel que muestra las propiedades de todos los elementos recopilados por la búsqueda de la solicitud. Busque la columna **Etiquetas** para identificar y ordenar los elementos por etiqueta.

#### <a name="use-the-annotate-command-to-redact-text"></a>Uso del comando Anotar para redactar texto
El comando **Anotar** del área de revisión de contenido permite crear marcas insertadas y redactar datos dentro de un elemento de contenido. Por ejemplo, si necesita incluir un archivo para una persona que también contenga la información personal de un interesado diferente, puede usar **la censura de área** en el botón Dibujo de la barra de comandos para desnegrecer toda la información que no pertenece a la persona que realizó la solicitud. Cuando se completen las modificaciones, seleccione **Incluir** para agregar el archivo redactado a la solicitud. La anotación crea una copia del archivo, que se almacena en el blob de Azure. El archivo original permanece inalterado y almacenado en su ubicación original.

#### <a name="enter-notes-about-a-file"></a>Escribir notas sobre un archivo
Para agregar o revisar notas en un elemento, seleccione el elemento de su fila y vaya a la pestaña **Notas** de archivo del área de revisión de contenido situada a la derecha. También puede usar la opción **Agregar nota de archivo** para crear un nuevo comentario. Para revisar o agregar notas en un nivel general de caso, vaya a la pestaña **notas** principal anterior y use **Agregar nota de caso**. Estas notas serán visibles para los usuarios que trabajan en la solicitud, pero no se incluirán en el informe final ni se compartirán con el interesado.

#### <a name="complete-the-review"></a>Completar la revisión

Cuando todos los elementos se han revisado y ha establecido su estado como **Incluir**, **Excluir** o **No una coincidencia,** es el momento de cerrar el paso de revisión seleccionando el botón  **Completar revisión** en la esquina superior derecha dentro de la solicitud. Un panel flotante mostrará un resumen de los datos y agregará las notas relacionadas. Estas notas son para mantener registros internos y no se comparten con el interesado.

Seleccione **Completar revisión** en el panel flotante para finalizar el paso de revisión. Los resúmenes de sus decisiones se proporcionarán más adelante en la pestaña **Informes** .

### <a name="collaborate-on-data-review"></a>Colaborar en la revisión de datos

Priva admite la colaboración a través de Microsoft Teams para permitir que el grupo trabaje juntos en las solicitudes de derechos de los sujetos. Al crear una nueva solicitud, se crea automáticamente un canal de Teams y se asocia a la solicitud de forma predeterminada. Aquí puede analizar la solicitud y compartir de forma segura entradas y contribuciones. Para unirse a la conversación, abra la solicitud y use la opción **Chatear con colaboradores** . Esto abrirá Microsoft Teams y lo colocará en el canal General para el sitio del equipo de la solicitud de derechos del sujeto.

Para revisar la lista de colaboradores activos que pueden ver y contribuir al sitio del equipo, en la solicitud de derechos del sujeto, abra la pestaña **Colaboradores** . Para agregar usuarios adicionales para colaborar en esta solicitud, seleccione la opción **Agregar un colaborador**.

Para cambiar el comportamiento predeterminado de generar sitios Teams al crear una solicitud de derechos de sujeto, vaya a **Configuración** en la navegación superior y seleccione **Teams colaboración** para modificar la configuración.

También puede usar la opción **Compartir** en la esquina superior derecha dentro de una solicitud de asunto derecho para hacer un bucle a las personas a través de Teams o correo electrónico, o para copiar el vínculo a la página en Priva. Compartir a través de Teams le permite seleccionar un sitio Teams existente y un canal disponible para su cuenta, donde publicará un vínculo a este caso junto con cualquier mensaje que proporcione.

## <a name="step-4-close-the-request"></a>Paso 4: Cerrar la solicitud

Cuando haya realizado todas las acciones necesarias para resolver la solicitud de derechos del firmante, seleccione **Cerrar la solicitud**. Esto crea el informe final, que se puede encontrar en la **pestaña Informes**. La finalización puede tardar un tiempo en función del número de archivos de la solicitud.

## <a name="next-steps"></a>Siguientes pasos
Para obtener más información sobre cómo trabajar con informes y completar solicitudes de derechos del sujeto, consulte [Generación de informes y cumplimiento de una solicitud de derechos de sujeto](subject-rights-requests-reports.md).

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legal

[Declinación de responsabilidades legal de Microsoft Priva](priva-disclaimer.md)
