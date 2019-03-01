---
title: eventMessageRequest-Ressourcentyp
description: Eine Nachricht, die eine Besprechungsanfrage darstellt.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1928273ef45b277fa81dba5a4db7b908134491d3
ms.sourcegitcommit: e8b488f8068845522b869bf97475da7b078bee3d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/01/2019
ms.locfileid: "30342303"
---
# <a name="eventmessagerequest-resource-type"></a>eventMessageRequest-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine Nachricht, die eine Besprechungsanfrage darstellt.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "event",
    "extensions",
    "previousLocation",
    "previousStartDateTime",
    "previousEndDateTime"
  ],
  "@odata.type": "microsoft.graph.eventMessageRequest"
}-->

```json
{
  "bccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "changeKey": "string",
  "conversationId": "string",
  "createdDateTime": "String (timestamp)",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isOutOfDate": "Boolean",
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "meetingMessageType": "microsoft.graph.meetingMessageType",
  "parentFolderId": "string",
  "previousEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "previousLocation": {"@odata.type": "microsoft.graph.location"},
  "previousStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "receivedDateTime": "String (timestamp)",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "type": "string",
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|bccRecipients|[recipient](recipient.md) collection|Die Bcc:-Empfänger der Nachricht.|
|body|[itemBody](itembody.md)|Der Text der Nachricht.|
|bodyPreview|String|Die ersten 255 Zeichen des Nachrichtentexts.|
|categories|String collection|Die Kategorien, die mit der Nachricht verknüpft sind.|
|ccRecipients|[recipient](recipient.md)-Sammlung|Die Cc:-Empfänger der Nachricht.|
|changeKey|Zeichenfolge|Die Version der Nachricht.|
|conversationId|Zeichenfolge|Die ID der Unterhaltung, zu der die E-Mail gehört.|
|createdDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht erstellt wurde.|
|endDateTime|[DateTimeTimeZone](datetimetimezone.md)|Die Endzeit der angeforderten Besprechung.|
|Von|[Empfänger](recipient.md)|Der Postfachbesitzer und der Absender der Nachricht.|
|hasAttachments|Boolescher Wert|Gibt an, ob die Nachricht Anlagen enthält.|
|ID|Zeichenfolge|Schreibgeschützt.|
|importance|Zeichenfolge| Wichtigkeit der Nachricht: `Low`, `Normal`, `High`.|
|inferenceClassification|Zeichenfolge| Mögliche Werte: `Focused`, `Other`.|
|isDeliveryReceiptRequested|Boolean|Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.|
|isDraft|Boolean|Gibt an, ob die Nachricht ein Entwurf ist. Eine Nachricht ist ein Entwurf, solange sie noch nicht gesendet wurde.|
|isOutOfDate|Boolean|Gibt an, ob diese Besprechungsanfrage aufgrund einer neueren Anforderung veraltet ist.|
|isRead|Boolean|Gibt an, ob die Nachricht gelesen wurde.|
|isReadReceiptRequested|Boolean|Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.|
|lastModifiedDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht zuletzt geändert wurde.|
|location|[Ort](location.md)|Der Ort der angeforderten Besprechung.|
|meetingMessageType|String| Der Typ der Ereignisnachricht: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTentativelyAccepted`, `meetingDeclined`.|
|parentFolderId|Zeichenfolge|Der eindeutige Bezeichner für das übergeordnete mailFolder-Element der Nachricht.|
|previousEndDateTime|[DateTimeTimeZone](datetimetimezone.md)|Die vorherige Endzeit der angeforderten Besprechung.|
|Previouslocation –|[Ort](location.md)|Der vorherige Speicherort der angeforderten Besprechung.|
|previousStartDateTime|[DateTimeTimeZone](datetimetimezone.md)|Die vorherige Startzeit der angeforderten Besprechung.|
|receivedDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht erhalten wurde.|
|recurrence|[PatternedRecurrence](patternedrecurrence.md)|Das Serienmuster der angeforderten Besprechung.|
|replyTo|[recipient](recipient.md) collection|Die E-Mail-Adressen, die beim Antworten verwendet werden sollen.|
|sender|[Empfänger](recipient.md)|Das Konto, das tatsächlich verwendet wird, um die Nachricht zu generieren.|
|sentDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht gesendet wurde.|
|startDateTime|[DateTimeTimeZone](datetimetimezone.md)|Die Startzeit der angeforderten Besprechung.|
|Betreff|String|Der Betreff der Nachricht.|
|toRecipients|[recipient](recipient.md) collection|Die An:-Empfänger der Nachricht.|
|type|Zeichenfolge|Der Typ der angeforderten `singleInstance`Besprechung `occurence`: `exception`, `seriesMaster`,,.|
|uniqueBody|[itemBody](itembody.md)|Der Teil des Textkörpers der Nachricht, der für die aktuelle Nachricht eindeutig ist.|
|webLink|Zeichenfolge|Die URL zum Öffnen der Nachricht in Outlook Web App.<br><br>Sie können am Ende der URL das Argument „ispopout“ anhängen, um zu ändern, wie die Nachricht angezeigt wird. Wenn „ispopout“ nicht vorhanden oder auf 1 festgelegt ist, wird die Nachricht in einem Popout-Fenster angezeigt. Wenn „ispopout“ auf 0 festgelegt ist, zeigt der Browser die Nachricht in Outlook Web App im Prüffensterbereich an.<br><br>Die Nachricht wird im Browser geöffnet, wenn Sie über Outlook Web App bei Ihrem Postfach angemeldet sind. Sie werden aufgefordert, sich anzumelden, wenn Sie noch nicht beim Browser angemeldet sind.<br><br>Auf diese URL kann von einem iFrame aus zugegriffen werden.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Anlagen|[Anlagensammlung](attachment.md)| Schreibgeschützt. Lässt Nullwerte zu.|
|Ereignis|[Ereignis](event.md)| Das Ereignis, das der Ereignisnachricht zugeordnet ist. Für Teilnehmer oder Raumressourcen wird davon ausgegangen, dass die Kalenderautomatik für die automatische Aktualisierung des Kalenders mit einem Ereignis festgelegt ist, wenn Ereignisnachrichten mit Besprechungsanfragen eingehen Navigationseigenschaft.  Schreibgeschützt.|
|Erweiterungen|[Erweiterungssammlung](extension.md)| Schreibgeschützt. Nullwerte zulassend.|

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[eventMessage abrufen](../api/eventmessage-get.md) | [eventMessage](eventmessage.md) |Liest die Eigenschaften und Beziehungen eines eventMessage-Objekts.|
|[Anlage erstellen](../api/eventmessage-post-attachments.md) |[Anlage](attachment.md)| Erstellt eine neue Anlage durch Veröffentlichen in der Anlagensammlung.|
|[Anlagen auflisten](../api/eventmessage-list-attachments.md) |[attachment](attachment.md)-Sammlung| Ruft eine Sammlung von Anlagenobjekten ab.|
|[Aktualisieren](../api/eventmessage-update.md) | [eventMessage](eventmessage.md)  |Aktualisiert das eventMessage-Objekt. |
|[Löschen](../api/eventmessage-delete.md) | Keine |Löscht das eventMessage-Objekt. |
|[Kopieren](../api/message-copy.md)|[Nachricht](message.md)||
|[createForward](../api/message-createforward.md)|[Nachricht](message.md)||
|[createReply](../api/message-createreply.md)|[Nachricht](message.md)||
|[createReplyAll](../api/message-createreplyall.md)|[Nachricht](message.md)||
|[forward](../api/message-forward.md)|Keine|Weiterleiten einer Nachricht. Die Nachricht wird dann im Ordner "Gesendete Elemente" gespeichert.|
|[move](../api/message-move.md)|[Nachricht](message.md)|Verschieben Sie die Nachricht in einen e-Mail-Ordner.|
|[Antworten](../api/message-reply.md)|Keine|Antwortet dem Absender einer Nachricht. Die Nachricht wird dann im Ordner "Gesendete Elemente" gespeichert.|
|[replyAll](../api/message-replyall.md)|Keine|Sendet eine Antwort an alle Empfänger einer E-Mail. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|
|[Senden](../api/message-send.md)|Keine|Sendet einen zuvor erstellten Nachrichtenentwurf. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "eventMessageRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/eventmessagerequest.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
