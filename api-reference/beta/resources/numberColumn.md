---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: a0f5d13381c82a42159d0802d850d9996aaf8b54
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855181"
---
# <a name="numbercolumn-resource-type"></a>NumberColumn-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
| **decimalPlaces**  | string | Wie viele Dezimalstellen angezeigt werden sollen. Informationen zu den möglichen Werten finden Sie weiter unten.
| **displayAs**      | string | Wie sollte der Wert in der UX dargestellt werden. Müssen `number` oder `percentage` sein. Wenn nicht angegeben, werden sie als `number` behandelt.
| **maximum**        | double | Der maximal zulässige Wert.
| **minimum**        | double | Der minimal zulässige Wert.

## <a name="decimalplaces-values"></a>DecimalPlaces-Werte

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
  "tocPath": "Resources/NumberColumn"
} -->
