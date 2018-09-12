# <a name="mailtips-resource-type"></a>Ressourcentyp mailTips

Informative Nachrichten über einen Empfänger, die Benutzern beim Verfassen einer Nachricht angezeigt werden. Zum Beispiel eine Abwesenheitsnachricht als automatische Antwort für einen Nachrichtenempfänger.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| automaticReplies | [automaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | E-Mail-Info für die automatische Antwort, wenn sie vom Empfänger eingerichtet wurde. |
| customMailTip | Zeichenfolge | Eine benutzerdefinierte E-Mail-Info, die auf dem Postfach des Empfängers eingestellt werden kann. |
| deliveryRestricted| Boolesch | Ob das Postfach des Empfängers eingeschränkt ist, z. B. nur Nachrichten von einer vordefinierten Liste von Absendern annehmen, Nachrichten von einer vordefinierten Liste von Absendern ablehnen oder nur Nachrichten von authentifizierten Absendern annehmen. |
| emailAddress | [emailAddress](../resources/emailaddress.md) | Die E-Mail-Adresse des Empfängers, für den Sie E-Mail-Info erhalten möchten. |
| error | [mailTipsError](../resources/mailtipserror.md) | Fehler, die während der Aktion [getMailTips](../api/user_getmailtips.md) auftreten. |
| externalMemberCount | Int32 | Die Anzahl der externen Mitglieder, wenn der Empfänger eine Verteilerliste ist. |
| isModerated |Boolesch  | Ob das Versenden von Nachrichten an den Empfänger eine Genehmigung benötigt. Zum Beispiel, wenn der Empfänger eine große Verteilerliste ist und ein Moderator eingerichtet wurde, um an diese Verteilerliste gesendete Nachrichten zu genehmigen, oder wenn das Senden von Nachrichten an einen Empfänger die Genehmigung des Managers des Empfängers benötigt. |
| mailboxFull | Boolesch | Der Status Postfach voll des Empfängers. |
| maxMessageSize | Int32 | Die maximale Nachrichtengröße, die für die Organisation oder das Postfach des Empfängers konfiguriert wurde. |
| recipientScope | RecipientScopeType | Der Bereich des Empfängers. Mögliche Werte sind: `none`, `internal`, `external`, `externalPartner` und `externalNonParther`. Beispielsweise kann ein Administrator eine andere Organisation als "Partner" festlegen. Der Bereich ist nützlich, wenn ein Administrator möchte, dass bestimmte E-Mail-Info für bestimmte Bereiche zugänglich sind. Es ist auch nützlich, die Absender darüber zu informieren, dass ihre Nachricht die Organisation verlassen kann, um ihnen bei den richtigen Entscheidungen über Wortlaut, Ton und Inhalt zu helfen.|
| recipientSuggestions | [Empfänger](../resources/recipient.md)-Sammlung | Empfänger, die auf der Grundlage früherer Kontexte vorgeschlagen werden, in denen sie in der gleichen Nachricht erscheinen. |
| totalMemberCount | Int32 | Die Anzahl der Mitglieder, wenn der Empfänger eine Verteilerliste ist. |

### <a name="recipientscopetype-values"></a>RecipientScopeType-Werte

| Wert
|:-------------------------
| keine
| intern
| extern
| ExternalPartner
| ExternalNonPartner


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "automaticReplies",
    "customMailTip",
    "deliveryRestricted",
    "emailAddress",
    "error",
    "externalMemberCount",
    "isModerated",
    "mailboxFull",
    "maxMessageSize",
    "recipientScope",
    "recipientSuggestions",
    "totalMemberCount"
  ],
  "@odata.type": "microsoft.graph.mailTips"
}-->

```json
{
  "automaticReplies": {"@odata.type": "microsoft.graph.automaticRepliesMailTips"},
  "customMailTip": "string",
  "deliveryRestricted": "boolean",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "error": {"@odata.type": "microsoft.graph.mailTipsError"},
  "externalMemberCount": 1024,
  "isModerated": "boolean",
  "mailboxFull": "boolean",
  "maxMessageSize": 1024,
  "recipientScope": "string",
  "recipientSuggestions": [{"@odata.type": "microsoft.graph.recipient"}],
  "totalMemberCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
