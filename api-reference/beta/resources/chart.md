---
title: Chart-Ressourcentyp
description: Steht für ein Diagrammobjekt in einer Arbeitsmappe.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: b038ecc79f497a2c52cda180217f290c7fb2de6a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572003"
---
# <a name="chart-resource-type"></a>Chart-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Steht für ein Diagrammobjekt in einer Arbeitsmappe.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Chart abrufen](../api/chart-get.md) | [WorkbookChart](chart.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des chart-Objekts.|
|[ChartSeries erstellen](../api/chart-post-series.md) |[WorkbookChartSeries](chartseries.md)| Dient zum Erstellen einer neuen ChartSeries durch Veröffentlichen in der Datenreihensammlung.|
|[Reihe auflisten](../api/chart-list-series.md) |[WorkbookChartSeries](chartseries.md) -Auflistung| Dient zum Abrufen einer ChartSeries-Objektsammlung.|
|[Aktualisieren](../api/chart-update.md) | [WorkbookChart](chart.md)   |Dient zum Aktualisieren des Chart-Objekts. |
|[Image](../api/chart-image.md)|Abbildung der base64-codierten Zeichenfolge|Rendert das Diagramm als base64-codiertes Bild durch Skalierung, um es an die angegebenen Maße anzupassen.|
|[Löschen](../api/chart-delete.md)|Keine|Löscht das Diagrammobjekt.|
|[Setdata](../api/chart-setdata.md)|Keine|Setzt die Quelldaten für das Diagramm zurück.|
|[Setposition](../api/chart-setposition.md)|Keine|Positioniert das Diagramm im Verhältnis zu den Zellen im Arbeitsblatt.|
|[List](../api/chart-list.md) | [WorkbookChart](chart.md) -Auflistung |Dient zum Abrufen der Diagrammobjeksammlung. |
|[Itemat](../api/chartcollection-itemat.md)|[WorkbookChart](chart.md)|Ruft ein Diagramm anhand seiner Position in der Sammlung ab.|
|[Add](../api/chartcollection-add.md)|[WorkbookChart](chart.md)|Erstellt ein neues Diagramm.|

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
|Achsen|[WorkbookChartAxes](chartaxes.md)|Die Achsen des Diagramms. Schreibgeschützt.|
|dataLabels|[WorkbookChartDataLabels](chartdatalabels.md)|Stellt die Datenbeschriftungen im Diagramm dar. Schreibgeschützt.|
|Format|[WorkbookChartAreaFormat](chartareaformat.md)|Kapselt die Formateigenschaften für den Diagrammbereich. Schreibgeschützt.|
|legend|[WorkbookChartLegend](chartlegend.md)|Die Legende für das Diagramm. Schreibgeschützt.|
|series|[WorkbookChartSeries](chartseries.md) -Auflistung|Eine einzelne Datenreihe oder eine Sammlung von Datenreihen im Diagramm. Schreibgeschützt.|
|title|[WorkbookChartTitle](charttitle.md)|Der Titel des angegebenen Diagramms, einschließlich Text, Sichtbarkeit, Position und Formatierung des Titels. Schreibgeschützt.|
|Arbeitsblatt|[WorkbookWorksheet](worksheet.md)|Das Arbeitsblatt, das das aktuelle Diagramm enthält. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChart"
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
<!--
{
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
