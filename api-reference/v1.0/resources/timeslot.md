---
title: Ressourcentyp „timeSlot“
description: Ein Zeitfenster
localization_priority: Normal
ms.openlocfilehash: e01b8d0f34a21eb18bc92e8bcc4e1b8365541d5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860564"
---
# <a name="timeslot-resource-type"></a>Ressourcentyp „timeSlot“

Ein Zeitfenster

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeSlot"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|end|[dateTimeTimeZone](datetimetimezone.md)|Die Startzeit des betreffenden Zeitfensters|
|start|[dateTimeTimeZone](datetimetimezone.md)|Die Endzeit des betreffenden Zeitfensters|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
