---
title: Establecimiento de permisos de usuario y asignación de roles en Microsoft Priva
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
- M365-priva-subject-rights-requests
search.appverid:
- MOE150
- MET150
description: Obtenga información sobre cómo configurar permisos de Microsoft Priva y asignar usuarios a grupos de roles.
ms.openlocfilehash: 14ae1b1b9ee1f1ccc8d3a1914f0d7308a8467f23
ms.sourcegitcommit: 09ecdaded9a9f8f79587f2acb978dc53b83e5c01
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/19/2022
ms.locfileid: "64930621"
---
# <a name="set-user-permissions-and-assign-roles-in-microsoft-priva"></a>Establecimiento de permisos de usuario y asignación de roles en Microsoft Priva

Para conceder a los miembros de la organización permisos para usar Microsoft Priva, asígnelos a los grupos de roles adecuados en el portal de cumplimiento de Microsoft Purview.

> [!NOTE]
> La mayoría de los roles Priva se designan actualmente como "administración de privacidad". Consulte a continuación para obtener una lista completa. Los roles específicos de Priva no aparecerán en Azure Active Directory.

## <a name="sign-in-and-set-permissions"></a>Inicio de sesión y establecimiento de permisos

1. Vaya al [portal de cumplimiento de Microsoft Purview](https://compliance.microsoft.com/) y seleccione **Permisos** en el panel de navegación izquierdo.  
2. En la lista desplegable **Centro de cumplimiento** , seleccione **Roles**. Aparecerá la lista completa de grupos de roles.
3. Busque el grupo de roles al que desea agregar uno o varios usuarios y active la casilla situada a la izquierda del nombre del grupo.
4. En el panel flotante de ese grupo, seleccione **Editar** en el encabezado **Miembros** .  
5. Seleccione **Elegir miembros**. Aparecerá otra ventana flotante.
6. Seleccione **+ Agregar** para elegir uno o varios usuarios para agregar al grupo.  
7. Seleccione la casilla situada junto a los nombres que desea agregar y, a continuación, seleccione el botón **Agregar** en la parte inferior.  
8. Cuando haya terminado de asignar usuarios, seleccione **Listo**, **Guardar** y **Cerrar**.

## <a name="learn-more-about-role-groups-and-roles"></a>Más información sobre los grupos de roles y los roles

En función de la estructura del equipo, tiene opciones para asignar usuarios a grupos de roles específicos para administrar diferentes conjuntos de características priva. Los miembros deben asignarse a grupos de roles en función de las tareas que necesiten realizar y del nivel de acceso a archivos adecuado. Cada grupo de roles incluye uno o varios roles. Estos roles pueden pertenecer a tareas priva específicas o funciones clave habilitadas o restringidas para los miembros de ese grupo. Por lo tanto, los distintos usuarios pueden tener diferentes niveles de visibilidad y acceso a determinadas características priva.

Los grupos de roles se pueden personalizar si es necesario. Para evitar la pérdida accidental de acceso, se recomienda crear una copia del grupo de roles existente que desea personalizar, dar a la copia un nombre identificable, realizar y comprobar los cambios en el nuevo grupo y asignarle personas según corresponda.

## <a name="privacy-management-role-group"></a>Grupo de roles de administración de privacidad

Este grupo contiene todos los roles de permiso Priva en un solo grupo. Este grupo de roles puede ser una buena opción para las organizaciones en las que la misma persona puede realizar todas las tareas. Al proporcionar la pertenencia a este grupo de roles, se concederá a esa cuenta acceso total a todas las características de Priva para las que tenga una licencia.

Se recomienda asegurarse de que siempre haya al menos un miembro activo de este grupo.

Los roles incluyen:

- Administración de casos  
- Visor de contenido de clasificación de datos  
- Visor de lista de clasificación de datos  
- Administrador de administración de privacidad  
- Análisis de administración de privacidad  
- Investigación de administración de privacidad  
- Contribución permanente a la administración de la privacidad  
- Contribución temporal a la administración de la privacidad  
- Visor de administración de privacidad  
- Administrador de solicitudes de derechos de sujeto  
- caso View-Only

## <a name="privacy-management-administrators-role-group"></a>Grupo de roles Administradores de administración de privacidad

Los miembros de este grupo de roles tienen un amplio acceso a las funciones Priva, incluida la creación, lectura, actualización y eliminación de directivas de administración de riesgos de privacidad, solicitudes de derechos del sujeto, permisos y configuración.

Los roles incluyen:

- Administración de casos  
- Administrador de administración de privacidad  
- caso View-Only

## <a name="privacy-management-analysts-role-group"></a>Grupo de roles Analistas de administración de privacidad

Los miembros de este grupo de roles actúan como analistas de casos. Pueden investigar las coincidencias de directivas, ver los metadatos de los archivos y realizar acciones de corrección. Este grupo no puede acceder a los archivos completos a través del Explorador de contenido.

Los roles incluyen:

- Administración de casos  
- Visor de lista de clasificación de datos  
- Análisis de administración de privacidad  
- caso View-Only

### <a name="privacy-management-investigators-role-group"></a>Grupo de roles Investigadores de administración de privacidad

Los miembros de este grupo actúan como investigadores de datos. Pueden investigar las coincidencias de directivas, ver el contenido del archivo asociado y realizar acciones de corrección. Este grupo puede acceder a los archivos a través del Explorador de contenido.

Los roles incluyen:

- Administración de casos  
- Visor de contenido de clasificación de datos  
- Visor de lista de clasificación de datos  
- Investigación de administración de privacidad  
- caso View-Only

## <a name="privacy-management-viewer-role-group"></a>Grupo de roles Visor de administración de privacidad

Los miembros de este grupo pueden ver información analítica en Priva, como la información general, el perfil de datos y los informes de solicitudes del interesado.

Los roles incluyen:

- Visor de administración de privacidad

## <a name="subject-rights-request-administrators-role-group"></a>Grupo de roles Administradores de solicitudes de derechos del firmante

Los miembros de este grupo tienen acceso total para administrar y crear solicitudes de derechos del sujeto.

Los roles incluyen:

- Administrador de solicitudes de derechos de sujeto

## <a name="privacy-management-contributors-role-group"></a>Grupo de roles Colaboradores de administración de privacidad

Los miembros de este grupo tienen acceso a las solicitudes de derechos del sujeto para las que se han agregado como colaboradores.  

Los roles incluyen:

- Contribución temporal a la administración de la privacidad  
- Contribución permanente a la administración de la privacidad

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legal

[Declinación de responsabilidades legal de Microsoft Priva](priva-disclaimer.md)