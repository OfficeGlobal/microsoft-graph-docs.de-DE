---
title: Ressourcentyp usedInsight
description: Einen Einblick, Dokumente, die von einem bestimmten Benutzer darstellt. Einblicke in die gibt, die zutreffenden Dokumente, die ein Benutzer anzeigen oder darauf zugreifen.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 056654a5e467e202b2bde5ac8ee98dccab93d7c9
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574229"
---
# <a name="used-resource-type"></a>Ressourcentyp verwendet

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Einen Einblick, Dokumente, die von einem bestimmten Benutzer darstellt. Einblicke in die gibt, die zutreffenden Dokumente, die ein Benutzer anzeigen oder darauf zugreifen. Dazu gehören Dokumente in:

- OneDrive for Business
- SharePoint

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Verwendet wird](../api/insights-list-used.md) |[Insights_used](insights-used.md) -Auflistung| Rufen Sie eine Liste der geöffneten Dateien.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft              | Typ                      | Beschreibung  |
| -------------         |---------------            | -------------|
| id                    | String                    | Eindeutiger Bezeichner der Beziehung. Schreibgeschützt.        |
| lastUsed              | [usageDetails](insights-usagedetails.md)              | Wenn das Element zuletzt Informationen angezeigt und vom Benutzer geändert. Schreibgeschützt.     |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | Eigenschaften, die Sie verwenden können, um das Dokument in Ihre Erfahrung visualisieren. Schreibgeschützt      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Referenz-Eigenschaften des Dokuments verwendete, wie die Url und den Typ des Dokuments. Schreibgeschützt     |

## <a name="relationships"></a>Beziehungen

| Eigenschaft      | Typ          | Beschreibung  |
| ------------- |---------------| -------------|
| resource      | Entity-Auflistung | Verwendet zum Navigieren zu dem Element, das verwendet wurde. Dateianlagen ist der Typ *FileAttachment*. Für verknüpfte Anlagen ist der Typ *DriveItem*. |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.usedInsight"
}-->
```json
{
  "id": "string",
  "lastUsed": "usageDetails",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-used.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
