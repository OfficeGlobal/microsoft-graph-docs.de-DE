---
title: Ressourcentyp audioConferencing
description: Stellt Access Telefoninformationen für einen OnlineMeeting.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb822f2049d84f9a2460370f05d5dfc85c347f15
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522175"
---
# <a name="audioconferencing-resource-type"></a>Ressourcentyp audioConferencing

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt Access Telefoninformationen für einen [OnlineMeeting](onlinemeeting.md).

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ    | Beschreibung                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| dialinUrl           | String  | Eine URL, die extern zugängliche Webseite, die Einwahlinformationen enthält. |
| leaderPasscode      | String  | Der Leiter Kennwort zum Verbinden mit dem Audio Conference Provider erforderlich.      |
| participantPasscode | String  | Die Teilnehmer das Kennwort zum Verbinden mit dem Audio Conference Provider erforderlich. |
| tollFreeNumber      | String  | Die gebührenfreie Telefonnummer für die Audio Conference Provider die Verbindung.              |
| tollNumber          | String  | Die gebührenpflichtige Telefonnummer für die Audio Conference Provider die Verbindung.                   |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "leaderPasscode": "String",
  "participantPasscode": "String",
  "tollFreeNumber": "String",
  "tollNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audioconferencing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
