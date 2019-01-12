---
title: ChartTitle-Ressourcentyp
description: Ein Diagrammtitelobjekt eines Diagramms.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: db0b95e0e01fcbf1c962689a1615066692700992
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977563"
---
# <a name="charttitle-resource-type"></a>ChartTitle-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ein Diagrammtitelobjekt eines Diagramms.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[ChartTitle abrufen](../api/charttitle-get.md) | [ChartTitle](charttitle.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des chartTitle-Objekts.|
|[Update](../api/charttitle-update.md) | [ChartTitle](charttitle.md)    |Dient zum Aktualisieren des ChartTitle-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Overlay|boolean|Boolescher Wert, der angibt, ob der Diagrammtitel das Diagramm überlagert.|
|text|string|Stellt den Titeltext eines Diagramms dar.|
|visible|boolean|Ein boolescher Wert, der die Sichtbarkeit eines Diagrammtitelobjekts darstellt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|format|[ChartTitleFormat](charttitleformat.md)|Stellt die Formatierung für einen Diagrammtitel dar, einschließlich Füllung und Schriftartformatierung. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
