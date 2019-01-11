---
title: plannerTaskDetails-Ressourcentyp
description: Die **plannerTaskDetails**-Ressource stellt die zusätzlichen Informationen zu einer Aufgabe dar. Jedes task-Objekt hat ein Detailobjekt.
localization_priority: Normal
ms.openlocfilehash: 0bec5b47d1472eae43906841c5074e4080672817
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888165"
---
# <a name="plannertaskdetails-resource-type"></a>plannerTaskDetails-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **plannerTaskDetails**-Ressource stellt die zusätzlichen Informationen zu einer Aufgabe dar. Jedes [task](plannertask.md)-Objekt hat ein Detailobjekt.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[plannerTaskDetails abrufen](../api/plannertaskdetails-get.md) | [plannerTaskDetails](plannertaskdetails.md) |Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerTaskDetails**-Objekts.|
|[Update](../api/plannertaskdetails-update.md) | [plannerTaskDetails](plannertaskdetails.md)    |Dient zum Aktualisieren des **plannerTaskDetails**-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|checklist|[plannerChecklistItems](plannerchecklistitems.md)|Die Sammlung von Checklistenelementen für die Aufgabe.|
|description|String|Beschreibung der Aufgabe.|
|id|String| Schreibgeschützt. ID des die Aufgabendetails. Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet. [Format Validierung](tasks-identifiers-disclaimer.md) erfolgt für den Dienst.|
|previewType|string|Hierdurch wird der Typ der Vorschau festgelegt, die für die Aufgabe angezeigt wird. Mögliche Werte: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Bei Festlegung auf `automatic` wird die angezeigte Vorschau von der App ausgewählt, mit der die Aufgabe angezeigt wird.|
|references|[plannerExternalReferences](plannerexternalreferences.md)|Die Sammlung der Verweise für die Aufgabe.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
