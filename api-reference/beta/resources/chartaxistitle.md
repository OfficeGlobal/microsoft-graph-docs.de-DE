---
title: ChartAxisTitle-Ressourcentyp
description: Stellt den Titel einer Diagrammachse dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 25a5daf571f7533bd1682974adecad1cfd984894
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513123"
---
# <a name="chartaxistitle-resource-type"></a>ChartAxisTitle-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt den Titel einer Diagrammachse dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|ChartAxisTitle abrufen | [chartAxisTitle](chartaxistitle.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des chartAxisTitle-Objekts.|
|[Update](../api/chartaxistitle-update.md) | ChartAxisTitle    |Dient zum Aktualisieren de chartAxisTitle-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|text|string|Stellt den Achsentitel dar.|
|visible|Boolescher Wert|Ein boolescher Wert, der die Sichtbarkeit eines Achsentitels angibt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|format|[ChartAxisTitleFormat](chartaxistitleformat.md)|Stellt die Formatierung des Diagrammachsentitels dar. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxistitle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
