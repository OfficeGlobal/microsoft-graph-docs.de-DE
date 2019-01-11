---
title: ChartLineFormat-Ressourcentyp
description: Kapselt die Formatierungsoptionen für Linienelemente.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: b2b7e8bd5c0b489ed42baaa3939f7a839c74c3e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871134"
---
# <a name="chartlineformat-resource-type"></a>ChartLineFormat-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Kapselt die Formatierungsoptionen für Linienelemente.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[ChartLineFormat abrufen](../api/chartlineformat-get.md) | [ChartLineFormat](chartlineformat.md) |Dient zum Lesen der Eigenschaften und Beziehungen eines chartLineFormat-Objekts.|
|[Update](../api/chartlineformat-update.md) | [ChartLineFormat](chartlineformat.md) |Dient zum Aktualisieren des ChartLineFormat-Objekts. |
|[Clear](../api/chartlineformat-clear.md)|Keine|Löschen der Linienformatierung eines Diagrammelements.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|color|string|HTML-Farbcode, der die Farbe der Linien im Diagramm darstellt.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
