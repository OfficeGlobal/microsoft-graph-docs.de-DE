---
title: Ressourcentyp mediaPrompt
description: Der Typ des MediaPrompt.
ms.openlocfilehash: 1a782d391110d35b07b551e44ebd3b931dbcadba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064244"
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
