---
title: Ressourcentyp mediaStream
description: Der Typ des MediaStream.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4867675da3427beb790beb240cd7bc0b86f04317
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519962"
---
# <a name="mediastream-resource-type"></a>Ressourcentyp mediaStream

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Der Typ des MediaStream.

## <a name="properties"></a>Eigenschaften

| Eigenschaft    | Typ    | Beschreibung                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| Richtung   | String  | Die Richtung. Die möglichen Werte sind `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.                  |
| label       | String  | Die Bezeichnung des Media-Stream.                                                                                       |
| MediaType   | String  | Geben Sie das Medium. Die mögliche Werte sind `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.        |
| serverMuted | Boolescher Wert | Wenn vom Server die Medien stummgeschaltet sind.                                                                          |
| SourceId    | String  | Die Quell-ID.                                                                                                |

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
<!--
{
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mediastream.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
