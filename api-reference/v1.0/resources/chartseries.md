---
title: ChartSeries-Ressourcentyp
description: Stellt eine Datenreihe in einem Diagramm dar.
author: lumine2008
ms.openlocfilehash: 60cd3e29f1b2c2f106fae0fdfb76b18657d68120
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314490"
---
# <a name="chartseries-resource-type"></a>ChartSeries-Ressourcentyp

Stellt eine Datenreihe in einem Diagramm dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[ChartSeries abrufen](../api/chartseries-get.md) | [WorkbookChartSeries](chartseries.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des chartSeries-Objekts.|
|[ChartPoints erstellen](../api/chartseries-post-points.md) |[ChartPoints](chartpoint.md)| Dient zum Erstellen eines neuen ChartPoints durch Veröffentlichen in der Punkteammlung.|
|[Punkte auflisten](../api/chartseries-list-points.md) |[ChartPoints-Sammlung](chartpoint.md)| Dient zum Abrufen einer ChartPoints-Objeksammlung.|
|[Update](../api/chartseries-update.md) | [WorkbookChartSeries](chartseries.md) |Dient zum Aktualisieren des ChartSeries-Objekts. |
|[List](../api/chartseries-list.md) | [WorkbookChartSeries](chartseries.md) -Auflistung |Dient zum Abrufen der chartSeries-Objektsammlung. |
|[ItemAt](../api/chartseriescollection-itemat.md)|[WorkbookChartSeries](chartseries.md)|Ruft eine Datenreihe anhand ihrer Position in der Sammlung ab.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|name|string|Gibt den Namen einer Datenreihe in einem Diagramm an.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Format|[WorkbookChartSeriesFormat](chartseriesformat.md)|Stellt die Formatierung für eine Diagrammdatenreihe dar, einschließlich Füllung und Linienformatierung. Schreibgeschützt.|
|points|[WorkbookChartPoint](chartpoint.md) -Auflistung|Stellt eine Sammlung aller Punkte in der Datenreihe dar. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->