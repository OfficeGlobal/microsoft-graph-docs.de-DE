---
title: Ressourcentyp licenseAssignmentState
description: 'Die **LicenseAssignmentStates** -Eigenschaft der Benutzerentität ist eine Auflistung von **LicenseAssignmentState**. Es enthält Details zur Lizenz Zuordnungen für einen Benutzer. Die Details enthält Informationen wie folgt:  '
ms.openlocfilehash: 4e7101acc756a845913a081368b79242834ef3bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063893"
---
# <a name="licenseassignmentstate-resource-type"></a>Ressourcentyp licenseAssignmentState

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **LicenseAssignmentStates** -Eigenschaft der Entität [Benutzer](user.md) ist eine Auflistung von **LicenseAssignmentState**. Es enthält Details zur Lizenz Zuordnungen für einen Benutzer. Die Details enthält Informationen wie folgt:  

 - Welche Pläne für einen Benutzer deaktiviert sind
 - Gibt an, ob die Lizenz zugewiesen, die dem Benutzer direkt oder aus einer Gruppe geerbt wurde
 - Aktuellen Status der Zuordnung
 - Wenn der Zuordnung Zustand Fehler ist, was die Fehlerdetails für den Fehler ist? 


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