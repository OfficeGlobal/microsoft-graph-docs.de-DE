---
title: Ressourcentyp teamMessagingSettings
description: So konfigurieren Sie die messaging-Einstellungen und erwähnungen im Team.
ms.openlocfilehash: 51a0fb53079e8fd79f469f022efb2f293e9a6cba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060204"
---
# <a name="teammessagingsettings-resource-type"></a>Ressourcentyp teamMessagingSettings

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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
