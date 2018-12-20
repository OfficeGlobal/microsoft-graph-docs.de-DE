---
title: Ressourcentyp mediaPrompt
description: Der Typ des MediaPrompt.
author: VinodRavichandran
ms.openlocfilehash: 4782772f463a613a759ad3b2b25cb05e7e160555
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380289"
---
# <a name="mediaprompt-resource-type"></a>Ressourcentyp mediaPrompt

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Der Typ des MediaPrompt.

## <a name="properties"></a>Eigenschaften

| Eigenschaft    | Typ                      | Beschreibung                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| Schleife        | Int32                     | Die Anzahl der Schleifen. Wert 0 gibt an, dass Endlosschleife ausgeführt. Der Standardwert lautet `1`. |
| mediaInfo   | [mediaInfo](mediainfo.md) | Die Medieninformationen                                                           |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "loop": 1024,
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

## <a name="example"></a>Beispiel

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->
```json
{
  "mediaInfo": {
    "uri": "https://cdn.contoso.com/beep.wav",
    "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
  },
  "loop": 5
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
