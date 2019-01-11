---
title: Ressourcentyp imageInfo
description: Einen komplexen Typ für die **Zuweisung** -Eigenschaft im VisualInfo Teil des Aktivität-Objekts darstellt.
localization_priority: Normal
ms.openlocfilehash: 2bac97ff945c0e0975ffa19636a954308b895e88
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856462"
---
# <a name="imageinfo-resource-type"></a>Ressourcentyp imageInfo

Einen komplexen Typ für die **Zuweisung** -Eigenschaft im [VisualInfo](../resources/projectrome-visualinfo.md) Teil des [Aktivität](../resources/projectrome-activity.md) -Objekts darstellt.

## <a name="properties"></a>Eigenschaften

|Name | Typ | Beschreibung|
|:----|:-----|:-----------|
|iconUrl | String | Optional; URI, der auf ein Symbol, die die Anwendung verwendet verweist, um die Aktivität generieren darstellt.|
|alternateText | String | Optional; ALT-Text zugegriffen werden Inhalte für das Bild|
|addImageQuery | Boolean | Optional; Parameter verwendet, um den Server anzugeben kann dynamisch als Reaktion auf Parametrisierung Bild zu rendern. Beispiel – ein hoher Kontrast-Bild|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
