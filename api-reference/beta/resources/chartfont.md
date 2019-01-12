---
title: ChartFont-Ressourcentyp
description: Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Diagrammobjekt dar.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 4187d2837835520864ec3a1ef5c47b578b3d3da4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920947"
---
# <a name="chartfont-resource-type"></a>ChartFont-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Dieses Objekt stellt die Zeichenformatierung (Schriftart, Schriftgrad, Farbe usw.) für ein Diagrammobjekt dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[ChartFont abrufen](../api/chartfont-get.md) | [ChartFont](chartfont.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des chartFont-Objekts.|
|[Update](../api/chartfont-update.md) | [ChartFont](chartfont.md)   |Dient zum Aktualisieren des ChartFont-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|bold|boolean|Stellt den Fett-Status der Schriftart dar.|
|color|string|HTML-Farbcodedarstellung der Textfarbe. #ff0000 stellt beispielsweise Rot dar.|
|italic|boolean|Stellt den Kursiv-Status der Schriftart dar.|
|name|string|Schriftartname (z. B. "Calibri")|
|size|double|Der Schriftgrad (z. B. 11)|
|underline|string|Art der auf die Schriftart angewendeten Unterstreichung. Mögliche Werte: `None`, `Single`.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartFont"
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
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
