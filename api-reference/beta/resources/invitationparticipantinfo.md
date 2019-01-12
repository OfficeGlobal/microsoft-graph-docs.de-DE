---
title: Ressourcentyp invitationParticipantInfo
description: Die **InvitationParticipant** wird verwendet, um die Darstellung eines Satzes von Identitäten zugeordnet einer unterhaltungseinladung zu einer und bietet zusätzliche Einladung-Parameter.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8febd66915ee0b4fba26d9253cd56d67086e63bc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982897"
---
# <a name="invitationparticipantinfo-resource-type"></a>Ressourcentyp invitationParticipantInfo

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **InvitationParticipant** wird verwendet, um die Darstellung eines Satzes von Identitäten zugeordnet einer unterhaltungseinladung zu einer und bietet zusätzliche Einladung-Parameter.

## <a name="properties"></a>Eigenschaften

| Eigenschaft                           | Typ                          | Beschreibung                                                                          |
| :--------------------------------- | :---------------------------- | :----------------------------------------------------------------------------------- |
| endpointType                       | String                        | Mögliche Werte: `default`, `voicemail`. |
| identity                           | [identitySet](identityset.md) | Die [IdentitySet](identityset.md) Einladung zugeordnet.                   |
| languageId                         | Zeichenfolge                        | Die Sprache-Kultur-Zeichenfolge.                                                                                     |
| Region                             | Zeichenfolge                        | Region des Teilnehmers.                                                           |
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
<!-- {
  "type": "#page.annotation",
  "description": "invitationParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
