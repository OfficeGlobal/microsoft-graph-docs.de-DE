---
title: von ScheduleItem Ressourcentyp
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: ed6b7441996cdf00b33be03f70afb888cc9bb251
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511352"
---
# <a name="scheduleitem-resource-type"></a>von ScheduleItem Ressourcentyp

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Ein Element, das beschreibt die Verfügbarkeit eines Benutzers auf ein Ereignis tatsächliche auf Standardkalender des Benutzers entspricht. Dieses Element gilt für als auch eine Ressource.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |Das Datum, Uhrzeit und Zeitzone, die das zugehörige Ereignis endet. |
|IsPrivate |Boolescher Wert |Die Vertraulichkeit des entsprechenden Ereignisses. True, wenn das Ereignis markiert wird `private`false andernfalls. |
|location |String | Der Speicherort, an dem entsprechenden Ereigniscode gehalten oder teilnahmen aus. Optional.|
|start |[dateTimeTimeZone](datetimetimezone.md) |Das Datum, Uhrzeit und Zeitzone, die das zugehörige Ereignis beginnt. |
|status |String | Der Verfügbarkeitsstatus des Benutzers oder der Ressource während des entsprechenden Ereignisses. Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`. |
|subject |String | Die Betreffzeile das entsprechende Ereignis. Optional.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleItem"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "isPrivate": true,
  "location": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
