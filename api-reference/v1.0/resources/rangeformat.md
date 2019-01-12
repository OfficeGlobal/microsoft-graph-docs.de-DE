---
title: RangeFormat-Ressourcentyp
description: Gibt ein Formatobjekt zurück, das die Schriftart des Bereichs, Füllung, Rahmen, die Ausrichtung und andere Eigenschaften verschachtelt.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: f0e57522812b966c39a6981de964e786d33c5006
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919211"
---
# <a name="rangeformat-resource-type"></a>RangeFormat-Ressourcentyp

Gibt ein Formatobjekt zurück, das die Schriftart des Bereichs, Füllung, Rahmen, die Ausrichtung und andere Eigenschaften verschachtelt.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[RangeFormat abrufen](../api/rangeformat-get.md) | [WorkbookRangeFormat](rangeformat.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFormat-Objekts.|
|[RangeBorder erstellen](../api/rangeformat-post-borders.md) |[WorkbookRangeBorder](rangeborder.md)| Dient zum Erstellen eines neues RangeBorder durch Veröffentlichen in der Rahmensammlung.|
|[Rahmen auflisten](../api/rangeformat-list-borders.md) |[WorkbookRangeBorder](rangeborder.md) -Auflistung| Dient zum Abrufen einer RangeBorder-Objeksammlung.|
|[Update](../api/rangeformat-update.md) | [WorkbookRangeFormat](rangeformat.md) |Dient zum Aktualisieren des RangeFormat-Objekts. |
|[Autofitcolumns](../api/rangeformat-autofitcolumns.md)|Keine|Ändert die Breite der Spalten des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Spalten die optimale Breite zu erzielen.|
|[Autofitrows](../api/rangeformat-autofitrows.md)|Keine|Ändert die Höhe der Zeilen des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Zeilen die optimale Höhe zu erzielen.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|columnWidth|double|Ruft die Breite aller Spalten innerhalb des Bereichs ab oder legt diese fest. Wenn die Breite der Spalten nicht gleichmäßig ist, wird Null zurückgegeben.|
|horizontalAlignment|string|Die horizontale Ausrichtung für das angegebene Objekt darstellt. Die möglichen Werte sind: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.|
|rowHeight|double|Ruft die Höhe aller Zeilen des Bereichs ab oder legt diese fest. Wenn die Höhe der Zeilen nicht gleichmäßig ist, wird Null zurückgegeben.|
|verticalAlignment|string|Die vertikale Ausrichtung für das angegebene Objekt darstellt. Die möglichen Werte sind: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.|
|wrapText|boolean|Gibt an, ob Excel den Text im Objekt umbricht. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Textumbruch-Einstellung hat|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Borders|[WorkbookRangeBorder](rangeborder.md) -Auflistung|Auflistung von Border-Objekten, die für den gesamten ausgewählten Bereich gelten, schreibgeschützt.|
|fill|[WorkbookRangeFill](rangefill.md)|Gibt das Fill-Objekt an, das für den gesamten Bereich definiert ist. Schreibgeschützt.|
|Schriftart|[WorkbookRangeFont](rangefont.md)|Gibt das Font-Objekt zurück, das für den gesamten ausgewählten Bereich definiert ist, schreibgeschützt.|
|protection|[WorkbookFormatProtection](formatprotection.md)|Gibt das Formatschutz-Objekt für einen Bereich zurück. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeFormat"
}-->

```json
{
  "columnWidth": 1024,
  "horizontalAlignment": "string",
  "rowHeight": 1024,
  "verticalAlignment": "string",
  "wrapText": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
