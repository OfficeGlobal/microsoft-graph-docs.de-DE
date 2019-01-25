---
title: Ressourcentyp organizerMeetingInfo
description: Besprechungsinformationen, die den Organisator der Besprechung enthält.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3b7d21a313d8744f18c8b96549bc9470b587361c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512241"
---
# <a name="organizermeetinginfo-resource-type"></a>Ressourcentyp organizerMeetingInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Besprechungsinformationen, die den Organisator der Besprechung enthält.

## <a name="properties"></a>Eigenschaften

| Eigenschaft                     | Typ                          | Beschreibung                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| allowConversationWithoutHost | Boolescher Wert                       | Gibt an, ob eine Unterhaltung fortgesetzt werden kann, sobald der Host der Unterhaltung verlässt. |
| organizer                    | [identitySet](identityset.md) | Der Organisator Azure Active Directory-Identität.  |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": { "@odata.type": "#microsoft.graph.identitySet" }
}
```

## <a name="example"></a>Beispiel

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": {
    "user": {
      "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
      "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/organizermeetinginfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
