---
title: Ressourcentyp licenseAssignmentState
description: 'Die **LicenseAssignmentStates** -Eigenschaft der Benutzerentität ist eine Auflistung von **LicenseAssignmentState**. Es enthält Details zur Lizenz Zuordnungen für einen Benutzer. Die Details enthält Informationen wie folgt:  '
localization_priority: Normal
ms.openlocfilehash: f2f905baaba4dddd65266ffafab44febe7a61139
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575181"
---
# <a name="licenseassignmentstate-resource-type"></a>Ressourcentyp licenseAssignmentState

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **LicenseAssignmentStates** -Eigenschaft der Entität [Benutzer](user.md) ist eine Auflistung von **LicenseAssignmentState**. Es enthält Details zur Lizenz Zuordnungen für einen Benutzer. Die Details enthält Informationen wie folgt:  

 - Welche Pläne für einen Benutzer deaktiviert sind
 - Gibt an, ob die Lizenz zugewiesen, die dem Benutzer direkt oder aus einer Gruppe geerbt wurde
 - Aktuellen Status der Zuordnung
 - Wenn der Zuordnung Zustand Fehler ist, was die Fehlerdetails für den Fehler ist? 


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|assignedByGroup|string|Die Id der Gruppe, die diese Lizenz zugewiesen. Wenn die Zuordnung einer Lizenz Direct zugewiesen ist, werden in diesem Feld auf Null festgelegt. Schreibgeschützt.|
|disabledPlans| Zeichenfolgenauflistung |Die Servicepläne, die in dieser Aufgabe deaktiviert sind. Schreibgeschützt.|
|error|String|Lizenz-Zuordnung-Fehler. Wenn die Lizenz erfolgreich zugewiesen ist, werden in diesem Feld auf Null festgelegt. Schreibgeschützt. Mögliche Werte: `CountViolation`, `MutuallyExclusiveViolation`, `DependencyViolation`, `ProhibitedInUsageLocationViolation`, `UniquenessViolation`, und `Others`. Weitere Informationen zum Identifizieren und Beheben von lizenzzuweisung Fehler finden Sie [hier](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems).|
|skuId|String|Die eindeutige ID der SKU. Schreibgeschützt.|
|state|String|Geben Sie den aktuellen Status dieser Aufgabe an. Schreibgeschützt. Mögliche Werte: aktiv "," ActiveWithError "," deaktiviert "und" Fehler.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.licenseAssignmentState"
}-->
```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/licenseAssignmentState.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
