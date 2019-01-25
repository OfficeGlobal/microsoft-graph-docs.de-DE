---
title: SortField-Ressourcentyp
description: Stellt eine Bedingung in einem Sortiervorgang dar.
localization_priority: Normal
ms.openlocfilehash: 52817df89ed130b6984ae3a76da775e0e000dee5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521635"
---
# <a name="sortfield-resource-type"></a>SortField-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Bedingung in einem Sortiervorgang dar.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|ascending|Boolescher Wert|Stellt dar, ob die Sortierung in aufsteigender Reihenfolge ausgeführt wird.|
|color|string|Stellt die Farbe dar, die das Ziel der Bedingung ist, wenn die Sortierung für die Schrift- oder Zellenfarbe gilt.|
|dataOption|string|Stellt weitere Sortieroptionen für dieses Feld dar. Die folgenden Werte sind möglich: `Normal`, `TextAsNumber`.|
|Key|int|Stellt die Spalte (oder Zeile, je nach Sortierausrichtung) dar, für die die Bedingung gilt. Wird als Offset von der ersten Spalte (oder Zeile) dargestellt.|
|sortOn|string|Stellt den Typ der Sortierung dieser Bedingung dar. Die folgenden Werte sind möglich: `Value`, `CellColor`, `FontColor`, `Icon`.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Symbol|[Icon](icon.md)|Stellt das Symbol dar, das das Ziel der Bedingung ist, wenn die Sortierung für das Symbol der Zelle gilt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sortfield.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
