---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ThumbnailSet
localization_priority: Normal
ms.openlocfilehash: 779cc9129bbbe660286d2350a76451c9666752d5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888872"
---
# <a name="thumbnailset-resource-type"></a>ThumbnailSet-Ressourcentyp

Die **ThumbnailSet**-Ressource ist eine verschlüsselter Sammlung von [thumbnail](thumbnail.md)-Ressourcen. Sie wird zum Darstellen eines Satzes von Miniaturansichten verwendet, die mit einem DriveItem verknüpft sind.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "source",
    "small",
    "medium",
    "large"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.thumbnailSet",
  "openType": true
}-->

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
<!-- {
  "type": "#page.annotation",
  "description": "ThumbnailSet enables access to thumbnails of different sizes",
  "section": "documentation",
  "tocPath": "Resources/ThumbnailSet"
} -->
