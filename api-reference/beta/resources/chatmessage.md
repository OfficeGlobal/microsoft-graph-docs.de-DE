---
title: chatMessage-Ressourcentyp
description: Stellt eine einzelne Chatnachricht innerhalb eines Kanals oder einer Chatentität dar. Die Nachricht kann eine Stammnachricht oder Teil eines Threads sein, die bzw. der von der **replyToId**-Eigenschaft in der Nachricht definiert wird.
localization_priority: Priority
ms.openlocfilehash: a74f422c6bf60e1293d8620b440152be77dacdc7
ms.sourcegitcommit: cd4bdb2c6754b1d5658e68909ea6c219466da6df
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30644321"
---
# <a name="chatmessage-resource-type"></a>chatMessage-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt eine einzelne Chatnachricht innerhalb eines [Kanals](channel.md) oder einer Chatentität dar. Die Nachricht kann eine Stammnachricht oder Teil eines Threads sein, die bzw. der von der **replyToId**-Eigenschaft in der Nachricht definiert wird.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Kanalnachrichten auflisten](../api/channel-list-messages.md) | [chatMessage](chatmessage.md)-Sammlung | Abrufen der Liste aller Stammnachrichten in einem Kanal.|
|[Kanalnachricht abrufen](../api/channel-get-message.md) | [chatmessage](chatmessage.md) | Abrufen einer einzelnen Stammnachricht aus einem Kanal.|
|[Antworten in einer Nachricht auflisten](../api/channel-list-messagereplies.md) | [chatMessage](chatmessage.md)-Sammlung| Abrufen der Liste aller Antworten auf eine Nachricht im Kanal.|
|[Antwort auf eine Nachricht abrufen](../api/channel-get-messagereply.md) | [chatmessage](chatmessage.md)| Abrufen einer einzelnen Antwort auf eine Nachricht in einem Kanal.|
|[Senden einer Nachricht in einem Kanal](../api/channel-post-chatmessage.md) | [chatmessage](chatmessage.md)| Erstellen Sie eine neue Nachricht auf oberster Ebene in einem Kanal.|
|[Antworten auf eine Nachricht in einem Kanal](../api/channel-post-messagereply.md) | [chatmessage](chatmessage.md)| Antworten Sie auf eine Nachricht in einem Kanal.|


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Schreibgeschützt. Eindeutige ID der Nachricht.|
|replyToId| string | ID der übergeordneten Nachricht/Stammnachricht des Threads. |
|von|[identitySet](identityset.md)| Schreibgeschützt. Einzelheiten über den Absender der Nachricht.|
|etag| string | Versionsnummer der Nachricht. |
|messageType|Zeichenfolge|Der Typ der Nachricht; aktuell unterstützte Werte sind: message, chatEvent, Typing.|
|createdDateTime|dateTimeOffset|Schreibgeschützt. Zeitstempel, wann die Nachricht erstellt wurde.|
|lastModifiedDateTime|dateTimeOffset|Schreibgeschützt. Zeitstempel, wann die Nachricht bearbeitet/aktualisiert wurde.|
|deleted|Boolesch|Gibt an, ob eine Nachricht vorläufig gelöscht wurde.|
|deletedDateTime|dateTimeOffset|Schreibgeschützt. Zeitstempel, wann die Nachricht gelöscht wurde. |
|subject|Zeichenfolge|Nachrichtenbetreff Optional.|
|Text|[itemBody](itembody.md)|Nur-Text-/HTML-Darstellung des Inhalts der Nachricht. Gibt standardmäßig Nur-Text wieder; Anwendung kann HTML wahlweise als Teil eines Abfrageparameters auswählen|
|Zusammenfassung|Zeichenfolge|Zusammenfassungstext der Nachricht, die für Pushbenachrichtigungen und Zusammenfassungs- oder Fallbackansichten verwendet werden kann |
|Erwähnungen|[chatMessageMention](chatmention.md)-Sammlung| Liste der Entitäten, die in der Nachricht angegeben werden. Derzeit unterstützt: user, bot, team, channel.|
|Wichtigkeit| string | Legt die Wichtigkeit der Nachricht fest: Hoch, Niedrig.|
|Reaktionen| [chatMessageReaction](chatreaction.md)-Sammlung | Reaktionen auf diese Nachricht (z. B. Gefällt mir)|
|Gebietsschema|Zeichenfolge|Vom Client festgelegtes Gebietsschema der Nachricht|
|Anlagen|[chatMessageAttachment](chatattachment.md)-Sammlung |Angefügte Dateien. Anlagen sind derzeit schreibgeschützt – das Senden von Anlagen wird nicht unterstützt. |


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deleted",
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
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
