---
title: ChartTitle-Ressourcentyp
description: Ein Diagrammtitelobjekt eines Diagramms.
author: lumine2008
ms.openlocfilehash: b3d685c68b14ebe3f49eb3dd9186838c977c1cac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338101"
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
|Format|[ChartTitleFormat](charttitleformat.md)|Stellt die Formatierung für einen Diagrammtitel dar, einschließlich Füllung und Schriftartformatierung. Schreibgeschützt.|

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