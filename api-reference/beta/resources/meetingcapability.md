---
title: Ressourcentyp meetingCapability
description: Enthält die Funktionen einer Besprechung
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e71d7c8c6489d5856e5f2441cd93c7fdea033bd4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524289"
---
# <a name="meetingcapability-resource-type"></a>Ressourcentyp meetingCapability

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Enthält die Funktionen einer Besprechung

## <a name="properties"></a>Eigenschaften

| Eigenschaft                          | Typ    | Beschreibung                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| allowAnonymousUsersToDialOut      | Boolescher Wert | Gibt an, ob anonyme Benutzer als Client-Anschluss in einer Besprechung zulässig ist. |
| allowAnonymousUsersToStartMeeting | Boolescher Wert | Gibt an, ob anonyme Benutzer zugelassen sind, um eine Besprechung zu starten.  |
| autoAdmittedUsers                 | String  | Mögliche Werte: `everyoneInCompany`, `everyone`.              |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
  "allowAnonymousUsersToStartMeeting": true,
  "autoAdmittedUsers": "everyoneInCompany | everyone"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingcapability.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
