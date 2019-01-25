---
title: RangeFill-Ressourcentyp
description: Stellt den Hintergrund eines Bereichsobjekts dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d1ae60c0b362ba8593f374c5edd505121cd18587
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509672"
---
# <a name="rangefill-resource-type"></a>RangeFill-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt den Hintergrund eines Bereichsobjekts dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|RangeFill abrufen | RangeFill |Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFill-Objekts.|
|[Update](../api/rangefill-update.md) | RangeFill   |Dient zum Aktualisieren des RangeFill-Objekts. |
|[Clear](../api/rangefill-clear.md)|Keine|Setzt den Hintergrund des Bereichs zurück.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|color|string|HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  "FFA500") oder als benannte HTML-Farbe (z. B. "orange") darstellt.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangefill.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
