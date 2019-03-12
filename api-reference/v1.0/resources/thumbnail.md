---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Miniaturansicht
localization_priority: Normal
ms.openlocfilehash: d11f9eead6faf885bee579c634267e038f8a8ee4
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482259"
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
| height       | Int32  | Die Höhe der Miniaturansicht in Pixel.
| sourceItemId | String | Der eindeutige Bezeichner des Elements, das die Miniaturansicht zur Verfügung stellt. Diese Eigenschaft ist nur verfügbar, wenn eine Ordnerminiaturansicht angefordert wird.
| url          | String | Die URL, die zum Abrufen der Miniaturansichtsinhalte verwendet wird.
| width        | Int32  | Die Breite der Miniaturansicht in Pixel.
| content      | Stream | Der Inhaltsdatenstrom für die Miniaturansicht.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
