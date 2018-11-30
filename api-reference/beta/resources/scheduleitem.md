---
title: von ScheduleItem Ressourcentyp
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: a7a31f47cde92549a72299b22a40b10c6f7845c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063538"
---
# <a name="scheduleitem-resource-type"></a>von ScheduleItem Ressourcentyp

 > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.
 
Ein Element, das beschreibt die Verfügbarkeit eines Benutzers auf ein Ereignis tatsächliche auf Standardkalender des Benutzers entspricht. Dieses Element gilt für als auch eine Ressource.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |Das Datum, Uhrzeit und Zeitzone, die das zugehörige Ereignis endet. |
|isPrivate |Boolesch |Die Vertraulichkeit des entsprechenden Ereignisses. True, wenn das Ereignis markiert wird `private`false andernfalls. |
|location |String | Der Speicherort, an dem entsprechenden Ereigniscode gehalten oder teilnahmen aus. Optional.|
|start |[dateTimeTimeZone](datetimetimezone.md) |Das Datum, Uhrzeit und Zeitzone, die das zugehörige Ereignis beginnt. |
|status |String | Der Verfügbarkeitsstatus des Benutzers oder der Ressource während des entsprechenden Ereignisses. Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`. |
|Betreff |String | Die Betreffzeile das entsprechende Ereignis. Optional.|


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
<!-- {
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->