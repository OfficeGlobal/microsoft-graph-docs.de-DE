---
title: Ressourcentyp licenseAssignmentState
description: Die **LicenseAssignmentStates** -Eigenschaft der Benutzerentität ist eine Auflistung von **LicenseAssignmentState** -Objekten. Es enthält Details zur Lizenz Zuordnungen für einen Benutzer.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0822c975ab81badf5334881bb460532161858010
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649419"
---
# <a name="licenseassignmentstate-resource-type"></a>Ressourcentyp licenseAssignmentState


Die **LicenseAssignmentStates** -Eigenschaft der Entität [Benutzer](user.md) ist eine Auflistung von **LicenseAssignmentState** -Objekten. Es enthält Details zur Lizenz Zuordnungen für einen Benutzer. Die Details enthalten Informationen wie etwa:  

 - Welche Pläne für einen Benutzer deaktiviert sind
 - Gibt an, ob die Lizenz zugewiesen, die dem Benutzer direkt oder aus einer Gruppe geerbt wurde
 - Den aktuellen Status der Zuordnung
 - Wenn der Zuordnung Zustand Fehler ist Fehlerdetails 


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|assignedByGroup|string|Die Id der Gruppe, die diese Lizenz zugewiesen. Wenn die Zuordnung einer Lizenz Direct zugewiesen ist, werden in diesem Feld auf Null festgelegt. Schreibgeschützt.|
|disabledPlans|Collection(String)|Die Servicepläne, die in dieser Aufgabe deaktiviert sind. Schreibgeschützt.|
|error|String|Lizenz-Zuordnung-Fehler. Wenn die Lizenz erfolgreich zugewiesen ist, werden in diesem Feld auf Null festgelegt. Schreibgeschützt. Mögliche Werte: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, und `Others`. Weitere Informationen zum Identifizieren und Beheben von lizenzzuweisung Fehler finden Sie [hier](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).|
|skuId|String|Die eindeutige ID der SKU. Schreibgeschützt.|
|state|String|Geben Sie den aktuellen Status dieser Aufgabe an. Schreibgeschützt. Mögliche Werte: aktiv "," ActiveWithError "," deaktiviert "und" Fehler.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseAssignmentState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: microsoft.graph.user/licenseAssignmentStates:
      Referenced type microsoft.graph.licenseAssignmentState is not defined in the doc set! Potential suggestion: UNKNOWN"
  ]
}-->
