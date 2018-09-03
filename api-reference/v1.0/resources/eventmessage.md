# <a name="eventmessage-resource-type"></a>eventMessage-Ressourcentyp

Eine Nachricht, die für eine Besprechungsanfrage, -absage oder -antwort steht (diese kann folgende umfassen: Zusage, Zusage mit Vorbehalt oder Absage).

Die **eventMessage**-Entität wird von [message](message.md) abgeleitet. Die **meetingMessageType**-Eigenschaft gibt den Typ der Ereignisnachricht an.

Wenn ein Organisator oder eine App eine Besprechungsanfrage sendet, trifft die Besprechungsanfrage als eine **eventMessage**-Instanz mit **meetingMessageType** von **meetingRequest** in dem Postfach des Teilnehmers ein. Darüber hinaus erstellt Outlook automatisch eine **event**-Instanz im Kalender des Teilnehmers mit der **showAs**-Eigenschaft als **tentative**. 

Um die Eigenschaften des zugeordneten Ereignisses im Postfach des Teilnehmers abzurufen, kann die App die **event**-Navigationseigenschaft von **eventMessage** verwenden, wie in diesem [Beispiel zum Abrufen von Ereignisnachrichten](../api/eventmessage_get.md#request-2) dargestellt. Die App kann auch im Namen der Teilnehmer programmgesteuert auf dieses Ereignis antworten, indem Sie eine [Zusage](../api/event_accept.md), [, eine Zusage mit Vorbehalt](../api/event_tentativelyaccept.md) oder [eine Absage](../api/event_decline.md) sendet.

Neben einer Besprechungsanfrage wird eine **eventMessage**-Instanz infolge einer Besprechungsabsage eines Ereignisorganisators im Ordner „Posteingang“ des Teilnehmers, oder infolge einer Antwort auf die Besprechungsanfrage durch den Teilnehmer, im Posteingang des Organisators dargestellt. Eine App kann bei Ereignisnachrichten auf die gleiche Weise wie bei Nachrichten handeln, mit kleineren Unterschieden.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[eventMessage abrufen](../api/eventmessage_get.md) | [eventMessage](eventmessage.md) |Liest die Eigenschaften und Beziehungen eines eventMessage-Objekts.|
|[Aktualisieren](../api/eventmessage_update.md) | [eventMessage](eventmessage.md)  |Aktualisiert das eventMessage-Objekt. |
|[Löschen](../api/message_delete.md) | Keiner |Löscht das eventMessage-Objekt. |
|[copy](../api/message_copy.md)|[Nachricht](message.md)|Mit dieser API können Sie Nachrichten in Ordner kopieren.|
|[createForward](../api/message_createforward.md)|[Nachricht](message.md)|Erstellt einen Entwurf der Weiterleitungsnachricht. Sie können den Entwurf dann [aktualisieren](../api/message_update.md) oder [senden](../api/message_send.md).|
|[createReply](../api/message_createreply.md)|[Nachricht](message.md)|Erstellt einen Entwurf der Antwortnachricht. Sie können den Entwurf dann [aktualisieren](../api/message_update.md) oder [senden](../api/message_send.md).|
|[createReplyAll](../api/message_createreplyall.md)|[Nachricht](message.md)|Erstellt einen Entwurf der „Allen Antworten“-Nachricht. Sie können den Entwurf dann [aktualisieren](../api/message_update.md) oder [senden](../api/message_send.md).|
|[Weiterleiten](../api/message_forward.md)|Keine|Leitet eine Nachricht weiter. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|
|[Verschieben](../api/message_move.md)|[Nachricht](message.md)|Verschiebt eine Nachricht in einen Ordner. Dadurch wird eine neue Kopie der Nachricht im Zielordner erstellt.|
|[Antworten](../api/message_reply.md)|Keine|Antwortet auf eine Nachricht des Absenders. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|
|[replyAll](../api/message_replyall.md)|Keine|Sendet eine Antwort an alle Empfänger einer E-Mail. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|
|[Senden](../api/message_send.md)|Keine|Sendet einen zuvor erstellten Nachrichtenentwurf. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|
|**Anlagen**| | |
|[Anlagen auflisten](../api/eventmessage_list_attachments.md) |[attachment](attachment.md)-Sammlung| Ruft alle Anlagen für eine eventMessage ab.|
|[Hinzufügen einer Anlage](../api/eventmessage_post_attachments.md) |[Anlage](attachment.md)| Fügt einer eventMessage eine neue Anlage durch Veröffentlichen in der Anlagensammlung hinzu.|
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Ruft ein offenes Erweiterungsobjekt oder Objekte basierend auf ihrem Namen oder vollqualifizierten Namen ab.|
|**Erweiterte Eigenschaften**| | |
|[Einwertige erweiterte Eigenschaft erstellen](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[eventMessage](eventMessage.md)  |Erstellt eine oder mehrere einwertige erweiterte Eigenschaften in einer neuen oder vorhandenen eventMessage.   |
|[eventMessage mit einer einwertigen erweiterten Eigenschaft abrufen](../api/singlevaluelegacyextendedproperty_get.md)  | [eventMessage](eventMessage.md) | Ruft mithilfe von `$expand` oder `$filter` eventMessages mit einer einwertigen erweiterten Eigenschaft ab. |
|[Mehrwertige erweiterte Eigenschaft erstellen](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [eventMessage](eventMessage.md) | Erstellt eine oder mehrere mehrwertige erweiterte Eigenschaften in einer neuen oder vorhandenen eventMessage.  |
|[eventMessage mit mehrwertiger erweiterter Eigenschaft abrufen](../api/multivaluelegacyextendedproperty_get.md)  | [eventMessage](eventMessage.md) | Ruft unter Verwendung von `$expand` eine eventMessage ab, die eine mehrwertige erweiterte Eigenschaft enthält. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|bccRecipients|[Empfänger](recipient.md)-Sammlung|Die Bcc:-Empfänger der Nachricht.|
|Text|[itemBody](itembody.md)|Der Text der Nachricht. Er kann im HTML- oder Textformat vorliegen.|
|bodyPreview|Zeichenfolge|Die ersten 255 Zeichen des Nachrichtentexts. Liegt im Textformat vor.|
|Kategorien|Zeichenfolgenauflistung|Die Kategorien, die mit der Nachricht verknüpft sind.|
|ccRecipients|[Empfänger](recipient.md)-Sammlung|Die Cc:-Empfänger der Nachricht.|
|changeKey|Zeichenfolge|Die Version der Nachricht.|
|conversationId|Zeichenfolge|Die ID der Unterhaltung, zu der die E-Mail gehört.|
|createdDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht erstellt wurde.|
|Flag|[followupFlag](followupflag.md)|Der Flag-Wert, der den Status, das Startdatum, das Fälligkeitsdatum oder das Enddatum für die Nachricht angibt.|
|Von|[Empfänger](recipient.md)|Der Postfachbesitzer und der Absender der Nachricht.|
|hasAttachments|boolesch|Gibt an, ob die Nachricht Anlagen enthält.|
|ID|Zeichenfolge|Eindeutiger Bezeichner für die Nachricht (beachten Sie, dass sich dieser Wert ändern kann, wenn eine Nachricht verschoben oder geändert wird)|
|Wichtigkeit|Zeichenfolge| Wichtigkeit der Nachricht: `low`, `normal`, `high`.|
|inferenceClassification|Zeichenfolge| Die möglichen Werte sind: `focused`, `other`.|
|internetMessageHeaders | [internetinternetMessageHeaders](internetmessageheader.md)-Sammlung | Die Sammlung von Nachrichtenkopfzeilen, definiert von [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), die Informationen des von einer Nachricht vom Absender bis zum Empfänger verwendeten Pfads einer Nachricht liefert. Schreibgeschützt.|
|internetMessageId |Zeichenfolge |Die Nachrichten-ID im von [RFC2822](http://www.ietf.org/rfc/rfc2822.txt) angegebenen Format. |
|isDeliveryReceiptRequested|Boolesch|Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.|
|isDraft|Boolesch|Gibt an, ob die Nachricht ein Entwurf ist. Eine Nachricht ist ein Entwurf, solange sie noch nicht gesendet wurde.|
|isRead|Boolesch|Gibt an, ob die Nachricht gelesen wurde.|
|isReadReceiptRequested|Boolesch|Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.|
|lastModifiedDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht zuletzt geändert wurde.|
|meetingMessageType|meetingMessageType| Der Typ der Ereignisnachricht: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTenativelyAccepted`, `meetingDeclined`.|
|parentFolderId|Zeichenfolge|Der eindeutige Bezeichner für das übergeordnete mailFolder-Element der Nachricht.|
|receivedDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht erhalten wurde.|
|replyTo|[Empfänger](recipient.md)-Sammlung|Die E-Mail-Adressen, die beim Antworten verwendet werden sollen.|
|Absender|[Empfänger](recipient.md)|Das Konto, das tatsächlich verwendet wird, um die Nachricht zu generieren.|
|sentDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht gesendet wurde.|
|Betreff|Zeichenfolge|Der Betreff der Nachricht.|
|toRecipients|[Empfänger](recipient.md)-Sammlung|Die An:-Empfänger der Nachricht.|
|uniqueBody|[itemBody](itembody.md)|Der Teil des Textkörpers der Nachricht, der für die aktuelle Nachricht eindeutig ist.|
|webLink|Zeichenfolge|Die URL zum Öffnen der Nachricht in Outlook Web App.<br><br>Sie können am Ende der URL das Argument „ispopout“ anhängen, um zu ändern, wie die Nachricht angezeigt wird. Wenn „ispopout“ nicht vorhanden oder auf 1 festgelegt ist, wird die Nachricht in einem Popout-Fenster angezeigt. Wenn „ispopout“ auf 0 festgelegt ist, zeigt der Browser die Nachricht in Outlook Web App im Prüffensterbereich an.<br><br>Die Nachricht wird im Browser geöffnet, wenn Sie über Outlook Web App bei Ihrem Postfach angemeldet sind. Sie werden aufgefordert, sich anzumelden, wenn Sie noch nicht beim Browser angemeldet sind.<br><br>Auf diese URL kann von einem iFrame aus zugegriffen werden.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Anlagen|[attachment](attachment.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu.|
|Ereignis|[Ereignis](event.md)| Das Ereignis, das der Ereignisnachricht zugeordnet ist. Für Teilnehmer oder Raumressourcen wird davon ausgegangen, dass die Kalenderautomatik für die automatische Aktualisierung des Kalenders mit einem Ereignis festgelegt ist, wenn Ereignisnachrichten mit Besprechungsanfragen eingehen Navigationseigenschaft.  Schreibgeschützt.|
|Erweiterungen|[extension](extension.md)-Sammlung|Die Sammlung der für das Ereignis definierten offenen Erweiterungen. Schreibgeschützt. Lässt NULL-Werte zu.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung| Die Sammlung der für die eventMessage definierten mehrwertigen erweiterten Eigenschaften. Schreibgeschützt. Lässt Nullwerte zu.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung| Die Sammlung der für die eventMessage definierten einwertigen erweiterten Eigenschaften. Schreibgeschützt. Lässt Nullwerte zu.|

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
  "baseType": "microsoft.graph.message",
  "@odata.type": "microsoft.graph.eventMessage",
  "@odata.annotations": [
    {
      "property": "event",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
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
  "createdDateTime": "DateTimeOffset",
  "event": { "@odata.type": "microsoft.graph.event" },
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageHeaders": [{"@odata.type": "microsoft.graph.internetMessageHeader"}],
  "internetMessageId": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "DateTimeOffset",
  "meetingMessageType": "String",
  "parentFolderId": "string",
  "receivedDateTime": "DateTimeOffset",
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "DateTimeOffset",
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "eventMessage resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
