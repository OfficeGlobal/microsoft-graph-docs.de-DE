---
title: RoleAssignmentScopeType Enum-Typ
description: Gibt den Typ des Bereichs für eine Rollenzuweisung.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 738579fbd8bcda9ac438ada2f7746e020396d225
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871540"
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





