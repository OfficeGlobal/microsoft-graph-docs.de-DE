---
title: RoleAssignmentScopeType Enum-Typ
description: Gibt den Typ des Bereichs für eine Rollenzuweisung.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b72e74bdb401f556214470b4c0aeda651339e332
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916082"
---
# <a name="roleassignmentscopetype-enum-type"></a>RoleAssignmentScopeType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Gibt den Typ des Bereichs für eine Rollenzuweisung.
## <a name="members"></a>Elemente
|Element|Wert|Beschreibung|
|:---|:---|:---|
|resourceScope|0|Zuordnungen für den angegebenen ResourceScopes zulassen.|
|allDevices|1|Zuordnungen für alle Intune Geräte zulassen|
|allLicensedUsers|2|Zuordnungen für alle Intune lizenzierten Benutzer zulassen.|
|allDevicesAndLicensedUsers|3|Zuordnungen für alle Intune Geräte und lizenzierte Benutzer zulassen.|





