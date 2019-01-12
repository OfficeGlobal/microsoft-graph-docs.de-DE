---
title: ChartPoint-Ressourcentyp
description: Stellt einen Punkt einer Datenreihe in einem Diagramm dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 66c58e08063bd9757ad9c174e81f35328dd2722b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912757"
---
# <a name="chartpoint-resource-type"></a>ChartPoint-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt einen Punkt einer Datenreihe in einem Diagramm dar.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[ChartPoint abrufen](../api/chartpoint-get.md) | [ChartPoint](chartpoint.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des chartPoint-Objekts.|
|[List](../api/chartpoint-list.md) | [ChartPoint-Sammlung](chartpoint.md) |Dient zum Abrufen der ChartPoint-Objektsammlung. |
|[Itemat](../api/chartpointscollection-itemat.md)|[ChartPoint](chartpoint.md)|Abrufen eines Punkts anhand seiner Position in der Datenreihe.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Wert|object|Gibt den Wert eines Diagrammpunkts zurück. Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|format|[ChartPointFormat](chartpointformat.md)|Kapselt die Formateigenschaften eines Diagrammpunkts. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartPoint"
}-->

```json
{
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
