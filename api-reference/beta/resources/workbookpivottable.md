---
title: Ressourcentyp pivotTable
description: Stellt eine Excel-PivotTable dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fc43bf160e93e354ff58b2f960e8ec38d252287f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520459"
---
# <a name="pivottable-resource-type"></a>Ressourcentyp pivotTable

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine Excel-PivotTable dar.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[workbookPivotTable abrufen](../api/workbookpivottable-get.md) | [workbookPivotTable](workbookpivottable.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des workbookPivotTable-Objekts.|
|[Aktualisieren](../api/workbookpivottable-refresh.md)|Keine|Aktualisiert die PivotTable. |
|[Refreshall](../api/workbookpivottable-refreshall.md)|Keine|Aktualisiert alle Tabellen im gegebenen Arbeitsblatt. Beachten Sie, dass diese Aktion nur für die PivotTable-Sammlung verfügbar ist.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Die ID der PivotTable.   Schreibgeschützt.|
|name|String|Der Name der PivotTable.    |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Arbeitsblatt|[Arbeitsblatt](worksheet.md)| Das Arbeitsblatt, das die aktuelle PivotTable enthält. Schreibgeschützt.   |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/workbookpivottable.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
