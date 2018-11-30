---
title: SortField-Ressourcentyp
description: Stellt eine Bedingung in einem Sortiervorgang dar.
ms.openlocfilehash: bb5915e9d9637912b97c0425819acd15a6ed40ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063901"
---
# <a name="sortfield-resource-type"></a>SortField-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine Bedingung in einem Sortiervorgang dar.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|ascending|boolean|Stellt dar, ob die Sortierung in aufsteigender Reihenfolge ausgeführt wird.|
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
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->