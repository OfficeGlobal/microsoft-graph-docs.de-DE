---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Miniaturansicht
localization_priority: Normal
ms.openlocfilehash: 485714109005415d4a2c98fbbf2befb50ca991d0
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481755"
---
# <a name="thumbnail-resource-type"></a>Thumbnail-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
| sourceItemId | Zeichenfolge | Der eindeutige Bezeichner des Elements, das die Miniaturansicht zur Verfügung stellt. Diese Eigenschaft ist nur verfügbar, wenn eine Ordnerminiaturansicht angefordert wird. |
| url          | String | Die URL, die zum Abrufen der Miniaturansichtsinhalte verwendet wird.                                                                                |
| width        | Int32  | Die Breite der Miniaturansicht in Pixel.                                                                                      |

## <a name="relationships"></a>Beziehungen

| Name    | Typ   | Beschreibung                           |
| :------ | :----- | :------------------------------------ |
| Inhalt | Stream | Der Inhaltsdatenstrom für die Miniaturansicht. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail",
  "suppressions": [
    "Error: /api-reference/beta/resources/thumbnail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
