---
title: Ressourcentyp pivotTable
description: Stellt eine Excel-PivotTable dar.
author: lumine2008
ms.openlocfilehash: 68075aebeac9c0846e48739daf65e5bf97e4d6f5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334111"
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
|id|String| Die ID der PivotTable.   Schreibgeschützt.|
|name|String|Der Name der PivotTable.    |

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
