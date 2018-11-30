---
title: RangeBorder-Ressourcentyp
description: Stellt den Rahmen eines Objekts dar.
ms.openlocfilehash: 30d5548ba867dc652c700985d65a6db01ce8bc99
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017052"
---
# <a name="rangeborder-resource-type"></a>RangeBorder-Ressourcentyp

Stellt den Rahmen eines Objekts dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[RangeBorder abrufen](../api/rangeborder-get.md) | [WorkbookRangeBorder](rangeborder.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des rangeBorder-Objekts.|
|[Update](../api/rangeborder-update.md) | [WorkbookRangeBorder](rangeborder.md) |Dient zum Aktualisieren des RangeBorder-Objekts. |
|[List](../api/rangeborder-list.md) | [WorkbookRangeBorder](rangeborder.md) -Auflistung |Dient zum Abrufen der RangeBorder-Objeksammlung. |
|[Itemat](../api/rangebordercollection-itemat.md)|[WorkbookRangeBorder](rangeborder.md)|Dient zum Abrufen eines Rahmenobjekts mithilfe seines Index.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|color|string|HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  „FFA500“) oder als benannte HTML-Farbe (z. B. „orange“) darstellt.|
|id|string|Stellt Rahmen Bezeichner. Die möglichen Werte sind: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Schreibgeschützt.|
|sideIndex|string|Konstanter Wert, der angibt, die bestimmte Seiten des Rahmens. Die möglichen Werte sind: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Schreibgeschützt.|
|style|string|Eine der Konstanten der Linienart die Linienart für den Rahmen angeben. Die möglichen Werte sind: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.|
|weight|string|Gibt die Stärke des Rahmens um einen Bereich an. Die möglichen Werte sind: `Hairline`, `Thin`, `Medium`, `Thick`.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->