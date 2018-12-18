---
title: RangeFill-Ressourcentyp
description: Stellt den Hintergrund eines Bereichsobjekts dar.
author: lumine2008
ms.openlocfilehash: 6ddd039190af0e86067dfda651b2bc387b4cf74f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303563"
---
# <a name="rangefill-resource-type"></a>RangeFill-Ressourcentyp

Stellt den Hintergrund eines Bereichsobjekts dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[RangeFill abrufen](../api/rangefill-get.md) | [WorkbookRangeFill](rangefill.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFill-Objekts.|
|[Update](../api/rangefill-update.md) | [WorkbookRangeFill](rangefill.md)   |Dient zum Aktualisieren des RangeFill-Objekts. |
|[Löschen](../api/rangefill-clear.md)|Keine|Setzt den Hintergrund des Bereichs zurück.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|color|string|HTML-Farbcode, der die Farbe der Rahmenlinie, des Formulars #RRGGBB (z. B.  "FFA500") oder als benannte HTML-Farbe (z. B. "orange") darstellt.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFill"
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
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->