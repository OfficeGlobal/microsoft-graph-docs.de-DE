---
title: ChartTitle-Ressourcentyp
description: Ein Diagrammtitelobjekt eines Diagramms.
ms.openlocfilehash: 44777d939e67d2e8b5563cf3edb0b5bfddeeef9a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017013"
---
# <a name="charttitle-resource-type"></a>ChartTitle-Ressourcentyp

Ein Diagrammtitelobjekt eines Diagramms.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[ChartTitle abrufen](../api/charttitle-get.md) | [WorkbookChartTitle](charttitle.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des chartTitle-Objekts.|
|[Update](../api/charttitle-update.md) | [WorkbookChartTitle](charttitle.md)    |Dient zum Aktualisieren des ChartTitle-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Overlay|boolean|Boolescher Wert, der angibt, ob der Diagrammtitel das Diagramm überlagert.|
|text|string|Stellt den Titeltext eines Diagramms dar.|
|visible|boolean|Ein boolescher Wert, der die Sichtbarkeit eines Diagrammtitelobjekts darstellt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Format|[WorkbookChartTitleFormat](charttitleformat.md)|Stellt die Formatierung für einen Diagrammtitel dar, einschließlich Füllung und Schriftartformatierung. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartTitle"
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