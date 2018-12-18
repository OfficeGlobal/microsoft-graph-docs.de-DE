---
title: TableRow-Ressourcentyp
description: Stellt eine Zeile in einer Tabelle dar.
author: lumine2008
ms.openlocfilehash: de83ec8cae87f159c6f1f9687bd093873558c150
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309884"
---
# <a name="tablerow-resource-type"></a>TableRow-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine Zeile in einer Tabelle dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[TableRow abrufen](../api/tablerow-get.md) | [TableRow](tablerow.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des tableRow-Objekts.|
|[Update](../api/tablerow-update.md) | [TableRow](tablerow.md)  |Dient zum Aktualisieren des TableRow-Objekts. |
|[Range](../api/tablerow-range.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das mit der gesamten Zeile verknüpft ist.|
|[Delete](../api/tablerow-delete.md)|Keine|Löscht die Zeile aus der Tabelle.|
|[List](../api/tablerow-list.md) | [TableRow](tablerow.md)-Sammlung |Dient zum Abrufen einer tableRow-Objektsammlung. |
|[Itemat](../api/tablerowcollection-itemat.md)|[TableRow](tablerow.md)|Ruft eine Zeile anhand ihrer Position in der Auflistung ab.|
|[Add](../api/tablerowcollection-add.md)|[TableRow](tablerow.md)|Fügt der Tabelle eine neue Zeile hinzu.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Index|int|Gibt die Indexnummer der Zeile in der Zeilenauflistung der Tabelle zurück. Nullindiziert. Schreibgeschützt.|
|values|json|Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableRow"
}-->

```json
{
  "index": 1024,
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->