---
title: scheduleItem-Ressourcentyp
description: Ein Element, das die Verfügbarkeit eines Benutzers beschreibt, der einem tatsächlichen Ereignis im Standardkalender des Benutzers entspricht. Dieses Element gilt auch für eine Ressource.
localization_priority: Normal
ms.openlocfilehash: a39f45598ab3c427a741659aa93615317c3c57a7
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869309"
---
# <a name="scheduleitem-resource-type"></a>scheduleItem-Ressourcentyp

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Ein Element, das die Verfügbarkeit eines Benutzers beschreibt, der einem tatsächlichen Ereignis im Standardkalender des Benutzers entspricht. Dieses Element gilt auch für eine Ressource (Raum oder Gerät).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|end |[dateTimeTimeZone](datetimetimezone.md) |Das Datum, die Uhrzeit und die Zeitzone, die das entsprechende Ereignis beendet. |
|isPrivate |Boolesch |Die Vertraulichkeit des entsprechenden Ereignisses. True, wenn das Ereignis markiert `private`ist, andernfalls false. Optional. |
|location |String | Der Ort, an dem das entsprechende Ereignis gehalten oder besucht wird. Optional.|
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
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
