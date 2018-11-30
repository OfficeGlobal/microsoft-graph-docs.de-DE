---
title: scoredEmailAddress-Ressourcentyp
description: Gibt eine bewertete E-Mail-Adresse an.
ms.openlocfilehash: 9cdd33a6df9eefca0f7a00c5fe8b17832e0056d9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020088"
---
# <a name="scoredemailaddress-resource-type"></a>scoredEmailAddress-Ressourcentyp

Gibt eine bewertete E-Mail-Adresse an.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|address|string|Die E-Mail-Adresse|
|relevanceScore|double|Die Relevanzbewertung der E-Mail-Adresse. Eine Relevanzbewertung dient als Sortierschlüssel, in Bezug auf andere zurückgegebene Ergebnisse. Ein höherer Relevanzwert entspricht einem relevanteren Ergebnis. Relevanz wird durch die Kommunikations- und Zusammenarbeitsmuster und Geschäftsbeziehungen des Benutzers bestimmt. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scoredEmailAddress"
}-->

```json
{
  "address": "string",
  "relevanceScore": 1024.0
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scoredEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
