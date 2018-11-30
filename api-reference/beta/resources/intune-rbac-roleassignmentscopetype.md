---
title: RoleAssignmentScopeType Enum-Typ
description: Gibt den Typ des Bereichs für eine Rollenzuweisung.
ms.openlocfilehash: dcfac7b345dde2d8f107b8ec756d017966a6a94a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063364"
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





