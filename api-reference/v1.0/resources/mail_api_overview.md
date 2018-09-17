# <a name="use-the-outlook-mail-rest-api"></a>Verwenden der Outlook-Mail-REST-API

Mit Microsoft Graph kann Ihre App autorisierten Zugriff auf die E-Mail-Daten eines Benutzers in einem persönlichen oder Organisationskonto in Outlook erhalten. Mit den [entsprechenden delegierten Berechtigungen oder Anwendungsberechtigungen](../../../concepts/permissions_reference.md) kann die App auf die E-Mail-Daten des angemeldeten Benutzers oder eines beliebigen Benutzers in einem Mandanten zugreifen. Die E-Mail-Daten können sich in der Cloud in Exchange Online als Teil von Office 365 oder in einer lokalen Exchange-Installation in einer [Hybridbereitstellung](../../../concepts/hybrid_rest_support.md) befinden.

## <a name="using-the-mail-rest-api"></a>Verwenden der E-Mail-REST-API

E-Mail-API-Anforderungen werden im Auftrag eines [Benutzers](../resources/user.md) ausgeführt, der durch die Eigenschaft **ID** des Benutzers (eine eindeutige GUID), die E-Mail-Adresse oder die Aliasverknüpfung `me` für den angemeldeten Benutzer identifiziert werden kann.

E-Mail-Nachrichten werden durch die Ressource [message](../resources/message.md) dargestellt und in einem [mailFolder](../resources/mailfolder.md) organisiert. Nachrichten und E-Mail-Ordner werden durch ihre Eigenschaft **ID** identifiziert, die mit `GET`-Operationen abgerufen werden kann.

>**Hinweis:** Gehen Sie im Allgemeinen nicht davon aus, dass die IDs von **message** und **mailfolder** in einem Postfach eindeutig und unveränderlich sind. Sie können sich nach bestimmten Aktionen wie z. B. Kopieren, Verschieben oder Senden ändern.

Nachrichtentext kann im HTML- oder Textformat vorliegen.

Sie können bekannte Ordnernamen wie `Inbox`, `Drafts`, `SentItems` oder `DeletedItems` verwenden, um bestimmte, standardmäßig für alle Benutzer vorhandene Mail-Ordner einfacher zu identifizieren. Eine Liste der unterstützten bekannten Ordnernamen finden Sie unter [mailFolder-Ressourcentyp](../resources/mailfolder.md).

So können Sie beispielsweise Nachrichten im Outlook-Ordner **Gesendete Elemente** des angemeldeten Benutzers erhalten, ohne zuvor die Ordner-ID erhalten zu haben:

```http
GET /me/mailFolders('SentItems')/messages?$select=sender,subject
```

## <a name="common-use-cases"></a>Allgemeine Anwendungsfälle

Die Ressource **message** macht Eigenschaften wie **categories**, **conversationId**, **flag** und **importance** verfügbar, die Features in der Benutzeroberfläche entsprechen, sodass Apps die integrierte Outlook-Benutzeroberfläche automatisieren oder integrieren können.

Die Microsoft Graph-API stellt zudem Methoden und Aktionen bereit, die allgemeine Anwendungsfälle von Nachrichten unterstützen.

| Anwendungsfälle | REST-Ressourcen | Siehe auch |
|:----------|:---------------|:---------|
| **Benutzerorientierte Aktionen** | | |
| Nachrichten entwerfen, lesen, beantworten, weiterleiten, senden, aktualisieren oder löschen | [message](../resources/message.md) | [Methoden von „message“](../resources/message.md#methods) |
| Das Versenden von Nachrichten im Auftrag des Postfachbesitzers an einen anderen Benutzer delegieren | [message](../resources/message.md) | Festlegen der Eigenschaften **from** und **sender** in einer [Nachricht](../resources/message.md) |
| Wichtigere Nachrichten zuerst anzeigen | [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md) | [Posteingang mit Fokus](../resources/manage_focused_inbox.md) |
| Anlagen einer Nachricht hinzufügen, abrufen oder löschen | [attachment](../resources/attachment.md), <br> [fileAttachment](../resources/fileattachment.md), <br> [itemAttachment](../resources/itemattachment.md), <br> [referenceAttachment](../resources/referenceattachment.md), <br> [message](../resources/message.md) | [Methoden von „attachment“](../resources/attachment.md#methods) |
| Automatische Antwort, Gebietsschema, Zeitzone oder Arbeitszeiten eines Benutzers abrufen oder aktualisieren | [mailboxSettings](../resources/mailboxsettings.md), <br> [automaticRepliesSetting](../resources/automaticrepliessetting.md), <br> [localeInfo](../resources/localeinfo.md), <br> [workingHours](../resources/workinghours.md) | [Postfacheinstellungen des Benutzers abrufen](../api/user_get_mailboxsettings.md) <br> [Postfacheinstellungen des Benutzers aktualisieren](../api/user_update_mailboxsettings.md) |
| Abrufen von E-Mail-Infos von anderen Empfänger spezielle Status, z.B. Abwesenheitsbenachrichtigungen | [user](../resources/user.md), <br> [mailTips](../resources/mailtips.md) | [Abrufen von E-Mail-Infos](../api/user_getmailtips.md) |
| **E-Mail- und Ordnerverwaltung** | | |
| Nachrichten in einer E-Mail-Ordnerhierarchie organisieren | [mailFolder](../resources/mailfolder.md)  | [Methoden von „mailFolder“](../resources/mailfolder.md#methods) |
| Nachrichten suchen und filtern | [message](../resources/message.md) | [Abfrageparameter](../../../concepts/query_parameters.md)  |
| Benachrichtigung über Änderungen an Nachrichten in einem Ordner erhalten | [subscription](../resources/subscription.md) | [Arbeiten mit Webhooks in Microsoft Graph](../resources/webhooks.md) |
| Nachrichten oder eine E-Mail-Ordnerhierarchie synchronisieren | [message](../resources/message.md) | [Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen](../../../concepts/delta_query_messages.md) |
| **App-Entwicklung** | | |
| Hinzufügen von benutzerdefinierten App-Daten als Internet-Nachrichten-Header einer Nachricht | [message](../resources/message.md) | Hinzufügen von benutzerdefinierten Daten an die **InternetMessageHeaders**-Eigenschaft der Nachricht. |
| Benutzerdefinierte App-Daten mithilfe von Erweiterungen zu einer Nachricht hinzufügen | [openTypeExtension](../resources/opentypeextension.md), <br>[schemaExtension](../resources/schemaextension.md) | [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](../../../concepts/extensibility_overview.md) |
| Auf benutzerdefinierte Daten für nicht ausreichend verfügbare Outlook-MAPI-Eigenschaften zugreifen | [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), <br> [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) | [Übersicht über erweiterte Outlook-Eigenschaften](../resources/extended-properties-overview.md) |

## <a name="next-steps"></a>Nächste Schritte

Die E-Mail-API kann Ihnen neue Möglichkeiten für die Interaktion mit Benutzern eröffnen:

- [Übersicht über die Outlook-Mail-API](../../../concepts/outlook-mail-concept-overview.md)
- Führen Sie einen Drilldown für die [Methoden](../resources/message.md#methods), [Eigenschaften](../resources/message.md#properties) und [Beziehungen](../resources/message.md#relationships) der Ressourcen [message](../resources/message.md) und [mailFolder](../resources/mailfolder.md) aus.
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/en-us/graph/graph-explorer) aus.

Benötigen Sie weitere Ideen? Dann sehen Sie sich an, [wie unsere Partner Microsoft Graph verwenden](https://developer.microsoft.com/en-us/graph/graph/examples#partners).
