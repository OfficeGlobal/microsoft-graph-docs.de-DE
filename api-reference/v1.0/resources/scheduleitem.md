---
title: scheduleItem-Ressourcentyp
description: Ein Element, das die Verfügbarkeit eines Benutzers beschreibt, der einem tatsächlichen Ereignis im Standardkalender des Benutzers entspricht. Dieses Element gilt auch für eine Ressource (Raum oder Gerät).
localization_priority: Normal
ms.openlocfilehash: 8a30dcb4394a963e35047fab00391f0cc7eb7715
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30926603"
---
# <a name="scheduleitem-resource-type"></a>scheduleItem-Ressourcentyp

Ein Element, das die Verfügbarkeit eines Benutzers beschreibt, der einem tatsächlichen Ereignis im Standardkalender des Benutzers entspricht. Dieses Element gilt auch für eine Ressource (Raum oder Gerät).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |Das Datum, die Uhrzeit und die Zeitzone, die das entsprechende Ereignis beendet. |
|isPrivate |Boolescher Wert |Die Vertraulichkeit des entsprechenden Ereignisses. True, wenn das Ereignis markiert `private`ist, andernfalls false. Optional.|
|location |Zeichenfolge | Der Ort, an dem das entsprechende Ereignis gehalten oder besucht wird. Optional.|
|start |[dateTimeTimeZone](datetimetimezone.md) |Das Datum, die Uhrzeit und die Zeitzone, die das entsprechende Ereignis startet. |
|status |freeBusyStatus | Der Verfügbarkeitsstatus des Benutzers oder der Ressource während des entsprechenden Ereignisses. Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`. |
|subject |String | Die Betreffzeile des entsprechenden Ereignisses. Optional.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isPrivate",
    "location",
    "subject"
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
  "tocPath": ""
}
-->
