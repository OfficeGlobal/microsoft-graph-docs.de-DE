---
title: RangeFont-Ressourcentyp
description: Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Objekt dar.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: e6f448df142ffdc0c20e39045b4cd77a6c224a6f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912778"
---
# <a name="rangefont-resource-type"></a>RangeFont-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Objekt dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[RangeFont abrufen](../api/rangefont-get.md) | [RangeFont](rangefont.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFont-Objekts.|
|[Update](../api/rangefont-update.md) | [RangeFont](rangefont.md)   |Dient zum Aktualisieren des RangeFont-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|bold|boolean|Stellt den Fett-Status der Schriftart dar.|
|color|string|HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.|
|italic|boolean|Stellt den Kursiv-Status der Schriftart dar.|
|name|string|Schriftartname (z. B. "Calibri")|
|size|double|Schriftgrad|
|underline|string|Art der auf die Schriftart angewendete Unterstreichung. Die folgenden Werte sind möglich: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
