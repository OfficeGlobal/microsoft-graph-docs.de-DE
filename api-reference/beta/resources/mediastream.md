---
title: Ressourcentyp mediaStream
description: Der Typ des MediaStream.
author: VinodRavichandran
ms.openlocfilehash: f870611700289f0254272b78e18e344d02dd123e
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380296"
---
# <a name="mediastream-resource-type"></a>Ressourcentyp mediaStream

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Der Typ des MediaStream.

## <a name="properties"></a>Eigenschaften

| Eigenschaft    | Typ    | Beschreibung                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| Richtung   | Zeichenfolge  | Die Richtung. Die möglichen Werte sind `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.                  |
| label       | String  | Die Bezeichnung des Media-Stream.                                                                                       |
| mediaType   | Zeichenfolge  | Geben Sie das Medium. Die mögliche Werte sind `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.        |
| serverMuted | Boolescher Wert | Wenn vom Server die Medien stummgeschaltet sind.                                                                          |
| sourceId    | Zeichenfolge  | Die Quell-ID.                                                                                                |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted"
  ],
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "inactive | sendOnly | receiveOnly | sendReceive",
  "label": "String",
  "mediaType": "unknown | audio | video | videoBasedScreenSharing | data",
  "serverMuted": true,
  "sourceId": "String"
}
```

## <a name="example"></a>Beispiel

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "sendReceive",
  "label": "main-audio",
  "mediaType": "audio",
  "serverMuted": false,
  "sourceId": "1024"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
