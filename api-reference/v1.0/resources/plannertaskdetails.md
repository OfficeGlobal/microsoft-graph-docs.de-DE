---
title: plannerTaskDetails-Ressourcentyp
description: Die **plannerTaskDetails**-Ressource stellt die zusätzlichen Informationen zu einer Aufgabe dar. Jedes task-Objekt hat ein Detailobjekt.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 75e17200dc52fff385c7be8fb0269a3da20464b8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956010"
---
# <a name="plannertaskdetails-resource-type"></a>plannerTaskDetails-Ressourcentyp

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
|id|Zeichenfolge| Schreibgeschützt. ID des die Aufgabendetails. Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet. [Format Validierung](planner-identifiers-disclaimer.md) erfolgt für den Dienst.|
|previewType|string|Hierdurch wird den Typ der Vorschau, die für den Vorgang wird angezeigt. Die möglichen Werte sind: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Bei Festlegung auf `automatic` die angezeigte Vorschau wird von der app anzeigen den Vorgang ausgewählt.|
|references|[plannerExternalReferences](plannerexternalreferences.md)|Die Sammlung der Verweise für die Aufgabe.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
