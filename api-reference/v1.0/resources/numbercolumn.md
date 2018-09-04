---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 4aaff6539fc9c7ce77029463562c0f8fca57cac6
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23266506"
---
# <a name="numbercolumn-resource-type"></a>NumberColumn-Ressourcentyp

Die **numberColumn** einer [columnDefinition](columnDefinition.md)-Ressource gibt an, dass es sich bei den Spaltenwerten um Zahlen handelt.

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
| **displayAs**      | Zeichenfolge | Wie sollte der Wert in der UX dargestellt werden. Müssen `number` oder `percentage` sein. Wenn nicht angegeben, werden sie als `number` behandelt.
| **maximum**        | doppelt | Der maximal zulässige Wert.
| **minimum**        | doppelt | Der minimal zulässige Wert.

## <a name="decimalplaces"></a>DecimalPlaces

| Wert          | Beschreibung
|:---------------|:--------------------------------------------------------------
| **Automatisch**  | Standard. Dezimalstellen werden je nach Bedarf automatisch angezeigt.
| **keine**       | Keine Dezimalstellen anzuzeigen.
| **eine**        | Immer eine Dezimalstelle anzeigen.
| **zwei**        | Immer zwei Dezimalstellen anzeigen.
| **drei**      | Immer drei Dezimalstellen anzeigen.
| **vier**       | Immer vier Dezimalstellen anzeigen.
| **fünf**       | Immer füng Dezimalstellen anzeigen.

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
