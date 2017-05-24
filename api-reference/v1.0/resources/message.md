# <a name="message-resource-type"></a>Nachrichtenressourcentyp

Dieser Ressourcentyp stellt eine Nachricht in einem mailFolder-Objekt dar.

Diese Ressource unterstützt Folgendes:

- Hinzufügen Ihrer eigenen Daten zu benutzerdefinierten Eigenschaften mithilfe von [Erweiterungen](../../../concepts/extensibility_overview.md).
- Verwenden einer [Delta-Abfrage](../../../concepts/delta_query_overview.md) zum Nachverfolgen von inkrementellen Hinzufügungen, Löschungen und Aktualisierungen durch Bereitstellen der [delta](../api/message_delta.md)-Funktion.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Nachrichten auflisten](../api/user_list_messages.md) |Sammlung von [Nachrichten](message.md) | Dient zum Abrufen aller Nachrichten im Postfach des angemeldeten Benutzers (einschließlich der Ordner „Gelöschte Elemente“ und „Clutter“). |
|[Nachricht erstellen](../api/user_post_messages.md) | [Nachricht](message.md) | [Erstellt](../api/user_post_messages.md#request-1) einen Entwurf einer neuen Nachricht. |
|[Nachricht abrufen](../api/message_get.md) | [Nachricht](message.md) |Liest Eigenschaften und Beziehungen des Nachrichtenobjekts.|
|[Aktualisieren](../api/message_update.md) | [Nachricht](message.md) |Aktualisiert das Nachrichtenobjekt.|
|[Löschen](../api/message_delete.md) | Keiner |Löscht das Nachrichtenobjekt. |
|[Kopieren](../api/message_copy.md)|[Nachricht](message.md)|Kopiert eine Nachricht in einen Ordner.|
|[createForward](../api/message_createforward.md)|[Nachricht](message.md)|Erstellt einen Entwurf der Weiterleitungsnachricht. Sie können den Entwurf dann [aktualisieren](../api/message_update.md) oder [senden](../api/message_send.md).|
|[createReply](../api/message_createreply.md)|[Nachricht](message.md)|Erstellt einen Entwurf der Antwortnachricht. Sie können den Entwurf dann [aktualisieren](../api/message_update.md) oder [senden](../api/message_send.md).|
|[createReplyAll](../api/message_createreplyall.md)|[Nachricht](message.md)|Erstellt einen Entwurf der „Allen Antworten“-Nachricht. Sie können den Entwurf dann [aktualisieren](../api/message_update.md) oder [senden](../api/message_send.md).|
|[delta](../api/message_delta.md)|[message](message.md)-Sammlung| Dient zum Abrufen eines Satzes von Nachrichten, die einem bestimmten Ordner hinzugefügt bzw. daraus gelöscht oder darin aktualisiert wurden.|
|[forward](../api/message_forward.md)|Keine|Leitet eine Nachricht weiter. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|
|[Verschieben](../api/message_move.md)|[Nachricht](message.md)|Verschiebt eine Nachricht in einen Ordner. Dadurch wird eine neue Kopie der Nachricht im Zielordner erstellt.|
|[Antworten](../api/message_reply.md)|Keine|Antwortet auf eine Nachricht des Absenders. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|
|[replyAll](../api/message_replyall.md)|Keine|Sendet eine Antwort an alle Empfänger einer E-Mail. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|
|[Senden](../api/message_send.md)|Keine|Sendet einen zuvor erstellten Nachrichtenentwurf. Die Nachricht wird dann im Ordner „Gesendete Elemente“ gespeichert.|
|**Anlagen**| | |
|[Anlagen auflisten](../api/message_list_attachments.md) |[Anlagensammlung](attachment.md)| Ruft alle Anlagen in einer Nachricht ab.|
|[Hinzufügen einer Anlage](../api/message_post_attachments.md) |[Anlage](attachment.md)| Fügt einer Nachricht eine neue Anlage durch Veröffentlichen in der Anlagensammlung hinzu.|
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften in einer neuen oder vorhandenen Instanz einer Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Ruft ein offenes Erweiterungsobjekt oder Objekte basierend auf ihrem Namen oder vollqualifizierten Namen ab.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](../../../concepts/extensibility_schema_groups.md) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|
|**Erweiterte Eigenschaften**| | |
|[Einwertige erweiterte Eigenschaft erstellen](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[Nachricht](message.md)  |Erstellt eine oder mehrere einwertige erweiterte Eigenschaften in einer neuen oder vorhandenen Nachricht.   |
|[Nachricht mit einwertiger erweiterter Eigenschaft abrufen](../api/singlevaluelegacyextendedproperty_get.md)  | [Nachricht](message.md) | Ruft mithilfe von `$expand` oder `$filter` Nachrichten mit einer einwertigen erweiterten Eigenschaft ab. |
|[Mehrwertige erweiterte Eigenschaft erstellen](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [Nachricht](message.md) | Erstellt eine oder mehrere mehrwertige erweiterte Eigenschaften in einer neuen oder vorhandenen Nachricht.  |
|[Nachricht mit mehrwertiger erweiterter Eigenschaft abrufen](../api/multivaluelegacyextendedproperty_get.md)  | [Nachricht](message.md) | Ruft eine Nachricht mit einer mehrwertigen erweiterten Eigenschaft mithilfe von `$expand` ab. |


## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|bccRecipients|[recipient](recipient.md) collection|Die Bcc:-Empfänger der Nachricht.|
|body|[itemBody](itembody.md)|Der Text der Nachricht. Er kann im HTML- oder Textformat vorliegen.|
|bodyPreview|Zeichenfolge|Die ersten 255 Zeichen des Nachrichtentexts. Liegt im Textformat vor.|
|categories|String collection|Die Kategorien, die mit der Nachricht verknüpft sind.|
|ccRecipients|[recipient](recipient.md) collection|Die Cc:-Empfänger der Nachricht.|
|changeKey|String|Die Version der Nachricht.|
|conversationId|String|Die ID der Unterhaltung, zu der die E-Mail gehört.|
|createdDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht erstellt wurde.|
|Von|[Empfänger](recipient.md)|Der Postfachbesitzer und der Absender der Nachricht.|
|hasAttachments|Boolean|Gibt an, ob die Nachricht Anlagen enthält.|
|ID|String|Eindeutiger Bezeichner für die Nachricht (beachten Sie, dass sich dieser Wert ändern kann, wenn eine Nachricht verschoben oder geändert wird)|
|Wichtigkeit|String| Wichtigkeit der Nachricht: `Low`, `Normal`, `High`.|
|inferenceClassification | String | Die Klassifizierung der Nachricht für den Benutzer, basierend auf der abgeleiteten Relevanz oder Wichtigkeit oder auf einer expliziten Außerkraftsetzung. Mögliche Werte sind: `focused` oder `other`. |
|internetMessageId |String |Die Nachrichten-ID im von [RFC2822](http://www.ietf.org/rfc/rfc2822.txt) angegebenen Format. |
|isDeliveryReceiptRequested|Boolean|Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.|
|isDraft|Boolean|Gibt an, ob die Nachricht ein Entwurf ist. Eine Nachricht ist ein Entwurf, solange sie noch nicht gesendet wurde.|
|isRead|Boolean|Gibt an, ob die Nachricht gelesen wurde.|
|isReadReceiptRequested|Boolean|Zeigt an, ob für die Nachricht eine Lesebestätigung angefordert wird.|
|lastModifiedDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht zuletzt geändert wurde.|
|parentFolderId|String|Der eindeutige Bezeichner für das übergeordnete mailFolder-Element der Nachricht.|
|receivedDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht erhalten wurde.|
|replyTo|[recipient](recipient.md) collection|Die E-Mail-Adressen, die beim Antworten verwendet werden sollen.|
|sender|[Empfänger](recipient.md)|Das Konto, das tatsächlich verwendet wird, um die Nachricht zu generieren.|
|sentDateTime|DateTimeOffset|Das Datum und die Uhrzeit, zu der die Nachricht gesendet wurde.|
|Betreff|String|Der Betreff der Nachricht.|
|toRecipients|[recipient](recipient.md) collection|Die An:-Empfänger der Nachricht.|
|uniqueBody|[itemBody](itembody.md)|Der Teil des Nachrichtentexts, der nur in der aktuellen Nachricht vorhanden ist. **uniqueBody** wird nicht standardmäßig zurückgegeben, kann aber für eine bestimmte Nachricht mithilfe der Abfrage `?$select=uniqueBody` abgerufen werden. Er kann im HTML- oder Textformat vorliegen.|
|webLink|String|Die URL zum Öffnen der Nachricht in Outlook Web App.<br><br>Sie können am Ende der URL das Argument „ispopout“ anhängen, um zu ändern, wie die Nachricht angezeigt wird. Wenn „ispopout“ nicht vorhanden oder auf 1 festgelegt ist, wird die Nachricht in einem Popout-Fenster angezeigt. Wenn „ispopout“ auf 0 festgelegt ist, zeigt der Browser die Nachricht in Outlook Web App im Prüffensterbereich an.<br><br>Die Nachricht wird im Browser geöffnet, wenn Sie über Outlook Web App bei Ihrem Postfach angemeldet sind. Sie werden aufgefordert, sich anzumelden, wenn Sie noch nicht beim Browser angemeldet sind.<br><br>Auf diese URL kann von einem iFrame aus zugegriffen werden.|

**Entfernen von Skript aus den body-Eigenschaft**

Der Nachrichtentext im HTML- oder Textformat vorliegen. Wenn der Textkörper im HTML-Format vorliegt, werden standardmäßig alle potenziell unsicheren HTML-Elemente (z. B. JavaScript), die in der **body**-Eigenschaft eingebettet sind, vor dem Zurückgeben des Textkörperinhalts in einer REST-Antwort entfernt. Um den gesamten ursprünglichen HTML-Inhalt abzurufen, schließen Sie den folgenden HTTP-Anforderungsheader ein:
```
Prefer: outlook.allow-unsafe-html
```

**Festlegen der from- und sender-Eigenschaften**

Beim Schreiben einer Nachricht stellen in den meisten Fällen die From- und Sender-Eigenschaften den gleichen angemeldeten Benutzer dar, es sei denn, eine der beiden Eigenschaften wird wie in den folgenden Szenarien beschrieben aktualisiert:

- Die **from**-Eigenschaft kann geändert werden, wenn der Exchange-Administrator **sendAs**-Rechte des Postfachs anderen Benutzern zugewiesen hat. Der Administrator kann dies tun, indem er **Postfachberechtigungen** des Postfachbesitzers im Azure-Verwaltungsportal auswählt oder das Exchange Admin Center oder ein Windows PowerShell Add-ADPermission-Cmdlet verwendet. Dann können Sie programmgesteuert die **from**-Eigenschaft eines dieser Benutzer festlegen, die **sendAs**-Rechte für das Postfach haben.
- Die **sender**-Eigenschaft kann geändert werden, wenn der Postfachbesitzer das Recht, Nachrichten von diesem Postfach aus zu senden, an einen oder mehrere Benutzer delegiert hat. Der Postfachbesitzer kann in Outlook an einen Stellvertreter delegieren. Wenn ein Stellvertreter eine Nachricht im Namen des Postfachbesitzers sendet, ist die **sender**-Eigenschaft auf das Konto des Stellvertreters festgelegt, während die **from**-Eigenschaft weiterhin den Postfachbesitzer angibt. Programmgesteuert können Sie die **sender**-Eigenschaft auf einen Benutzer festlegen, der Stellvertretungsrechte für dieses Postfach besitzt.

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|attachments|[attachment](attachment.md)-Sammlung|Die [fileAttachment](fileattachment.md)- und [itemAttachment](itemattachment.md)-Anlagen der Nachricht.|
|Erweiterungen|[extension](extension.md)-Sammlung|Die Sammlung der für die Nachricht definierten offenen Erweiterungen. Schreibgeschützt. Lässt NULL-Werte zu.|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)-Sammlung| Die Sammlung der für die Nachricht definierten mehrwertigen erweiterten Eigenschaften. Schreibgeschützt. Lässt NULL-Werte zu.|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)-Sammlung| Die Sammlung der für die Nachricht definierten einwertigen erweiterten Eigenschaften. Schreibgeschützt. Lässt Nullwerte zu.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "extensions",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.message"
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
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageId": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "parentFolderId": "string",
  "receivedDateTime": "String (timestamp)",
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string"
}

```

## <a name="see-also"></a>Siehe auch

- [Postfacheinstellungen abrufen](../api/user_get_mailboxsettings.md) 
- [Postfacheinstellungen aktualisieren](../api/user_update_mailboxsettings.md)
- [Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten](../../../concepts/delta_query_overview.md)
- [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](../../../concepts/delta_query_messages.md)
- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](../../../concepts/extensibility_overview.md)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](../../../concepts/extensibility_open_users.md)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
