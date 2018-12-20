---
title: Ressourcentyp toneInfo
description: Ein einzelnes DTMF-Ereignis.
author: VinodRavichandran
ms.openlocfilehash: 0ae78a9a4721c88767ebc460a99c7cdea30f44c5
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380338"
---
# <a name="toneinfo-resource-type"></a>Ressourcentyp toneInfo

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ein einzelnes DTMF-Ereignis.

## <a name="properties"></a>Eigenschaften

| Eigenschaft       | Typ    | Beschreibung|
|:---------------|:--------|:----------|
| sequenceId | Int64 | Ein inkrementelle Bezeichner für eine Sortierung DTMF-Ereignisse verwendet. |
| Tone | Zeichenfolge | Mögliche Werte sind: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.toneInfo"
}-->
```json
{
  "sequenceId": 1024,
  "tone": "tone0 | tone1 | tone2 | tone3 | tone4 | tone5 | tone6 | tone7 | tone8 | tone9 | star | pound | a | b | c | d | flash"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "toneInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->