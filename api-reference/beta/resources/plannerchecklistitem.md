---
title: plannerChecklistItem-Ressourcentyp
description: Die Ressource **PlannerChecklistItem** stellt ein Element in der Prüfliste eines Vorgangs dar. Die Checkliste für einen Vorgang wird durch das ChecklistItems-Objekt dargestellt.
ms.openlocfilehash: 846c1877fb421c9070eff7c041983367a7beb29b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061428"
---
# <a name="plannerchecklistitem-resource-type"></a>plannerChecklistItem-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **plannerChecklistItem**-Ressource stellt ein Element in der Checkliste einer Aufgabe dar. Die Checkliste für eine Aufgabe wird durch das [checklistItems-Objekt](plannerchecklistitems.md) dargestellt.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|isChecked|Boolean|Der Wert ist `true`, wenn das Element geprüft wurde, andernfalls `false`.|
|lastModifiedBy|[identitySet](identityset.md)| Schreibgeschützt. Benutzer-ID, von der das Objekt zuletzt geändert wurde.|
|lastModifiedDateTime|DateTimeOffset|Schreibgeschützt. Datum und Uhrzeit der letzten Änderung des Objekts. Der Zeitstempeltyp stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|orderHint|String|Wird verwendet, um die relative Reihenfolge der Elemente in der Checkliste festzulegen. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.|
|title|String|Titel des Checklistenelements.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->