---
title: Ressourcentyp teamMessagingSettings
description: So konfigurieren Sie die messaging-Einstellungen und erwähnungen im Team.
author: nkramer
ms.openlocfilehash: 387c2e3ccedc6f11f17d4868b1b0d3eaf67624fa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304550"
---
# <a name="teammessagingsettings-resource-type"></a>Ressourcentyp teamMessagingSettings



So konfigurieren Sie die messaging-Einstellungen und erwähnungen im [Team](team.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowUserEditMessages|Boolesch|Wenn es sich bei Festlegung auf true können Benutzer ihre Nachrichten bearbeiten kann.|
|allowUserDeleteMessages|Boolesch|Bei Festlegung auf true können Benutzer ihre Nachrichten löschen kann.|
|allowOwnerDeleteMessages|Boolesch|Bei Festlegung auf "true" Websitebesitzer eine beliebige Nachricht löschen kann.|
|allowTeamMentions|Boolesch|Wenn Festlegung auf "true", "@team erwähnungen sind zulässig.|
|allowChannelMentions|Boolesch|Wenn Festlegung auf "true", "@channel erwähnungen sind zulässig.|

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
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
