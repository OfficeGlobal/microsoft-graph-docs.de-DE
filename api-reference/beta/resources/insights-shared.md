---
title: Shared-Ressourcentyp
description: 'Einen Einblick, freigegebene mit oder von einem bestimmten Benutzer Dateien darstellt. Die folgenden freigegebenen Dateien werden unterstützt:'
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 11a6989e0130e7eedca7fff6f6cc9790d8109d84
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524688"
---
# <a name="shared-resource-type"></a>Shared-Ressourcentyp

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
| resource      | Entität        | Verwendet zum Navigieren zu dem Element, das freigegeben wurde. Dateianlagen ist der Typ *FileAttachment*. Für verknüpfte Anlagen ist der Typ *DriveItem*. |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

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
