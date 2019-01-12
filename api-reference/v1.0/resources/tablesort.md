---
title: TableSort-Ressourcentyp
description: Verwaltet Sortiervorgänge für Table-Objekte.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: be607832be82b99853b4cd44cfa5b60449a2c432
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929473"
---
# <a name="tablesort-resource-type"></a>TableSort-Ressourcentyp

Verwaltet Sortiervorgänge für Table-Objekte.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Get TableSort](../api/tablesort-get.md) | [WorkbookTableSort](tablesort.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des tableSort-Objekts.|
|[Apply](../api/tablesort-apply.md)|Keine|Führt einen Sortiervorgang aus.|
|[Clear](../api/tablesort-clear.md)|Keine|Löscht die Sortierung, die derzeit in der Tabelle enthalten ist. Dies ändert nicht die Sortierung der Tabelle, löscht jedoch den Zustand der Kopfzeilen-Schaltflächen.|
|[Reapply](../api/tablesort-reapply.md)|Keine|Wendet die aktuellen Sortierparameter erneut auf die Tabelle an.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|fields|[WorkbookSortField](sortfield.md) -Auflistung|Stellt die aktuellen Bedingungen dar, die zuletzt zum Sortieren der Tabelle verwendet wurden. Schreibgeschützt.|
|matchCase|boolean|Stellt dar, ob die Groß-/Kleinschreibung den letzten Sortiervorgang der Tabelle beeinflusst hat. Schreibgeschützt.|
|method|string|Stellt Chinesisches Zeichen Sortierung Methode zuletzt verwendet, um die Tabelle zu sortieren. Die möglichen Werte sind: `PinYin`, `StrokeCount`. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
