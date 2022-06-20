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
ms.openlocfilehash: 6120fdaa97cf79ac122f6992f9ce476fdc4c5da3
ms.sourcegitcommit: 8cbafebb1a1b26a0bd92e500a1e6d6c60243c64b
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/20/2022
ms.locfileid: "66166649"
---
# <a name="review-data-for-a-subject-rights-request"></a>Revisión de los datos de una solicitud de derechos del interesado

**En este artículo**: obtenga información sobre cómo revisar los datos recopilados para una solicitud de derechos del interesado mediante herramientas de censura y etiquetas de archivo. Comprenda cómo usar la funcionalidad de colaboración, que incluye un canal de Teams dedicado.

Una vez recopilados los datos de una solicitud de derechos del interesado, la siguiente fase es revisar los elementos de contenido, decidir qué elementos incluir o excluir como parte de la solicitud y redactar la información si es necesario.

## <a name="tasks-for-completing-the-data-review"></a>Tareas para completar la revisión de datos

La fase **Revisar datos** es cuando los colaboradores examinan los elementos de contenido en la pestaña **Datos recopilados**. Se configurará automáticamente un canal Teams para facilitar la revisión de contenido por parte de todas las partes interesadas. Consulte [Colaboración para la revisión de datos](#collaboration-for-data-review) a continuación para obtener más detalles. A continuación se describen las tareas esenciales para el paso de revisión de datos.

#### <a name="import-additional-files"></a>Importación de archivos adicionales

Es posible que desee incluir elementos de contenido adicionales en la solicitud de revisión de datos. Por ejemplo, los archivos almacenados fuera del entorno de Microsoft 365 de la organización u otros elementos que considere pertinentes pero que no se han limitado en la búsqueda. Puede importar archivos en la pestaña **Datos recopilados** de una solicitud individual en la que se va a revisar y trabajar, junto con los demás elementos. Los archivos importados se agregan al mismo contenedor Azure Blob Storage con los demás elementos de contenido recuperados de la búsqueda.

Siga los pasos siguientes para importar archivos:

1. En la página de detalles de la solicitud, seleccione **Importar archivos** en la barra de comandos de la parte superior de la página.

2.  Aparecerá un cuadro **Importar archivos** en la pantalla. Seleccione **Elegir archivos** y, en la vista del explorador de archivos, elija uno o varios archivos para importar.

3. Volverá al cuadro **Importar archivos** , que enumera los archivos que eligió. Puede seleccionar **Elegir archivos** de nuevo para agregar más elementos a la lista. Para quitar cualquiera de los archivos, seleccione **Borrar**, que quita todos los archivos y elija archivos de nuevo.

4. Cuando todos los archivos deseados aparezcan en el cuadro **Importar archivos** , seleccione **Importar**. Para salir sin cargar, seleccione **Cancelar importación**.

Cuando comience la importación, volverá a la pestaña **Datos recopilados** de la solicitud. Un mensaje situado encima de la pestaña indica que la carga está en curso. Si hay un problema con la carga, el mensaje le indicará y proporcionará una opción para volver a intentarlo.

Verá un mensaje de confirmación encima de la pestaña **Datos recopilados** cuando se complete la importación.

**Más detalles sobre la importación de archivos:**

- El tamaño de archivo individual no puede superar los 4 MB. Verá un mensaje de advertencia en el cuadro **Importar archivos** cuando un archivo sea demasiado grande para cargarlo.

- Los archivos importados pueden tardar hasta 20 minutos en estar disponibles en la pestaña **Datos recopilados** .

- Si ya hay una importación en curso para un usuario, el mismo usuario no podrá cargar archivos adicionales hasta que finalice el proceso de carga anterior. Varios usuarios pueden cargar archivos en la misma solicitud simultáneamente. Sin embargo, cuantos más cargas estén en curso, más tiempo tardarán en completarse. Los mensajes de estado de la solicitud informarán cuando haya finalizado una carga y los archivos estén listos para revisarse.

#### <a name="mark-items-as-include-or-exclude-and-add-notes"></a>Marcar elementos como Incluir o Excluir y agregar notas

Revise los elementos enumerados en la pestaña **Datos recopilados** de la solicitud.  Si decide que el elemento debe incluirse como parte del informe final al interesado, seleccione **Incluir** en la barra de comandos de la parte superior de la lista de elementos. También puede seleccionar el botón **azul Incluir** en el área de revisión de contenido situada a la derecha de la lista de elementos. Al seleccionar **Incluir**, aparece un panel flotante con una opción para agregar notas. Cuando haya terminado, seleccione **Enviar** para guardar el estado de revisión del elemento como **Incluir**.

Si el elemento no pertenece como parte de la solicitud, puede seleccionar **Excluir** en la barra de comandos o el botón **Excluir** del área de revisión de contenido. Marcar un elemento explícitamente como **Excluir** suele ser necesario para los registros internos.

De forma predeterminada, solo los elementos que marque como **Incluir** se incluirán en los [informes finales que se generan para el interesado](subject-rights-requests-reports.md).

> [!NOTE]
> Si marca un elemento como **Excluir**, debe agregar una nota como justificación para por qué no pertenece a la solicitud de derechos del sujeto. Las notas son para fines internos y no se incluyen en los informes finales.

Si el contenido parece ser un falso positivo para la consulta de búsqueda, seleccione **No una coincidencia** y, en el panel flotante, seleccione **Confirmar**. Esta acción marcará el elemento como algo que no debería haberse detectado en la búsqueda.

#### <a name="apply-tags"></a>Apply tags

Las etiquetas se pueden usar para ayudarle a identificar elementos que necesitan más atención. Priva proporciona tres etiquetas predeterminadas (**seguimiento**, **eliminación** y **actualización**) para las que puede establecer una descripción. Priva también proporciona dos etiquetas personalizadas que puede asignar un nombre y describir.

Por ejemplo, si determina durante la revisión de datos que su organización no necesita conservar un elemento de contenido, puede aplicar la etiqueta **Eliminar** y, a continuación, exportar una lista de todos los archivos etiquetados para que pueda volver atrás y eliminar los elementos identificados cuando haya terminado con la solicitud.

Las cinco etiquetas que administra en **Configuración** se aplican a todas las solicitudes de derechos del sujeto.

**Para agregar o quitar etiquetas:**

- Seleccione el elemento de la lista en la pestaña **Datos recopilados** de la solicitud.
- En el área de vista previa del elemento situada a la derecha de la lista, seleccione el botón **Aplicar etiquetas** en la fila inferior. También puede seleccionar los tres puntos situados a la derecha del nombre del elemento y seleccionar la opción **Aplicar etiquetas** .
- Aparece un panel flotante con la lista de etiquetas. Active la casilla situada junto a cualquiera de las etiquetas que desea aplicar al elemento. Al desactivar una casilla, se quitará la etiqueta.
- Cuando haya terminado, seleccione **Guardar**, que guarda las selecciones de etiqueta y cierra el panel flotante.

**Para agregar etiquetas personalizadas o actualizar descripciones de etiquetas:**
- En la página Solicitudes de derechos del sujeto, seleccione **Configuración** en la esquina superior derecha de la pantalla para acceder a la configuración de Priva.
- Vaya a la página **Etiquetas de revisión de datos** y seleccione la etiqueta para escribir una descripción y, para las etiquetas personalizadas, un nombre. Obtenga más información sobre [la configuración de etiquetas](priva-settings.md#data-review-tags).

**Para exportar una lista de elementos etiquetados:**
- Vaya a la página **Datos recopilados** en una solicitud de derechos del interesado.
- Encima de la lista de elementos, seleccione el comando **Exportar** .
- Se descargará un archivo Excel que muestra las propiedades de todos los elementos recopilados por la búsqueda de la solicitud. Busque la columna **Etiquetas** para identificar y ordenar los elementos por etiqueta.

#### <a name="use-the-annotate-command-to-redact-text"></a>Uso del comando Anotar para redactar texto
El comando **Anotar** del área de revisión de contenido permite crear marcas insertadas y redactar datos dentro de un elemento de contenido. Por ejemplo, si necesita incluir un archivo para una persona que también contenga la información personal de un interesado diferente, puede usar **la censura de área** en el botón Dibujo de la barra de comandos para desnegrecer toda la información que no pertenece a la persona que realizó la solicitud. Cuando se completen las modificaciones, seleccione **Incluir** para agregar el archivo redactado a la solicitud. La anotación crea una copia del archivo, que se almacena en el blob de Azure. El archivo original permanece inalterado y almacenado en su ubicación original.

#### <a name="enter-notes-about-a-file"></a>Escribir notas sobre un archivo
Para agregar o revisar notas en un elemento, seleccione el elemento de su fila y vaya a la pestaña **Notas** de archivo del área de revisión de contenido situada a la derecha. También puede usar la opción **Agregar nota de archivo** para crear un nuevo comentario. Para revisar o agregar notas en un nivel general de caso, vaya a la pestaña **notas** principal anterior y use **Agregar nota de caso**. Estas notas serán visibles para los usuarios que trabajan en la solicitud, pero no se incluirán en el informe final ni se compartirán con el interesado.

## <a name="collaboration-for-data-review"></a>Colaboración para la revisión de datos

Los administradores de solicitudes de derechos del firmante pueden ver todas las solicitudes. Puede agregar otros usuarios para colaborar en una solicitud, lo que les dará acceso para ver esa solicitud y trabajar con los datos recopilados en ella para ayudar a mover la solicitud a la finalización.

Al crear una solicitud, se crea automáticamente un canal de Teams dedicado para que las partes interesadas analicen la solicitud y compartan de forma segura entradas y contribuciones. La pestaña **Colaboradores** de la página de detalles de la solicitud muestra todos los colaboradores que pueden ver y contribuir a la solicitud y a cualquier canal Teams asociado.

Para agregar más colaboradores, seleccione **Agregar colaborador**, empiece a escribir el nombre del usuario, seleccione el nombre una vez que aparezca y, a continuación, seleccione **Agregar**.

Para iniciar un chat Teams, cualquier colaborador puede seleccionar **Chatear con colaboradores** en la esquina superior derecha de la página de detalles de la solicitud. Esta acción abre Teams y le coloca en el canal **General** para el sitio de equipo de la solicitud de derechos del sujeto.

Para cambiar el comportamiento predeterminado de la creación de canales de Teams para solicitudes de derechos de sujeto, vaya a Priva **Configuración** en la esquina superior derecha de Subject Rights Request. Seleccione **Teams colaboración** y desactive la casilla de la página para desactivar Teams funcionalidades para todas las solicitudes de derechos del sujeto.

El comando **Compartir** de la esquina superior derecha de la página de detalles de una solicitud crea un vínculo que se puede compartir que va directamente a la solicitud en Priva. Proporcione este vínculo a los colaboradores para que puedan acceder a la solicitud a la que los ha agregado.

## <a name="complete-the-review"></a>Completar la revisión

Cuando todos los elementos se han revisado y ha establecido su estado como **Incluir**, **Excluir** o **No una coincidencia,** es el momento de cerrar el paso de revisión. Cualquiera de los colaboradores de una solicitud puede completar la revisión.

Seleccione el botón **Completar revisión** en la esquina superior derecha de la solicitud. Un panel flotante mostrará un resumen de los datos y agregará las notas relacionadas. Estas notas son para mantener registros internos y no se comparten con el interesado.

Seleccione **Completar revisión** en el panel flotante para finalizar el paso de revisión. Esta acción prepara la solicitud para las fases finales del proceso: generar informes y cerrar la solicitud. Los resúmenes de sus decisiones se proporcionarán más adelante en la pestaña **Informes** .

## <a name="next-steps"></a>Pasos siguientes
Obtenga información sobre cómo generar el informe final y trabajar para completar la solicitud en [Generar informes y cerrar una solicitud](subject-rights-requests-reports.md).

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legal

[Microsoft Priva declinación de responsabilidades legal](priva-disclaimer.md)
