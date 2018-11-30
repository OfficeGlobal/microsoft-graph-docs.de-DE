---
title: Ressourcentyp mediaStream
description: Der Typ des MediaStream.
ms.openlocfilehash: 28eb98a3ab1be67c60c6ebd35deb7618f1618be3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065724"
---
# <a name="mediastream-resource-type"></a>Ressourcentyp mediaStream

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Der Typ des MediaStream.

## <a name="properties"></a>Eigenschaften

| Eigenschaft    | Typ    | Beschreibung                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| Richtung   | String  | Die Richtung. Die möglichen Werte sind `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.                  |
| label       | String  | Die Bezeichnung des Media-Stream.                                                                                       |
| mediaType   | String  | Geben Sie das Medium. Die mögliche Werte sind `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.        |
| serverMuted | Boolesch | Wenn vom Server die Medien stummgeschaltet sind.                                                                          |
| sourceId    | String  | Die Quell-ID.                                                                                                |

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
