---
title: von ScheduleItem Ressourcentyp
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: e5d14826a27153af27648484554ec864d62ed6c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890433"
---
# <a name="scheduleitem-resource-type"></a>von ScheduleItem Ressourcentyp

 > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.
 
Ein Element, das beschreibt die Verfügbarkeit eines Benutzers auf ein Ereignis tatsächliche auf Standardkalender des Benutzers entspricht. Dieses Element gilt für als auch eine Ressource.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |Das Datum, Uhrzeit und Zeitzone, die das zugehörige Ereignis endet. |
|isPrivate |Boolescher Wert |Die Vertraulichkeit des entsprechenden Ereignisses. True, wenn das Ereignis markiert wird `private`false andernfalls. |
|location |Zeichenfolge | Der Speicherort, an dem entsprechenden Ereigniscode gehalten oder teilnahmen aus. Optional.|
|start |[dateTimeTimeZone](datetimetimezone.md) |Das Datum, Uhrzeit und Zeitzone, die das zugehörige Ereignis beginnt. |
|status |Zeichenfolge | Der Verfügbarkeitsstatus des Benutzers oder der Ressource während des entsprechenden Ereignisses. Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`. |
|Betreff |Zeichenfolge | Die Betreffzeile das entsprechende Ereignis. Optional.|


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
