---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
ms.openlocfilehash: ba72b813e0c68c3942a63b111e75298d7da3d68b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512696"
---
# <a name="thumbnailset-resource-type"></a>ThumbnailSet-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **ThumbnailSet**-Ressource ist eine verschlüsselter Sammlung von [thumbnail](thumbnail.md)-Ressourcen. Sie wird zum Darstellen eines Satzes von Miniaturansichten verwendet, die mit einem DriveItem verknüpft sind.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": ["source", "small", "medium", "large"],
  "openType": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->

```json
{
  "id": "string (identifier)",
  "large": { "@odata.type": "microsoft.graph.thumbnail" },
  "medium": { "@odata.type": "microsoft.graph.thumbnail" },
  "small": { "@odata.type": "microsoft.graph.thumbnail" },
  "source": { "@odata.type": "microsoft.graph.thumbnail" }
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ                      | Beschreibung                                                                       |
|:---------|:--------------------------|:----------------------------------------------------------------------------------|
| id       | String                    | Die ID innerhalb des Elements. Schreibgeschützt.                                                |
| large    | [Miniaturansicht](thumbnail.md) | Eine skalierte Miniaturansicht von 1920x1920.                                                     |
| medium   | [Miniaturansicht](thumbnail.md) | Eine skalierte Miniaturansicht von 176x176.                                                       |
| small    | [Miniaturansicht](thumbnail.md) | Eine zugeschnittene Miniaturansicht von 48x48.                                                        |
| source   | [Miniaturansicht](thumbnail.md) | Eine benutzerdefiniertes Miniaturbild oder das ursprüngliche Bild, das zum Erstellen anderer Miniaturansichten verwendet wird. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet",
  "suppressions": [
    "Error: /api-reference/beta/resources/thumbnailset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
