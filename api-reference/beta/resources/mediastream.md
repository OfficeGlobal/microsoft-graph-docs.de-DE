---
title: Ressourcentyp mediaStream
description: Der Typ des MediaStream.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fd003bde0eca5fd21cb12c23d5c83699a6b79c8e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916964"
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
