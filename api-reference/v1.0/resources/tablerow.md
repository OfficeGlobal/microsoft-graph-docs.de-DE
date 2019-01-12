---
title: TableRow-Ressourcentyp
description: Stellt eine Zeile in einer Tabelle dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c266476715da36bcdc0b621538722ba6320eba85
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937509"
---
# <a name="tablerow-resource-type"></a>TableRow-Ressourcentyp

Stellt eine Zeile in einer Tabelle dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[TableRow abrufen](../api/tablerow-get.md) | [WorkbookTableRow](tablerow.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des tableRow-Objekts.|
|[Update](../api/tablerow-update.md) | [WorkbookTableRow](tablerow.md)  |Dient zum Aktualisieren des TableRow-Objekts. |
|[Range](../api/tablerow-range.md)|[Range](range.md)|Ruft das Bereichsobjekt ab, das mit der gesamten Zeile verknüpft ist.|
|[Delete](../api/tablerow-delete.md)|Keine|Löscht die Zeile aus der Tabelle.|
|[List](../api/tablerow-list.md) | [WorkbookTableRow](tablerow.md) -Auflistung |Dient zum Abrufen einer tableRow-Objektsammlung. |
|[Itemat](../api/tablerowcollection-itemat.md)|[WorkbookTableRow](tablerow.md)|Ruft eine Zeile anhand ihrer Position in der Auflistung ab.|
|[Add](../api/tablerowcollection-add.md)|[WorkbookTableRow](tablerow.md)|Fügt der Tabelle eine neue Zeile hinzu.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Index|int|Gibt die Indexnummer der Zeile in der Zeilenauflistung der Tabelle zurück. Nullindiziert. Schreibgeschützt.|
|values|Json|Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableRow"
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
