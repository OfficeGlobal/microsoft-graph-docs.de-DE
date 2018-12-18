---
title: RoleAssignmentScopeType Enum-Typ
description: Gibt den Typ des Bereichs für eine Rollenzuweisung.
author: tfitzmac
ms.openlocfilehash: 0a3286b3b7bc583323204ca39ff85e01869ddbe7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343127"
---
# <a name="roleassignmentscopetype-enum-type"></a>RoleAssignmentScopeType Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Gibt den Typ des Bereichs für eine Rollenzuweisung.
## <a name="members"></a>Elemente
|Member|Wert|Beschreibung|
|:---|:---|:---|
|resourceScope|0|Zuordnungen für den angegebenen ResourceScopes zulassen.|
|allDevices|1|Zuordnungen für alle Intune Geräte zulassen|
|allLicensedUsers|2|Zuordnungen für alle Intune lizenzierten Benutzer zulassen.|
|allDevicesAndLicensedUsers|3|Zuordnungen für alle Intune Geräte und lizenzierte Benutzer zulassen.|





