---
title: Establecer permisos de usuario y asignar roles en Microsoft Priva
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
description: Obtenga información sobre cómo configurar los permisos de Microsoft Priva y asignar usuarios a grupos de roles.
ms.openlocfilehash: bcc2e108f10e427e55034621f2f8b5c40e6d9184
ms.sourcegitcommit: f145dff5e387a8e26db2f3a2c7de125978fbacc9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/28/2022
ms.locfileid: "62249105"
---
# <a name="set-user-permissions-and-assign-roles-in-microsoft-priva"></a>Establecer permisos de usuario y asignar roles en Microsoft Priva

Para conceder a los miembros de la organización permisos para usar Microsoft Priva, asígnelos a los grupos de roles adecuados en el Centro de cumplimiento de Microsoft 365.

> [!NOTE]
> La mayoría de los roles Priva se designan actualmente como "administración de privacidad". Vea a continuación una lista completa. Los roles específicos de Priva no aparecerán en Azure Active Directory.

## <a name="sign-in-and-set-permissions"></a>Iniciar sesión y establecer permisos

1. Vaya a la [Centro de cumplimiento de Microsoft 365](https://compliance.microsoft.com/) y seleccione **Permisos en** la navegación izquierda.  
2. En la lista **desplegable Centro de** cumplimiento, seleccione **Roles**. Aparecerá la lista completa de grupos de roles.
3. Busque el grupo de roles al que desea agregar uno o varios usuarios y active la casilla a la izquierda del nombre del grupo.
4. En el panel desplegable de ese grupo, seleccione **Editar en** el **encabezado** Miembros.  
5. Seleccione **Elegir miembros**. Aparecerá otra ventana desplegable.
6. Seleccione **+ Agregar** para elegir uno o varios usuarios para agregar al grupo.  
7. Seleccione la casilla situada junto a los nombres que desea agregar y, a continuación, seleccione el **botón** Agregar en la parte inferior.  
8. Cuando haya terminado de asignar usuarios, seleccione **Listo**, Luego **Guardar** y, a continuación, **Cerrar**.

## <a name="learn-more-about-role-groups-and-roles"></a>Más información sobre los grupos de roles y los roles

Según la estructura del equipo, tiene opciones para asignar usuarios a grupos de roles específicos para administrar diferentes conjuntos de características de Priva. Los miembros deben asignarse a grupos de roles en función de las tareas que necesiten realizar y del nivel de acceso a archivos adecuado. Cada grupo de roles incluye uno o más roles. Estos roles pueden pertenecer a tareas específicas de Priva o funciones clave que están habilitadas o restringidas para los miembros de ese grupo. Por lo tanto, es posible que distintos usuarios tengan diferentes niveles de visibilidad y acceso a determinadas características de Priva.

Los grupos de roles se pueden personalizar si es necesario. Para evitar la pérdida accidental de acceso, se recomienda crear una copia del grupo de roles existente que desee personalizar, asignar a la copia un nombre identificable, realizar y comprobar los cambios realizados en el nuevo grupo y asignarle personas según corresponda.

## <a name="privacy-management-role-group"></a>Grupo de roles de administración de privacidad

Este grupo contiene todos los roles de permiso Priva en un único grupo. Este grupo de roles puede ser un buen ajuste para las organizaciones donde la misma persona puede realizar todas las tareas. La pertenencia a este grupo de roles concederá a esa cuenta acceso total a todas las características de Priva para las que tiene una licencia.

Se recomienda asegurarse de que siempre hay al menos un miembro activo de este grupo.

Los roles incluyen:

- Administración de casos  
- Visor de contenido de clasificación de datos  
- Visor de listas de clasificación de datos  
- Administrador de administración de privacidad  
- Análisis de administración de privacidad  
- Investigación de administración de privacidad  
- Contribución permanente de administración de privacidad  
- Contribución temporal de administración de privacidad  
- Visor de administración de privacidad  
- Administrador de solicitudes de derechos de sujeto  
- View-Only case

## <a name="privacy-management-administrators-role-group"></a>Grupo de roles Administradores de administración de privacidad

Los miembros de este grupo de roles tienen un amplio acceso a las funciones Priva, como crear, leer, actualizar y eliminar directivas de administración de riesgos de privacidad, solicitudes de derechos de sujeto, permisos y configuración.

Los roles incluyen:

- Administración de casos  
- Administrador de administración de privacidad  
- View-Only case

## <a name="privacy-management-analysts-role-group"></a>Grupo de roles Analistas de administración de privacidad

Los miembros de este grupo de roles actúan como analistas de casos. Pueden investigar coincidencias de directivas, ver metadatos de archivos y realizar acciones de corrección. Este grupo no puede tener acceso a archivos completos a través del Explorador de contenido.

Los roles incluyen:

- Administración de casos  
- Visor de listas de clasificación de datos  
- Análisis de administración de privacidad  
- View-Only case

### <a name="privacy-management-investigators-role-group"></a>Grupo de roles De investigadores de administración de privacidad

Los miembros de este grupo actúan como investigadores de datos. Pueden investigar coincidencias de directivas, ver el contenido del archivo asociado y realizar acciones de corrección. Este grupo puede tener acceso a los archivos a través del Explorador de contenido.

Los roles incluyen:

- Administración de casos  
- Visor de contenido de clasificación de datos  
- Visor de listas de clasificación de datos  
- Investigación de administración de privacidad  
- View-Only case

## <a name="privacy-management-viewer-role-group"></a>Grupo de roles visor de administración de privacidad

Los miembros de este grupo pueden ver información analítica en Priva, como la información general, el perfil de datos y los informes de solicitud de sujeto.

Los roles incluyen:

- Visor de administración de privacidad

## <a name="subject-rights-request-administrators-role-group"></a>Grupo de roles Administradores de solicitudes de derechos de sujeto

Los miembros de este grupo tienen acceso completo para administrar y crear solicitudes de derechos de sujeto.

Los roles incluyen:

- Administrador de solicitudes de derechos de sujeto

## <a name="privacy-management-contributors-role-group"></a>Grupo de roles Colaboradores de administración de privacidad

Los miembros de este grupo tienen acceso a solicitudes de derechos de sujeto para las que se han agregado como colaboradores.  

Los roles incluyen:

- Contribución temporal de administración de privacidad  
- Contribución permanente de administración de privacidad

## <a name="legal-disclaimer"></a>Declinación de responsabilidades legales

[Declinación de responsabilidades legales de Microsoft Priva](priva-disclaimer.md)