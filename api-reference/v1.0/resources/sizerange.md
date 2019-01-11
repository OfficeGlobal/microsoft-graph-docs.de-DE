---
title: sizeRange-Ressourcentyp
description: Gibt die maximale und minimale Größe (in Kilobyte) an, die eine eingehende Nachrichten aufweisen muss, damit eine Bedingung oder Ausnahme zutrifft.
localization_priority: Normal
ms.openlocfilehash: ae754d0666185023272860864ef17f038aecff7c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873542"
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
