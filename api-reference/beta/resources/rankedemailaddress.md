---
title: Ressourcentyp rankedEmailAddress
description: Stellt eine bewerteter e-Mail-Adresse dar.
ms.openlocfilehash: 9234f527ecba6dc83f2e4f80911442d4a083503a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064979"
---
# <a name="rankedemailaddress-resource-type"></a>Ressourcentyp rankedEmailAddress

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine bewerteter e-Mail-Adresse dar.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|address|string|Die E-Mail-Adresse|
|rank|double|Die Rangfolge der e-Mail-Adresse. Ein Rang wird als Sortierschlüssel, in Bezug auf die anderen zurückgegebenen Ergebnisse verwendet. Ein höherer Rangwert entspricht ein relevanter Ergebnis. Relevanz ergibt sich für die Zusammenarbeit, Kommunikation und geschäftlichen Beziehung signalisiert.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rankedEmailAddress"
}-->

```json
{
  "address": "string",
  "rank": 1024
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
