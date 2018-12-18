---
title: ChartAxisTitle-Ressourcentyp
description: Stellt den Titel einer Diagrammachse dar.
author: lumine2008
ms.openlocfilehash: f787e4572c0b0f499740e2ba1e790fec1ce7ba61
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357295"
---
# <a name="chartaxistitle-resource-type"></a>ChartAxisTitle-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt den Titel einer Diagrammachse dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[ChartAxisTitle abrufen](../api/chartaxistitle-get.md) | [ChartAxisTitle](chartaxistitle.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des chartAxisTitle-Objekts.|
|[Update](../api/chartaxistitle-update.md) | [ChartAxisTitle](chartaxistitle.md)    |Dient zum Aktualisieren de chartAxisTitle-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|text|string|Stellt den Achsentitel dar.|
|visible|boolean|Ein boolescher Wert, der die Sichtbarkeit eines Achsentitels angibt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Format|[ChartAxisTitleFormat](chartaxistitleformat.md)|Stellt die Formatierung des Diagrammachsentitels dar. Schreibgeschützt.|

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->