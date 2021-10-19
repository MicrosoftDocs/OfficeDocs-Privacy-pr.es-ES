---
title: Buscar y visualizar datos personales en la administración de privacidad
f1.keywords:
- CSH
ms.author: v-jgriffee
author: jmgriffee
manager: laurawi
audience: Admin
ms.topic: article
ms.service: O365-seccomp
ms.localizationpriority: medium
ms.collection:
- M365-security-compliance
- M365-privacy-management
search.appverid:
- MOE150
- MET150
description: Obtenga información sobre la información general y el perfil de datos en la administración de privacidad y cómo obtener información sobre los datos personales en el entorno Microsoft 365 organización.
ms.openlocfilehash: 119dc0d3649abd35c03ea5bdfe40f7967a0d2c9d
ms.sourcegitcommit: 85e085eb17af8b4efd1f45207445e1b3c3679600
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/19/2021
ms.locfileid: "60478384"
---
# <a name="find-and-visualize-personal-data-in-privacy-management"></a>Buscar y visualizar datos personales en la administración de privacidad

La administración de privacidad le ayuda a comprender los datos que almacena su organización automatizando el descubrimiento de activos de datos personales y proporcionando visualizaciones de información esencial. Estas visualizaciones se pueden encontrar en las **páginas de información general** y perfil **de** datos. Puede actuar según los conocimientos aquí para reforzar la posición de privacidad de su organización y reducir el riesgo.

Para empezar, vaya a la sección de administración de privacidad de [la Centro de cumplimiento de Microsoft 365](https://compliance.microsoft.com/) y vea estas páginas:

- **Información** general: proporciona una vista general de los datos de la organización en Microsoft 365. Los administradores de privacidad pueden supervisar tendencias y actividades, identificar e investigar posibles riesgos relacionados con datos personales y participar en actividades clave como la administración de directivas o las acciones de solicitud de derechos de sujeto.
- **Perfil de** datos: proporciona una instantánea de los datos personales que la organización almacena en Microsoft 365. Esta página le ayuda a visualizar dónde se encuentran los datos personales, qué tipos son los más frecuentes en su organización y cuántos tipos diferentes existen en todas las ubicaciones del entorno Microsoft 365 usuario. También puede explorar datos personales desde esta ubicación.

A medida que los cambios de datos y la administración de privacidad realicen nuevos hallazgos, se actualizará la información que se muestra en estas páginas. Tenga en cuenta que los nuevos datos pueden tardar hasta 24 horas en representarse en los gráficos.

## <a name="explore-the-overview-page"></a>Explorar la página de información general

La página de información general consta de tres secciones principales. Los iconos de la parte superior de la página proporcionan estadísticas recientes esenciales sobre los datos. La sección de información clave proporciona oportunidades de investigación sobre tendencias y áreas de interés clave. Para obtener más perspectiva sobre el entorno de datos, consulte los gráficos de línea de tendencia. Para obtener más información sobre estas áreas, consulte las secciones siguientes.

![Página de información general de ejemplo.](../../media/privacy-management-overview.png)

### <a name="top-tiles"></a>Iconos superiores

#### <a name="policy-matches-over-past-7-days"></a>Coincidencias de directivas en los últimos 7 días

Cuando las directivas se establecen dentro de la administración de privacidad, los datos se evaluarán en función de las directivas para determinadas condiciones que pueden presentar riesgos de privacidad. Las coincidencias de directiva indican descubrimientos de datos que pueden necesitar más revisión o corrección. Este icono muestra cuántas coincidencias de directiva se han producido en los últimos siete días. Las coincidencias se mostrarán aquí si las directivas están activadas o se están ejecutando en modo de prueba, para que puedas ver los resultados de todas las directivas activas. La selección de este icono te llevará  a una vista filtrada de la página Directivas de administración de privacidad, que muestra las directivas que han tenido una coincidencia en los últimos siete días.

#### <a name="items-with-personal-data"></a>Elementos con datos personales

Para ver las funciones de detección automatizada de la solución de administración de privacidad en el trabajo, revise el **icono Elementos con datos** personales. Este icono muestra cuántos elementos nuevos que contienen datos personales basados en la configuración se han detectado en el entorno Microsoft 365 de la organización en los últimos siete días. Al seleccionar este icono, se cargará una vista de los 100 elementos más nuevos detectados.

#### <a name="subject-rights-requests"></a>Solicitudes de derechos de sujeto

La página de información general incluye un icono que muestra cuántas solicitudes de derechos de sujeto se han creado en los últimos siete días. Un segundo icono, si procede, muestra cuántas solicitudes están vencidas en función de las fechas límite designadas y puede que necesite atención inmediata. La selección de estos iconos llevará a los usuarios con los permisos adecuados a la página de solicitud de derechos del sujeto de la administración de privacidad.

### <a name="key-insights"></a>Información clave

#### <a name="content-items-with-the-most-personal-data"></a>Elementos de contenido con los datos más personales

El contenido que contiene una gran cantidad de datos personales puede presentar un mayor riesgo de exposición. Es posible que desee revisar estos elementos para asegurarse de que están cubiertos por una directiva de administración de privacidad. Para ayudar a llamar la atención sobre estos elementos, la página de información general proporciona una vista de los elementos de contenido que contienen los datos más personales según la configuración. Aquí puede ver el número de tipos de datos personales únicos detectados, cuántos propietarios de contenido únicos se han identificado y cuántos interesados se han identificado de acuerdo con la configuración de coincidencia de datos para solicitudes de derechos del sujeto.

Seleccione **Ver resumen para** obtener una vista resumida de los elementos encontrados. También puede elegir explorar estos **resultados** para obtener una vista previa de los archivos individuales. Esta vista muestra un máximo de 100 elementos. Los usuarios del grupo de roles Administración de privacidad pueden seleccionar archivos para revisar detalles y determinar la relevancia, y exportar la lista en .csv formato de referencia.

#### <a name="policies-with-the-most-matches-in-the-last-week"></a>Directivas con más coincidencias en la última semana

Esta información muestra qué directivas se han emparejado con más frecuencia en los últimos siete días, ya sea en modo "On" o "Testing". Ayuda a ilustrar el rendimiento de las directivas y los efectos del trabajo en curso a medida que los usuarios de administración de privacidad refinan sus comportamientos de privacidad.

Seleccione **Ver resumen para** obtener un resumen de las 10 directivas principales coincidentes y los propietarios de contenido del contenido asociado. También verá cuántas notificaciones de usuario se enviaron debido a estas coincidencias de directiva y el número de acciones de usuario realizadas. Seleccione **Investigar** para ver la página directivas en la administración de privacidad, filtrada para mostrar las directivas desde la vista de resumen. Esta vista de investigación mostrará estadísticas de toda la vigencia de la directiva. Selecciónelo para ver detalles como cuándo se detectaron inicialmente elementos coincidentes.

#### <a name="users-with-the-most-policy-matched-in-the-last-week"></a>Usuarios con la directiva más coincidente en la última semana

Esta información también aborda las coincidencias de las directivas en modo "Prueba" o "On". Le permite ver un resumen de los usuarios con más coincidencias de directiva en la última semana y qué directivas coinciden. Esto incluye totales de los propietarios de contenido únicos, las notificaciones enviadas a estos usuarios y cuántas acciones se realizaron desde esas notificaciones. Si selecciona **Investigar,** se le llevará a la página directivas, filtrada para mostrar las directivas desde la vista de resumen. En la vista de investigación, no encontrará información del usuario, pero puede seleccionar una directiva para ver los detalles de la directiva relacionados con estas coincidencias.

#### <a name="items-with-the-most-data-subject-content"></a>Elementos con más contenido del interesado

Esta información hace referencia a la información de la característica de coincidencia de datos en solicitudes de derechos de sujeto y presenta elementos de contenido detectados en Microsoft 365 que contienen la mayoría de los interesados. Para obtener más información acerca de esta configuración, vea [Administrar solicitudes de derechos de sujeto](privacy-management-subject-rights-requests.md).

Estos elementos pueden ayudar a confirmar la configuración de coincidencia de datos y ayudarle a mitigar los riesgos de privacidad relacionados con estos elementos. Seleccione **Ver resumen para** una vista de resumen. Seleccione **Explorar** para obtener una vista detallada de hasta 100 de estos elementos. Aquí puede obtener una vista previa de estos elementos y determinar la relevancia y exportar la lista en .csv formato.

### <a name="trendline-graphs"></a>Gráficos de línea de tendencia

Para ver las visualizaciones dinámicas de las tendencias encontradas en los datos de la organización, consulte los gráficos de línea de tendencia. Estos gráficos se pueden filtrar por características como intervalos de tiempo, tipo de datos o ubicaciones de datos. Usa los desplegables proporcionados para ajustar la vista. Mantener el mouse sobre las líneas del gráfico te permitirá ver estadísticas relacionadas con ese punto específico en el tiempo.

Los resultados relacionados con las directivas incluirán datos de directivas en modo "Prueba" y "On". Si no hay directivas de un tipo determinado activas, los gráficos relacionados no mostrarán resultados.

#### <a name="active-policy-alerts"></a>Alertas de directivas activas

Esta área muestra una instantánea de alertas activas desencadenadas por coincidencias de directiva. Con el tiempo, esta vista puede ayudarle a detectar más fácilmente anomalías como picos grandes de volumen. Seleccione **Ver alertas** para navegar a la página directivas de la administración de privacidad, donde puede investigar más a fondo las alertas y crear problemas para la corrección.

#### <a name="personal-data-found-in-organization"></a>Datos personales encontrados en la organización

Este gráfico muestra tendencias en la cantidad de datos personales que coinciden con la configuración que se ha detectado con el tiempo en el entorno Microsoft 365 y dónde se encuentra. Empezará a rellenarse después de que la administración de privacidad se haya estado ejecutando durante suficiente tiempo y después de que se haya encontrado contenido con datos personales en SharePoint, OneDrive, Teams y/o Exchange.

#### <a name="data-transfers-detected-in-organization"></a>Transferencias de datos detectadas en la organización

Este gráfico está relacionado con las directivas de transferencia de datos. Proporciona una vista de cómo se mueven los datos dentro de la organización, ya sea entre departamentos o entre regiones para organizaciones multige geográficas.

#### <a name="unused-personal-data"></a>Datos personales sin usar

Este gráfico está relacionado con las directivas de minimización de datos. Proporciona información sobre cómo su organización almacena contenido que contiene datos personales y cómo las directivas pueden mejorar el tratamiento de estos datos con el tiempo.

#### <a name="overexposed-personal-data"></a>Datos personales sobreexpuestos

Este gráfico está relacionado con directivas de sobreexposición de datos. Puede ayudarle a identificar comportamientos de uso compartido a lo largo del tiempo dentro de su organización y ubicaciones en las que el contenido con datos personales puede estar sobreexpuesto, por ejemplo, si se comparte públicamente, se comparte con un usuario externo o se comparte ampliamente dentro de la organización.

#### <a name="subject-rights-requests-by-regulation"></a>Solicitudes de derechos de sujeto por reglamento

Esta vista proporciona información sobre las normativas que más impulsan las solicitudes de derechos de sujeto con el tiempo. La leyenda de este gráfico muestra los nombres de las normativas de tendencias. Si se mantiene el mouse sobre las líneas de tendencia, se mostrarán los totales de solicitudes de derechos de sujeto abiertas para dicho reglamento durante el tiempo seleccionado.

#### <a name="subject-rights-requests-by-status"></a>Solicitudes de derechos de sujeto por estado

En este gráfico se muestra cómo está su organización completando solicitudes de derechos de sujeto, divididas en solicitudes que son **Active**, **Closed** o **Overdue**. Los resultados aquí pueden ayudar a indicar dónde podría beneficiarse de la asignación de más recursos para cerrar sus solicitudes y objetivos de reunión.

### <a name="additional-data-views"></a>Vistas de datos adicionales

#### <a name="subject-rights-requests-at-a-glance"></a>Solicitudes de derechos de sujeto de un vistazo

Esta vista proporciona una vista de alto nivel de las solicitudes de derechos de sujeto activas, incluido el tiempo restante para completar las solicitudes en sus fechas límite. Resume cuántas solicitudes totales tiene, cuántas están activas y cuántas están cerradas. Seleccione **Ver todas las** solicitudes para ir a la página solicitud de derechos del sujeto, donde puede ver más detalles y trabajar en las solicitudes activas para avanzar hacia su finalización.

#### <a name="subject-rights-requests-by-residency"></a>Solicitudes de derechos de sujeto por residencia

Esta vista de mapa le ayuda a visualizar el volumen de solicitudes de derechos de sujeto por la residencia de los interesados. Al pasar el puntero sobre una burbuja se identificará la región y el total de solicitudes de derechos de sujeto abiertas en nombre de los residentes allí.

## <a name="explore-the-data-profile-page"></a>Explorar la página de perfil de datos

La página de perfiles de datos de la administración de privacidad proporciona una vista instantánea de los datos personales que la organización almacena en Microsoft 365 y dónde se encuentra. También proporciona información sobre los tipos de datos que almacena. Los iconos principales incluyen lo siguiente.

![Página de perfil de datos de ejemplo.](../../media/privacy-management-dataprofile.png)

### <a name="personal-data-type-instances-detected-in-microsoft-365"></a>Instancias de tipo de datos personales detectadas en Microsoft 365

Este icono le ayuda a visualizar la cantidad de datos personales que existen en el entorno de Microsoft 365 en función de su configuración y de cómo se distribuyen los datos entre Exchange, OneDrive, SharePoint y Teams.

El gráfico de barras muestra el recuento agregado aproximado de instancias de tipo de datos personales únicos que se encuentran en el contenido. Algunos ejemplos de tipos de datos pueden incluir elementos como números de tarjeta de crédito y números de seguridad social. Por lo tanto, un archivo detectado que contiene tres números de tarjeta de crédito y un número de seguridad social contendrá dos tipos de datos personales únicos y cuatro instancias. La parte inferior de este icono muestra los tipos de datos personales únicos dentro de cada Microsoft 365 ubicación. Proporciona una vista de la diversidad de tipos de datos personales detectados en el contenido de la organización.

### <a name="top-personal-data-types-across-your-organization"></a>Tipos de datos personales principales en toda la organización

Este icono proporciona una instantánea de los tipos de datos personales principales detectados en el entorno, junto con información sobre cuántos elementos contienen ese tipo de datos personales y en qué ubicaciones.

### <a name="personal-data-type-instances-by-region"></a>Instancias de tipo de datos personales por región

Para entornos multige geográficos, este icono agrega regionalmente instancias de tipo de datos personales que se encuentran en el contenido, en función de las regiones en las que se hospeda este contenido. Para las organizaciones de una sola región, este icono mostrará un punto que representa Microsoft 365 ubicación. Si se mantiene el mouse sobre puntos en el mapa, se mostrará el recuento aproximado de instancias de tipo de datos personales detectadas en esa región.

### <a name="exploring-content"></a>Explorar contenido

Si selecciona **Explorar** en cualquier icono de perfil de datos, se abrirá el explorador de contenido. En este momento, no puede buscar un elemento de contenido específico y no verá Teams datos en esta vista. Esto significa que es posible que los números del explorador de contenido no coincidan con los números que se muestran en la página de perfil de datos, ya que la página de perfil de datos incluye Teams contenido. Los administradores de privacidad que desean obtener más información sobre sus datos de privacidad pueden hacerlo aquí en función del tipo de datos personales (tipo de información confidencial) o por ubicación (Exchange, OneDrive o SharePoint).

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legales

[Declinación de responsabilidades legales de administración de privacidad](privacy-management-disclaimer.md)
