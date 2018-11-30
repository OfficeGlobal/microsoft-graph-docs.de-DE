---
title: sizeRange-Ressourcentyp
description: Gibt die maximale und minimale Größe (in Kilobyte) an, die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.
ms.openlocfilehash: e9ef87063959f320068933a17c1fa8b0a70859da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016407"
---
# <a name="sizerange-resource-type"></a>sizeRange-Ressourcentyp


Gibt die maximale und minimale Größe (in Kilobyte) an, die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| maximumSize | Int32 | Die maximale Größe (in Kilobyte), die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft. |
| minimumSize | Int32 | Die minimale Größe (in Kilobyte), die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft. |


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.sizeRange"
}-->

```json
{
  "maximumSize": "Int32",
  "minimumSize": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sizeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->