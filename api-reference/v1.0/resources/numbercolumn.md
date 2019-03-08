---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: 42824275bd79f4b631d53365997d2dd96984f7b5
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480852"
---
# <a name="numbercolumn-resource-type"></a>NumberColumn-Ressourcentyp

Die **numberColumn** einer [columnDefinition](columndefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Zahlen handelt.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung einer **numberColumn**-Ressource.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a>Eigenschaften

| Eigenschaftenname      | Typ   | Beschreibung
|:-------------------|:-------|:-----------------------------------------------
| **decimalPlaces**  | Zeichenfolge | Wie viele Dezimalstellen angezeigt werden sollen. Informationen zu den möglichen Werten finden Sie weiter unten.
| **displayAs**      | string | Wie sollte der Wert in der UX dargestellt werden. Müssen `number` oder `percentage` sein. Wenn nicht angegeben, werden sie als `number` behandelt.
| **maximum**        | double | Der maximal zulässige Wert.
| **minimum**        | double | Der minimal zulässige Wert.

## <a name="decimalplaces"></a>DecimalPlaces

| Wert          | Beschreibung
|:---------------|:--------------------------------------------------------------
| **automatic**  | Standard. Dezimalstellen werden je nach Bedarf automatisch angezeigt.
| **none**       | Keine Dezimalstellen anzuzeigen.
| **one**        | Immer eine Dezimalstelle anzeigen.
| **two**        | Immer zwei Dezimalstellen anzeigen.
| **three**      | Immer drei Dezimalstellen anzeigen.
| **four**       | Immer vier Dezimalstellen anzeigen.
| **five**       | Immer füng Dezimalstellen anzeigen.

Hinweis: **decimalPlaces** und **displayAs** trifft darauf zu, wie Zahlen gerendert, nicht gespeichert werden.
Diese Eigenschaften können aktualisiert werden.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(automatic,none,one,two,three,four,five) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(number,percentage) are in resource, but () are in table"
  ],
  "tocPath": "Resources/NumberColumn"
} -->
