---
title: Ressourcentyp teamMessagingSettings
description: So konfigurieren Sie die messaging-Einstellungen und erwähnungen im Team.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 06aca84355a07052dcea316145dfff437eee743b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848258"
---
# <a name="teammessagingsettings-resource-type"></a>Ressourcentyp teamMessagingSettings

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

So konfigurieren Sie die messaging-Einstellungen und erwähnungen im [Team](team.md).

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowUserEditMessages|Boolean|Wenn es sich bei Festlegung auf true können Benutzer ihre Nachrichten bearbeiten kann.|
|allowUserDeleteMessages|Boolean|Bei Festlegung auf true können Benutzer ihre Nachrichten löschen kann.|
|allowOwnerDeleteMessages|Boolean|Bei Festlegung auf "true" Websitebesitzer eine beliebige Nachricht löschen kann.|
|allowTeamMentions|Boolean|Wenn Festlegung auf "true", "@team erwähnungen sind zulässig.|
|allowChannelMentions|Boolean|Wenn Festlegung auf "true", "@channel erwähnungen sind zulässig.|

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
