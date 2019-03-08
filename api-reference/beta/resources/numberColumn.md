---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: edd495b62f0ccbd163ec31a2efca70923d0bc8ad
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480768"
---
# <a name="numbercolumn-resource-type"></a>NumberColumn-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/numberColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
