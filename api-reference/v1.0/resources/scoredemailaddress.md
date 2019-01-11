---
title: scoredEmailAddress-Ressourcentyp
description: Gibt eine bewertete E-Mail-Adresse an.
localization_priority: Normal
ms.openlocfilehash: 740173e7d5f93dc875c08508bf73100727fdf415
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819474"
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
