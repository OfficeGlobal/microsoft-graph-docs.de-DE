---
title: Ressourcentyp invitationParticipantInfo
description: Die **InvitationParticipant** wird verwendet, um die Darstellung eines Satzes von Identitäten zugeordnet einer unterhaltungseinladung zu einer und bietet zusätzliche Einladung-Parameter.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb20dde1a74472695755e65dc404a6709f79c8b0
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641918"
---
# <a name="invitationparticipantinfo-resource-type"></a>Ressourcentyp invitationParticipantInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Die **InvitationParticipant** wird verwendet, um die Darstellung eines Satzes von Identitäten zugeordnet einer unterhaltungseinladung zu einer und bietet zusätzliche Einladung-Parameter.

## <a name="properties"></a>Eigenschaften

| Eigenschaft                           | Typ                          | Beschreibung                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| endpointType                       | String                        | Mögliche Werte: `default`, `voicemail`. |
| identity                           | [identitySet](identityset.md) | Die [IdentitySet](identityset.md) Einladung zugeordnet.                   |
| languageId                         | String                        | Die Sprache-Kultur-Zeichenfolge.                                                                                     |
| Region                             | String                        | Region des Teilnehmers.                                                           |
| replacesCallId                     | Zeichenfolge                        | Optional. Der Aufruf der das Ziel Idenity derzeit gehört. Sobald der Teilnehmer hinzugefügt wird, wird dieses Anrufs gelöscht werden. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}-->
```json
{
  "endpointType": "default | voicemail",
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "languageId": "String",
  "region": "String",
  "replacesCallId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/invitationparticipantinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
