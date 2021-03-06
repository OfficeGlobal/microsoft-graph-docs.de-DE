---
title: Zeitstempel Ressourcentyp
description: Datum und Uhrzeit Informationen für einen Punkt in der Zeit.
localization_priority: Normal
ms.openlocfilehash: c63b3bba93f4b108a8eb9943d3fc2a1b2961f06c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888802"
---
# <a name="timestamp-resource-type"></a>Zeitstempel Ressourcentyp

Datum und Uhrzeit Informationen für einen Punkt in der Zeit.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|date|Datum|Das der Zeitstempel Datumsteil.|
|time|TimeOfDay|Den Zeitbereich des der Zeitstempel.|
|timeZone|Zeichenfolge|Der Timezone-Teil der Zeitstempel, der einem der 24 Länge Bereiche in der ganzen Welt ist.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
