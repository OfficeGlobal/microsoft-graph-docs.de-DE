---
title: ChartGridlines-Ressourcentyp
description: Stellt Haupt-Gitternetzlinien oder Hilfs-Gitternetzlinien auf einer Diagrammachse dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3c57c68e7d9dfcd26741d15e302dd5dddeaae378
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572535"
---
# <a name="chartgridlines-resource-type"></a>ChartGridlines-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt Haupt-Gitternetzlinien oder Hilfs-Gitternetzlinien auf einer Diagrammachse dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[ChartGridlines abrufen](../api/chartgridlines-get.md) | [WorkbookChartGridlines](chartgridlines.md) |Dient zum Lesender Eigenschaften und der Beziehungen des chartGridlines-Objekts.|
|[Aktualisieren](../api/chartgridlines-update.md) | [WorkbookChartGridlines](chartgridlines.md)    |Dient zum Aktualisieren des ChartGridlines-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|visible|Boolescher Wert|Boolescher Wert, der angibt, ob die Achsengitternetzlinien angezeigt werden.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|format|[WorkbookChartGridlinesFormat](chartgridlinesformat.md)|Stellt die Formatierung der Diagrammgitternetzlinien dar. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartgridlines.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
