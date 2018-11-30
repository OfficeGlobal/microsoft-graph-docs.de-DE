---
title: RangeFill-Ressourcentyp
description: Stellt den Hintergrund eines Bereichsobjekts dar.
ms.openlocfilehash: 11806d95900c6e4ea1d4bf6ce4f4800bf5f6f66b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064978"
---
# <a name="rangefill-resource-type"></a>RangeFill-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt den Hintergrund eines Bereichsobjekts dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[RangeFill abrufen](../api/rangefill-get.md) | [RangeFill](rangefill.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFill-Objekts.|
|[Update](../api/rangefill-update.md) | [RangeFill](rangefill.md)   |Dient zum Aktualisieren des RangeFill-Objekts. |
|[Löschen](../api/rangefill-clear.md)|Keine|Setzt den Hintergrund des Bereichs zurück.|

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
<!-- {
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->