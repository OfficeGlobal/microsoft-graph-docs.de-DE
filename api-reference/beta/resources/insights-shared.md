---
title: freigegebene Ressource-Typ
description: 'Einen Einblick, freigegebene mit oder von einem bestimmten Benutzer Dateien darstellt. Die folgenden freigegebenen Dateien werden unterstützt:'
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 49e18318c1e93d2393b957b404ff4617b334f237
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573179"
---
# <a name="shared-resource-type"></a>freigegebene Ressource-Typ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Einen Einblick, freigegebene mit oder von einem bestimmten Benutzer Dateien darstellt. Die folgenden freigegebenen Dateien werden unterstützt:

- Anlagen direkt in eine e-Mail oder eine Besprechung einladen.
- OneDrive für Bussiness und SharePoint modernen Anlagen - Dateien in OneDrive für Unternehmen und SharePoint, die Benutzer in einer e-Mail als ein Links freigeben.

**Hinweis**: Wir arbeiten derzeit auf die Ergebnisse der Shared-API mit Daten auffüllen. Möglicherweise gibt es einige Daten in den ersten Wochen nach der Veröffentlichung fehlt.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Gemeinsame Liste](../api/insights-list-shared.md) |[Insights_shared](insights-shared.md) -Auflistung| Rufen Sie eine Liste der freigegebenen Dateien.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft              | Typ                      | Beschreibung  |
| -------------         |---------------            | -------------|
| id                    | String                    | Eindeutiger Bezeichner der Beziehung. Schreibgeschützt.        |
| lastShared            | [sharingDetail](insights-sharingdetail.md)                | Informationen zu freigegebenen Elements. Schreibgeschützt.        |
| resourceVisualization | [resourceVisualization](insights-resourcevisualization.md)                | Eigenschaften, die Sie verwenden können, um das Dokument in Ihre Erfahrung visualisieren. Schreibgeschützt      |
| resourceReference     | [resourceReference](insights-resourcereference.md)                      | Referenz-Eigenschaften des freigegebenen Dokuments, wie die Url und den Typ des Dokuments. Schreibgeschützt       |

## <a name="relationships"></a>Beziehungen

| Eigenschaft      | Typ          | Beschreibung  |
| ------------- |---------------| -------------|
| resource      | Entity-Auflistung | Verwendet zum Navigieren zu dem Element, das freigegeben wurde. Dateianlagen ist der Typ *FileAttachment*. Für verknüpfte Anlagen ist der Typ *DriveItem*. |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.shared"
}-->
```json
{
  "id": "string",
  "lastShared": "sharingDetail",
  "resourceVisualization": "resourceVisualization",
  "resourceReference": "resourceReference",
  
  "resource": [ { "@odata.type": "microsoft.graph.entity" } ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
