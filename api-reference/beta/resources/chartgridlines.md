---
title: ChartGridlines-Ressourcentyp
description: Stellt Haupt-Gitternetzlinien oder Hilfs-Gitternetzlinien auf einer Diagrammachse dar.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 7747564b2f72287ef6ec2c6cc1f912695f58218e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807826"
---
# <a name="chartgridlines-resource-type"></a>ChartGridlines-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt Hauptgitternetzlinien oder Hilfsgitternetzlinien auf einer Diagrammachse dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[ChartGridlines abrufen](../api/chartgridlines-get.md) | [ChartGridlines](chartgridlines.md) |Dient zum Lesender Eigenschaften und der Beziehungen des chartGridlines-Objekts.|
|[Update](../api/chartgridlines-update.md) | [ChartGridlines](chartgridlines.md)    |Dient zum Aktualisieren des ChartGridlines-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|visible|boolean|Boolescher Wert, der angibt, ob die Achsengitternetzlinien angezeigt werden.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|format|[ChartGridlinesFormat](chartgridlinesformat.md)|Stellt die Formatierung der Diagrammgitternetzlinien dar. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartGridLines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
