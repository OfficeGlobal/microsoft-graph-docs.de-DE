---
title: responseStatus-Ressourcentyp
description: Der Antwortstatus einer Besprechungsanfrage.
localization_priority: Normal
ms.openlocfilehash: 110b0eb158043b9573deb3e3ced792119bfa91a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830779"
---
# <a name="responsestatus-resource-type"></a>responseStatus-Ressourcentyp

Der Antwortstatus einer Besprechungsanfrage.

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ           | Beschreibung |
|:---------|:---------------|:------------|
| Antwort | responseType   | Der Antworttyp. Die möglichen Werte sind: `None`, `Organizer`, `TentativelyAccepted`, `Accepted`, `Declined`, `NotResponded`.
| Uhrzeit     | DateTimeOffset | Datum und Uhrzeit, an dem bzw. der die Antwort zurückgegeben wurde. Hierfür wird das ISO 8601-Format, und die Angabe erfolgt immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.responseStatus"
}-->

```json
{
  "response": "String",
  "time": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "responseStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
