---
title: Ressourcentyp chatMessageMention
description: 'Stellt einen Vermerk in einer ChatMessage Entität dar. Benutzer, Team, Bot oder DDE-Kanal kann die Erwähnung sein. '
localization_priority: Normal
ms.openlocfilehash: f37374a9793000ba641ed772e5dbfca5c0f1bd30
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515349"
---
# <a name="chatmessagemention-resource-type"></a>Ressourcentyp chatMessageMention

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt einen Vermerk in einer [ChatMessage](chatmessage.md) Entität dar. Benutzer, Team, Bot oder DDE-Kanal kann die Erwähnung sein. 

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|string|ID der Entität erwähnt wird|
|mentionText|string|Zeichenfolge, mit der Erwähnung Ex dargestellt: Anzeigename des Benutzers, Teamname usw.|
|erwähnten|[identitySet](identityset.md)|Der Benutzer, der erwähnt wurde|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "string (identifier)",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatMention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
