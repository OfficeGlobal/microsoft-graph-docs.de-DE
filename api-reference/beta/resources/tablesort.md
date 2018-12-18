---
title: TableSort-Ressourcentyp
description: Verwaltet Sortiervorgänge für Table-Objekte.
author: lumine2008
ms.openlocfilehash: 52ee5288698b236f7ee4d29eb75fdac5ad14fa0f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339823"
---
# <a name="tablesort-resource-type"></a>TableSort-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Verwaltet Sortiervorgänge für Table-Objekte.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Get TableSort](../api/tablesort-get.md) | [TableSort](tablesort.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des tableSort-Objekts.|
|[Apply](../api/tablesort-apply.md)|Keine|Führt einen Sortiervorgang aus.|
|[Löschen](../api/tablesort-clear.md)|Keine|Löscht die Sortierung, die derzeit in der Tabelle enthalten ist. Dies ändert nicht die Sortierung der Tabelle, löscht jedoch den Zustand der Kopfzeilen-Schaltflächen.|
|[Reapply](../api/tablesort-reapply.md)|Keine|Wendet die aktuellen Sortierparameter erneut auf die Tabelle an.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|matchCase|boolean|Stellt dar, ob die Groß-/Kleinschreibung den letzten Sortiervorgang der Tabelle beeinflusst hat. Schreibgeschützt.|
|method|string|Stellt die chinesische Zeichensortiermethode dar, mit der die Tabelle zuletzt sortiert wurde. Die folgenden Werte sind möglich: `PinYin`, `StrokeCount`. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|fields|[SortField](sortfield.md)|Stellt die aktuellen Bedingungen dar, die zuletzt zum Sortieren der Tabelle verwendet wurden. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string"
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