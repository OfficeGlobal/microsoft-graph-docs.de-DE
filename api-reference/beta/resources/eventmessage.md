---
title: eventMessage-Ressourcentyp
description: 'Eine Nachricht, die für eine Besprechungsanfrage, -absage oder -antwort steht (diese kann folgende umfassen: Zusage, Zusage mit Vorbehalt oder Absage). '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 926a9adc1a66ca912aff9a5ccea8db189eb4dae1
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643419"
---
# <a name="eventmessage-resource-type"></a>eventMessage-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Eine Nachricht, die für eine Besprechungsanfrage, -absage oder -antwort steht (diese kann folgende umfassen: Zusage, Zusage mit Vorbehalt oder Absage). 

Die Entität **EventMessage** [Nachricht](message.md)abgeleitet ist, und [EventMessageRequest](eventmessagerequest.md) **EventMessage** abgeleitet ist und eine Besprechungsanfrage darstellt. Die **meetingMessageType**-Eigenschaft gibt den Typ der Ereignisnachricht an.

Wenn ein Organisator oder eine App eine Besprechungsanfrage sendet, trifft die Besprechungsanfrage als eine **eventMessage**-Instanz mit **meetingMessageType** von **meetingRequest** in dem Postfach des Teilnehmers ein. Darüber hinaus erstellt Outlook automatisch eine **event**-Instanz im Kalender des Teilnehmers mit der **showAs**-Eigenschaft als **tentative**. 

Um die Eigenschaften des zugeordneten Ereignisses im Postfach des Teilnehmers abzurufen, kann die App die **event**-Navigationseigenschaft von **eventMessage** verwenden, wie in diesem [Beispiel zum Abrufen von Ereignisnachrichten](../api/eventmessage-get.md#request-2) dargestellt. Die app kann auch auf das Ereignis im Namen der Teilnehmer programmgesteuert [akzeptieren](../api/event-accept.md), [mit Vorbehalt annehmen](../api/event-tentativelyaccept.md)oder [Ablehnen](../api/event-decline.md) des Ereignisses reagieren.

Neben dem, einer Besprechungsanfrage kann eine **EventMessage** Instanz eines Teilnehmers Remoteelement in dem Ordner als Ergebnis der Organisator des Ereignisses Abbrechen einer Besprechung oder in der Organisator Posteingang aufgrund eines Teilnehmers reagiert auf die Besprechungsanfrage gefunden werden. Eine App kann mit kleineren Abweichungen Aktionen sowohl bei Ereignisnachrichten als auch bei Nachrichten ausführen.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.  

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "event",
    "extensions",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.eventMessage"
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
  "conversationIndex": "binary",
  "createdDateTime": "DateTimeOffset",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageHeaders": [{"@odata.type": "microsoft.graph.internetMessageHeader"}],
  "internetMessageId": "String",
  "isAllDay": "Boolean",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isOutOfDate": "Boolean",
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "DateTimeOffset",
  "location": {"@odata.type": "microsoft.graph.location"},
  "meetingMessageType": {"@odata.type": "microsoft.graph.meetingMessageType"},
  "parentFolderId": "string",
  "receivedDateTime": "DateTimeOffset",
  "recurrence": {"@odata.type": "microsoft.graph.patternedrecurrence"},
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "DateTimeOffset",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "type": "string",
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "UnsubscribeData": "string",
  "UnsubscribeEnabled": true,
  "webLink": "string"
}

```

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|bccRecipients|[recipient](recipient.md) collection|Die Bcc:-Empfänger der Nachricht.|
|body|[itemBody](itembody.md)|Der Text der Nachricht. Er kann im HTML- oder Textformat vorliegen.|
|bodyPreview|String|Die ersten 255 Zeichen des Nachrichtentexts. Liegt im Textformat vor. |
|categories|String collection|Die Kategorien, die mit der Nachricht verknüpft sind.|
|ccRecipients|[recipient](recipient.md) collection|Die Cc:-Empfänger der Nachricht.|
|changeKey|String|Die Version der Nachricht.|
|conversationId|String|Die ID der Unterhaltung, zu der die E-Mail gehört.|
|conversationIndex|Binär|Der Index der Unterhaltung, zu der die E-Mail gehört.|
|createdDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht erstellt wurde.|
|endDateTime|[dateTimeTimeZone](datetimetimezone.md)|Die Endzeit der angeforderten Besprechung.|
|Flag|[followUpFlag](followupflag.md)|Der Wert des Flags, der den Status, das Startdatum, das Fälligkeitsdatum oder das Enddatum für die Nachricht angibt.|
|Von|[Empfänger](recipient.md)|Der Postfachbesitzer und der Absender der Nachricht.|
|hasAttachments|Boolean|Gibt an, ob die Nachricht Anlagen enthält.|
|ID|String||
|Wichtigkeit|String| Wichtigkeit der Nachricht: `low`, `normal`, `high`.|
|inferenceClassification|String| Mögliche Werte: `focused`, `other`.|
|internetMessageHeaders | [internetinternetMessageHeaders](internetmessageheader.md)-Sammlung | Die Sammlung von Nachrichtenkopfzeilen, definiert von [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), die Informationen des von einer Nachricht vom Absender bis zum Empfänger verwendeten Pfads einer Nachricht liefert. Schreibgeschützt.|
|internetMessageId |Zeichenfolge |Die Nachrichten-ID im von [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) angegebenen Format. |
|isAllDay |Boolean|Gibt an, ob das Ereignis den ganzen Tag dauert. Anpassen dieser Eigenschaft erfordert die **StartDateTime** und **EndDateTime** Eigenschaften des Ereignisses sowie anpassen.|
|isDeliveryReceiptRequested|Boolean|Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.|
|isDraft|Boolean|Gibt an, ob die Nachricht ein Entwurf ist. Eine Nachricht ist ein Entwurf, solange sie noch nicht gesendet wurde.|
|isOutOfDate|Boolean|Gibt an, ob diese Besprechungsanfrage von einer neueren Anforderung veralteten vorgenommen wurden.|
|isRead|Boolean|Gibt an, ob die Nachricht gelesen wurde.|
|isReadReceiptRequested|Boolean|Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.|
|lastModifiedDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht zuletzt geändert wurde.|
|location|[location](location.md)|Der Speicherort der angeforderten Besprechung.|
|meetingMessageType|String| Der Typ der Ereignisnachricht: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTenativelyAccepted`, `meetingDeclined`.|
|parentFolderId|String|Der eindeutige Bezeichner für das übergeordnete mailFolder-Element der Nachricht.|
|receivedDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht erhalten wurde.|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|Das Serienmuster der angeforderten Besprechung.|
|replyTo|[recipient](recipient.md) collection|Die E-Mail-Adressen, die beim Antworten verwendet werden sollen.|
|sender|[Empfänger](recipient.md)|Das Konto, das tatsächlich verwendet wird, um die Nachricht zu generieren.|
|sentDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht gesendet wurde.|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|Die Anfangszeit der angeforderten Besprechung.|
|subject|String|Der Betreff der Nachricht.|
|toRecipients|[recipient](recipient.md) collection|Die An:-Empfänger der Nachricht.|
|type|String|Die Art der angeforderten Besprechung: `singleInstance`, `occurence`, `exception`, `seriesMaster`.|
|uniqueBody|[itemBody](itembody.md)|Der Teil des Textkörpers der Nachricht, der für die aktuelle Nachricht eindeutig ist.|
|UnsubscribeData|String|Die gültigen Einträge, die vom List-Unsubscribe-Header analysiert werden.  Dies sind die Daten für den E-Mail-Befehl im List-Unsubscribe-Header, wenn die UnsubscribeeEnabled-Eigenschaft „true“ ist.|
|UnsubscribeEnabled|Boolesch|Gibt an, ob die Nachricht zum Kündigen des Abonnements aktiviert ist.  Wenn der list-Unsubscribe-Header „rfc-2369“ entspricht, ist der Wert „true“.|
|webLink|String|Die URL zum Öffnen der Nachricht in Outlook Web App.<br><br>Sie können am Ende der URL das Argument „ispopout“ anhängen, um zu ändern, wie die Nachricht angezeigt wird. Wenn „ispopout“ nicht vorhanden oder auf 1 festgelegt ist, wird die Nachricht in einem Popout-Fenster angezeigt. Wenn „ispopout“ auf 0 festgelegt ist, zeigt der Browser die Nachricht in Outlook Web App im Prüffensterbereich an.<br><br>Die Nachricht wird im Browser geöffnet, wenn Sie über Outlook Web App bei Ihrem Postfach angemeldet sind. Sie werden aufgefordert, sich anzumelden, wenn Sie noch nicht beim Browser angemeldet sind.<br><br>Auf diese URL kann von einem iFrame aus zugegriffen werden.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|attachments|[attachment](attachment.md)-Sammlung|Die Auflistung von [FileAttachment](fileattachment.md), [ItemAttachment](itemattachment.md)und [ReferenceAttachment](referenceattachment.md) Anlagen für die Nachricht. Schreibgeschützt. Lässt Nullwerte zu.|
|event|[event](event.md)| Das Ereignis, das der Ereignisnachricht zugeordnet ist. Für Teilnehmer oder Raumressourcen wird davon ausgegangen, dass die Kalenderautomatik für die automatische Aktualisierung des Kalenders mit einem Ereignis festgelegt ist, wenn Ereignisnachrichten mit Besprechungsanfragen eingehen Navigationseigenschaft.  Schreibgeschützt.|
|Erweiterungen|[extension](extension.md)-Sammlung| Die Sammlung der für das Ereignis definierten offenen Erweiterungen. Schreibgeschützt. Lässt NULL-Werte zu.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung| Die Sammlung der für die eventMessage definierten mehrwertigen erweiterten Eigenschaften. Schreibgeschützt. Lässt Nullwerte zu.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung| Die Sammlung der für die eventMessage definierten einwertigen erweiterten Eigenschaften. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[eventMessage abrufen](../api/eventmessage-get.md) | [eventMessage](eventmessage.md) |Liest die Eigenschaften und Beziehungen eines eventMessage-Objekts.|
|[Aktualisieren](../api/eventmessage-update.md) | [eventMessage](eventmessage.md)  |Aktualisiert das eventMessage-Objekt.|
|[Löschen](../api/eventmessage-delete.md) | Keiner |Löscht das eventMessage-Objekt.|
|[copy](../api/message-copy.md)|[message](message.md)|Mit dieser API können Sie Nachrichten in Ordner kopieren.|
|[createForward](../api/message-createforward.md)|[message](message.md)|Erstellt einen Entwurf der Weiterleitungsnachricht. Sie können den Entwurf dann [aktualisieren](../api/message-update.md) oder [senden](../api/message-send.md).|
|[createReply](../api/message-createreply.md)|[message](message.md)|Erstellt einen Entwurf der Antwortnachricht. Sie können den Entwurf dann [aktualisieren](../api/message-update.md) oder [senden](../api/message-send.md).|
|[createReplyAll](../api/message-createreplyall.md)|[message](message.md)|Erstellt einen Entwurf der „Allen Antworten“-Nachricht. Sie können den Entwurf dann [aktualisieren](../api/message-update.md) oder [senden](../api/message-send.md).|
|[Weiterleiten](../api/message-forward.md)|Keine|Leitet eine Nachricht weiter. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|
|[move](../api/message-move.md)|[message](message.md)|Verschiebt eine Nachricht in einen Ordner. Dadurch wird eine neue Kopie der Nachricht im Zielordner erstellt.|
|[Antworten](../api/message-reply.md)|Keine|Antwortet auf eine Nachricht des Absenders. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|
|[replyAll](../api/message-replyall.md)|Keine|Sendet eine Antwort an alle Empfänger einer E-Mail. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|
|[Senden](../api/message-send.md)|Keine|Sendet einen zuvor erstellten Nachrichtenentwurf. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|
|[unsubscribe](../api/message-unsubscribe.md)|Keine|Sendet eine Nachricht unter Verwendung der Daten und der Adresse, die im ersten mailto-Befehl im List-Unsubscribe-Header angegeben wurden.|
|**Anlagen**| | |
|[Anlagen auflisten](../api/eventmessage-list-attachments.md) |[attachment](attachment.md)-Sammlung| Ruft alle Anlagen für eine eventMessage ab.|
|[Hinzufügen einer Anlage](../api/eventmessage-post-attachments.md) |[attachment](attachment.md)| Fügt einer eventMessage eine neue Anlage durch Veröffentlichen in der Anlagensammlung hinzu.|
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Rufen Sie eine open Erweiterung namentlich identifiziert.|
|**Erweiterte Eigenschaften**| | |
|[Einwertige erweiterte Eigenschaft erstellen](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[eventMessage](eventmessage.md)  |Erstellt eine oder mehrere einwertige erweiterte Eigenschaften in einer neuen oder vorhandenen eventMessage.   |
|[eventMessage mit einer einwertigen erweiterten Eigenschaft abrufen](../api/singlevaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | Ruft mithilfe von `$expand` oder `$filter` eventMessages mit einer einwertigen erweiterten Eigenschaft ab. |
|[Mehrwertige erweiterte Eigenschaft erstellen](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [eventMessage](eventmessage.md) | Erstellt eine oder mehrere mehrwertige erweiterte Eigenschaften in einer neuen oder vorhandenen eventMessage.  |
|[eventMessage mit mehrwertiger erweiterter Eigenschaft abrufen](../api/multivaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | Ruft unter Verwendung von `$expand` eine eventMessage ab, die eine mehrwertige erweiterte Eigenschaft enthält. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "eventMessage resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/eventmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
