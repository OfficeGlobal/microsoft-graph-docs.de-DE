---
title: Ressourcentyp teamMessagingSettings
description: So konfigurieren Sie die messaging-Einstellungen und erwähnungen im Team.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d98dfa3c2306cabb99b6de96aed2010cefa10717
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510099"
---
# <a name="teammessagingsettings-resource-type"></a>Ressourcentyp teamMessagingSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

So konfigurieren Sie die messaging-Einstellungen und erwähnungen im [Team](team.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowUserEditMessages|Boolescher Wert|Wenn es sich bei Festlegung auf true können Benutzer ihre Nachrichten bearbeiten kann.|
|allowUserDeleteMessages|Boolescher Wert|Bei Festlegung auf true können Benutzer ihre Nachrichten löschen kann.|
|allowOwnerDeleteMessages|Boolescher Wert|Bei Festlegung auf "true" Websitebesitzer eine beliebige Nachricht löschen kann.|
|allowTeamMentions|Boolescher Wert|Wenn Festlegung auf "true", "@team erwähnungen sind zulässig.|
|allowChannelMentions|Boolescher Wert|Wenn Festlegung auf "true", "@channel erwähnungen sind zulässig.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teammessagingsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
