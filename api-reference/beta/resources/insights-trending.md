---
title: Trend Ressourcentyp
description: Rich-Beziehung Herstellen einer Verbindung mit einem Benutzer Dokumente, die auf den Benutzer (für den Benutzer relevant sind) Trend sind. OneDrive-Dateien, und um die Benutzer können Dateien, die auf SharePoint-Teamwebsites trend.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 6a5bd678124a4768303d3cd3ffd4449f4d47bb69
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950746"
---
# <a name="trending-resource-type"></a>Trend Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Rich-Beziehung Herstellen einer Verbindung mit einem Benutzer Dokumente, die auf den Benutzer (für den Benutzer relevant sind) Trend sind. OneDrive-Dateien, und um die Benutzer können Dateien, die auf SharePoint-Teamwebsites trend.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Liste Trend](../api/insights-list-trending.md) |[Insights_trending](insights-trending.md) -Auflistung| Abrufen einer Liste von Trend-Dateien.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft      | Typ                              | Beschreibung  |
| ------------- |---------------                    | -------------|
| id                    | Zeichenfolge                    | Eindeutiger Bezeichner der Beziehung. Schreibgeschützt.        |
| weight                | Gleitkommawert mit doppelter Genauigkeit                    | Der Wert, der angibt, wie viel das Dokument aktuell Trend ist. Je höher die Zahl ist, desto das Dokument ist derzeit Trend um den Benutzer (aussagekräftiger ist es). Zurückgegebene Dokumente werden durch diesen Wert sortiert.  |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)    | Eigenschaften, die Sie verwenden können, um das Dokument in Ihre Erfahrung visualisieren. |
| resourceReference     | [resourceReference](insights-resourcereference.md)        | Referenz-Eigenschaften des Dokuments Trend, wie die Url und den Typ des Dokuments. |

## <a name="relationships"></a>Beziehungen

| Eigenschaft      | Typ          | Beschreibung  |
| ------------- |---------------| -------------|
| resource      | Entität        | Zum Navigieren zu dem Trend Dokument verwendet. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

```json
{
  "id": "string",
  "weight": "double",
  "resourceVisualization": [{"@odata.type": "microsoft.graph.resourceVisualization"}],
  "resourceReference": [{"@odata.type": "microsoft.graph.resourceReference"}],
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
