---
title: Ressourcentyp chatMessageReaction
description: 'Stellt eine Reaktion auf eine Entität ChatMessage dar. '
ms.openlocfilehash: 1ad1f7948405a8891ec9aa13065b71108e9c47c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065851"
---
# <a name="chatmessagereaction-resource-type"></a>Ressourcentyp chatMessageReaction

Stellt eine Reaktion auf eine Entität [ChatMessage](chatmessage.md) dar. 

Eine Entität vom Typ `chatMessageReaction` wird als Teil des [ChatMessage](chatmessage.md) -Entität als Teil des [Kanalnachrichten abrufen](../api/channel-get-message.md) -API zurückgegeben.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|reactionType|string| Der Typ der Reaktion. Geplante Werte: <br><ul><li>Wie - wie eine Nachricht Inhalte leer in diesem Fall ist.</li><li>Emoji - Emoji Reaktion. Inhalt wird auf Unicodewert, der die Emoji festgelegt.</li><li>Label - wird Inhalt auf die Zeichenfolge die Bezeichnung festgelegt.</li></ul>|
|createdDateTime|dateTimeOffset|UTC-Zeitstempel der Stamm Nachricht im ISO 8601-Format.|
|user|identitySet|Der Benutzer, die an die Nachricht reagiert.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "content"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageReaction"
}-->

```json
{
  "reactionType": "string ",
  "createdDateTime": "string (timestamp)",
  "user": {"@odata.type": "microsoft.graph.identitySet"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message reaction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
