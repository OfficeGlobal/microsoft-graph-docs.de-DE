---
title: Ressourcentyp pivotTable
description: Stellt eine Excel-PivotTable dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5f6360ce1eacc313f1bcc8a9f59b44b216a87b84
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958740"
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
