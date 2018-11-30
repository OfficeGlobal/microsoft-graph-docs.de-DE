---
title: Ressourcentyp chatMessage
description: Stellt eine einzelne Chatnachricht innerhalb einer Entität Kanal oder Chat. Die Nachricht kann ein Stamm-Nachricht oder einen Teil davon ein Thread, der von der **ReplyToId** -Eigenschaft in der Nachricht definiert ist.
ms.openlocfilehash: 1fba27567d5a1c80a36a5758925ec427735504cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058270"
---
# <a name="chatmessage-resource-type"></a>Ressourcentyp chatMessage

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine einzelne Chatnachricht innerhalb einer Entität [Kanal](channel.md) oder Chat. Die Nachricht kann ein Stamm-Nachricht oder einen Teil davon ein Thread, der von der **ReplyToId** -Eigenschaft in der Nachricht definiert ist.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Liste Channel Nachrichten](../api/channel-list-messages.md) | [Chatmessage](chatmessage.md) -Auflistung | Rufen Sie die Liste aller Stamm-Nachrichten in einem Kanal.|
|[Get-Channel-Nachricht](../api/channel-get-message.md) | [chatmessage](chatmessage.md) | Rufen Sie eine Nachricht einzelnen Stamm aus einem Kanal.|
|[Liste Antworten auf eine Nachricht](../api/channel-list-messagereplies.md) | [Chatmessage](chatmessage.md) -Auflistung| Abrufen der Liste mit allen Antworten auf eine Nachricht im Kanal.|
|[Erhalten Sie eine Antwort auf eine Nachricht](../api/channel-get-messagereply.md) | [chatmessage](chatmessage.md)| Abrufen einer einzigen Antwort auf eine Nachricht in einem Kanal.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Schreibgeschützt. Eindeutige ID der Nachricht.|
|replyToId| string | ID der übergeordneten Nachricht/Root Nachricht des Threads |
|Von|[identitySet](identityset.md)| Details des Absenders der Nachricht|
|etag| string | Versionsnummer der Nachricht |
|messageType|String|Der Typ der aktuellen Nachricht unterstützt Werte sind: Meldung, ChatEvent, Eingabe|
|createdDateTime|dateTimeOffset|Schreibgeschützt. Zeitstempel der Erstellung der Nachricht|
|lastModifiedDateTime|dateTimeOffset|Schreibgeschützt. Wenn die Nachricht bearbeitet/aktualisiert wurde Zeitstempel|
|isDeleted|Boolean|Darstellt, wenn eine Nachricht weiche gelöscht wurde|
|deletedDateTime|dateTimeOffset|Schreibgeschützt. Zeitstempel, an dem die Nachricht gelöscht wurde |
|subject|string|Betreffzeile der Nachricht. Optional|
|body|[itemBody](itembody.md)|Nur-Text/HTML-Darstellung des Inhalts der Nachricht. Gibt nur-Text in der Standardeinstellung kann Anwendung HTML als Teil einer Abfrage Param auswählen|
|Zusammenfassung|string|Zusammengefassten Texts der Nachricht, die für Pushbenachrichtigungen und Übersichten oder fallen Back Ansichten verwendet werden können|
|Erwähnungen|[ChatMessageMention](chatmention.md) -Auflistung| Liste der Entitäten, die in der Meldung genannten. Derzeit unterstützt Benutzer, Bot, Team, DDE-Kanal|
|Wichtigkeit| string | Die Wichtigkeit der Nachricht: Normal, hoch|
|Reaktionen| [ChatMessageReaction](chatreaction.md) -Auflistung | Reaktionen für diese Nachricht (beispielsweise wie)|
|Gebietsschema|string|Gebietsschema der Nachricht vom Client festgelegt|
|attachments|[ChatMessageAttachment](chatattachment.md) -Auflistung |Dateianlagen|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isDeleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "reactions",
    "mentions",
    "subject",
    "summary"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessage"
}-->

```json
{
  "id": "string (identifier)",
  "replyToId": "string (identifier)",
  "from": {"@odata.type": "microsoft.graph.identitySet"},
  "etag": "string",
  "messageType": "string",
  "createdDateTime": "string (timestamp)",
  "lastModifiedDateTime": "string (timestamp)",
  "isDeleted": "boolean",
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
