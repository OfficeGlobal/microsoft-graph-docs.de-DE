---
title: Ressourcentyp meetingParticipantInfo
description: Informationen über einen Teilnehmer an einer Besprechung.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1ba727344b1f653125a482b592e7d28c11d1d3d5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515027"
---
# <a name="meetingparticipantinfo-resource-type"></a>Ressourcentyp meetingParticipantInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Informationen über einen Teilnehmer an einer Besprechung.

## <a name="properties"></a>Eigenschaften

| Eigenschaft       | Typ                          | Beschreibung                              |
|:---------------|:------------------------------|:-----------------------------------------|
| [-Identity]       | [identitySet](identityset.md) | Identitätsinformationen des Teilnehmers. |
| UPN            | String                        | Benutzerprinzipalname des Teilnehmers.  |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingparticipantinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
