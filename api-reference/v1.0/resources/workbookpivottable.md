---
title: Ressourcentyp pivotTable
description: Stellt eine Excel-PivotTable dar.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: d500d4bc88608b032262cfae505385bf7ed3f072
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889208"
---
# <a name="pivottable-resource-type"></a>Ressourcentyp pivotTable

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
|id|Zeichenfolge| Die ID der PivotTable.   Schreibgeschützt.|
|name|Zeichenfolge|Der Name der PivotTable.    |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Arbeitsblatt|[WorkbookWorksheet](worksheet.md)| Das Arbeitsblatt, das die aktuelle PivotTable enthält. Schreibgeschützt.   |

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
