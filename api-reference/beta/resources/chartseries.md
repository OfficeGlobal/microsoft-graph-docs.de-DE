---
title: ChartSeries-Ressourcentyp
description: Stellt eine Datenreihe in einem Diagramm dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5a299c7140c2032a57cd47fb0880ae34620a920b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915816"
---
# <a name="chartseries-resource-type"></a>ChartSeries-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine Datenreihe in einem Diagramm dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[ChartSeries abrufen](../api/chartseries-get.md) | [ChartSeries](chartseries.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des chartSeries-Objekts.|
|[ChartPoints erstellen](../api/chartseries-post-points.md) |[ChartPoints](chartpoint.md)| Dient zum Erstellen eines neuen ChartPoints durch Veröffentlichen in der Punkteammlung.|
|[Punkte auflisten](../api/chartseries-list-points.md) |[ChartPoints-Sammlung](chartpoint.md)| Dient zum Abrufen einer ChartPoints-Objeksammlung.|
|[Update](../api/chartseries-update.md) | [ChartSeries](chartseries.md) |Dient zum Aktualisieren des ChartSeries-Objekts. |
|[List](../api/chartseries-list.md) | [ChartSeries-Sammlung](chartseries.md) |Dient zum Abrufen der chartSeries-Objektsammlung. |
|[Itemat](../api/chartseriescollection-itemat.md)|[ChartSeries](chartseries.md)|Ruft eine Datenreihe anhand ihrer Position in der Sammlung ab.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|name|string|Gibt den Namen einer Datenreihe in einem Diagramm an.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|format|[ChartSeriesFormat](chartseriesformat.md)|Stellt die Formatierung für eine Diagrammdatenreihe dar, einschließlich Füllung und Linienformatierung. Schreibgeschützt.|
|points|[ChartPoints-Sammlung](chartpoint.md)|Stellt eine Sammlung aller Punkte in der Datenreihe dar. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartSeries"
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
