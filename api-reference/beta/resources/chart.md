---
title: Chart-Ressourcentyp
description: Steht für ein Diagrammobjekt in einer Arbeitsmappe.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 09d5fd376cfdcd03517cc989708bbf17bcf49a72
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970675"
---
# <a name="chart-resource-type"></a>Chart-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Steht für ein Diagrammobjekt in einer Arbeitsmappe.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Chart abrufen](../api/chart-get.md) | [Chart](chart.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des chart-Objekts.|
|[ChartSeries erstellen](../api/chart-post-series.md) |[ChartSeries](chartseries.md)| Dient zum Erstellen einer neuen ChartSeries durch Veröffentlichen in der Datenreihensammlung.|
|[Reihe auflisten](../api/chart-list-series.md) |[ChartSeries-Sammlung](chartseries.md)| Dient zum Abrufen einer ChartSeries-Objektsammlung.|
|[Update](../api/chart-update.md) | [Chart](chart.md)   |Dient zum Aktualisieren des Chart-Objekts. |
|[Image](../api/chart-image.md)|Abbildung der base64-codierten Zeichenfolge|Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.|
|[Delete](../api/chart-delete.md)|Keine|Löscht das Diagrammobjekt.|
|[Setdata](../api/chart-setdata.md)|Keine|Setzt die Quelldaten für das Diagramm zurück.|
|[Setposition](../api/chart-setposition.md)|Keine|Positioniert das Diagramm im Verhältnis zu den Zellen im Arbeitsblatt.|
|[List](../api/chart-list.md) | [Diagrammsammlung](chart.md) |Dient zum Abrufen der Diagrammobjeksammlung. |
|[Itemat](../api/chartcollection-itemat.md)|[Chart](chart.md)|Ruft ein Diagramm anhand seiner Position in der Sammlung ab.|
|[Add](../api/chartcollection-add.md)|[Chart](chart.md)|Erstellt ein neues Diagramm.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|height|double|Die Höhe des Diagrammobjekts (in Punkten).|
|id|string|Ruft ein Diagramm anhand seiner Position in der Sammlung ab. Schreibgeschützt.|
|left|double|Der Abstand von der linken Seite des Diagramms zu dem Ursprung des Arbeitsblatts (in Punkten).|
|name|string|Gibt den Namen eines Diagrammobjekts an.|
|top|double|Der Abstand (in Punkten) von dem oberen Rand des Objekts zum oberen Rand von Zeile 1 (auf einem Arbeitsblatt) oder zum oberen Diagrammbereich (in einem Diagramm).|
|width|double|Die Breite des Diagrammobjekts (in Punkten).|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Achsen|[ChartAxes](chartaxes.md)|Die Achsen des Diagramms. Schreibgeschützt.|
|dataLabels|[ChartDataLabels](chartdatalabels.md)|Stellt die Datenbeschriftungen im Diagramm dar. Schreibgeschützt.|
|Format|[ChartAreaFormat](chartareaformat.md)|Kapselt die Formateigenschaften für den Diagrammbereich. Schreibgeschützt.|
|legend|[ChartLegend](chartlegend.md)|Die Legende für das Diagramm. Schreibgeschützt.|
|series|[ChartSeries-Sammlung](chartseries.md)|Eine einzelne Datenreihe oder eine Sammlung von Datenreihen im Diagramm. Schreibgeschützt.|
|title|[ChartTitle](charttitle.md)|Der Titel des angegebenen Diagramms, einschließlich Text, Sichtbarkeit, Position und Formatierung des Titels. Schreibgeschützt.|
|Arbeitsblatt|[Worksheet](worksheet.md)|Das Arbeitsblatt, das das aktuelle Diagramm enthält. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chart"
}-->

```json
{
  "height": 1024,
  "id": "string",
  "left": 1024,
  "name": "string",
  "top": 1024,
  "width": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
