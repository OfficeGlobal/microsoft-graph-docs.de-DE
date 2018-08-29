---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Miniaturansicht
ms.openlocfilehash: ff111f44101bb03b3d8475e2567d6e1b2b4a753d
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264973"
---
# <a name="thumbnail-resource-type"></a>Thumbnail-Ressourcentyp

Der **thumbnail**-Ressourcentyp stellt eine Miniaturansicht für ein Bild, ein Video, ein Dokument oder ein beliebiges Element dar, das über eine Bitmapdarstellung verfügt.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der **thumbnail**-Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "content",
    "height",
    "width",
    "sourceItemId"
  ],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,
  "content": "stream"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ   | Beschreibung
| :----------- | :----- | :----------------------------------------------------
| Höhe       | Int32  | Die Höhe der Miniaturansicht in Pixel.
| sourceItemId | Zeichenfolge | Der eindeutige Bezeichner des Elements, das die Miniaturansicht zur Verfügung stellt. Diese Eigenschaft ist nur verfügbar, wenn eine Ordnerminiaturansicht angefordert wird.
| URL          | Zeichenfolge | Die URL, die zum Abrufen der Miniaturansichtsinhalte verwendet wird.
| Breite        | Int32  | Die Breite der Miniaturansicht in Pixel.
| Inhalt      | Stream | Der Inhaltsdatenstrom für die Miniaturansicht.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
