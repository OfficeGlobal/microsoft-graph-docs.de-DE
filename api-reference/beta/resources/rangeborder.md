---
title: RangeBorder-Ressourcentyp
description: Stellt den Rahmen eines Objekts dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5b3b814da53013d1daca686d549596a7ab656027
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515384"
---
# <a name="rangeborder-resource-type"></a>RangeBorder-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt den Rahmen eines Objekts dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|RangeBorder abrufen | RangeBorder |Dient zum Lesen der Eigenschaften und der Beziehungen des rangeBorder-Objekts.|
|[Update](../api/rangeborder-update.md) | RangeBorder |Dient zum Aktualisieren des RangeBorder-Objekts. |
|[List](../api/rangeborder-list.md) | RangeBorder-Sammlung |Dient zum Abrufen der RangeBorder-Objeksammlung. |
|[Itemat](../api/rangebordercollection-itemat.md)|RangeBorder|Dient zum Abrufen eines Rahmenobjekts mithilfe seines Index.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|color|string|HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  „FFA500“) oder als benannte HTML-Farbe (z. B. „orange“) darstellt.|
|id|string|Stellt die Rahmen-ID dar. Mögliche Werte: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Schreibgeschützt.|
|sideIndex|string|Konstanter Wert, der die bestimmte Seite des Rahmens angibt. Mögliche Werte: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Schreibgeschützt.|
|style|string|Eine der Konstanten der Linienart, die die Linienart für den Rahmen angibt. Mögliche Werte: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.|
|weight|string|Gibt die Stärke des Rahmens um einen Bereich an. Mögliche Werte: `Hairline`, `Thin`, `Medium`, `Thick`.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeBorder"
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
<!--
{
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangeborder.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
