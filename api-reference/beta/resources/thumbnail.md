---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Thumbnail
ms.openlocfilehash: 8e56612185028891cf380d3240c999af78ff4740
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061646"
---
# <a name="thumbnail-resource-type"></a>Thumbnail-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Der **thumbnail**-Ressourcentyp stellt eine Miniaturansicht für ein Bild, ein Video, ein Dokument oder ein beliebiges Element dar, das über eine Bitmapdarstellung verfügt.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der **thumbnail**-Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width", "sourceItemId"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,

  /* relationships */
  "content": "stream"
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ   | Beschreibung                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| height       | Int32  | Die Höhe der Miniaturansicht in Pixel.                                                                                     |
| sourceItemId | String | Der eindeutige Bezeichner des Elements, das die Miniaturansicht zur Verfügung stellt. Diese Eigenschaft ist nur verfügbar, wenn eine Ordnerminiaturansicht angefordert wird. |
| url          | String | Die URL, die zum Abrufen der Miniaturansichtsinhalte verwendet wird.                                                                                |
| width        | Int32  | Die Breite der Miniaturansicht in Pixel.                                                                                      |

## <a name="relationships"></a>Beziehungen

| Name    | Typ   | Beschreibung                           |
| :------ | :----- | :------------------------------------ |
| Inhalt | Stream | Der Inhaltsdatenstrom für die Miniaturansicht. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
