# <a name="create-and-send-outlook-messages"></a>Erstellen und Senden von Outlook-Nachrichten

E-Mails werden in Microsoft Graph durch die [message](../api-reference/v1.0/resources/message.md)-Ressource dargestellt.

Standardmäßig werden Nachrichten durch eine eindeutige Eintrags-ID in der **id**-Eigenschaft identifiziert. Ein Speicheranbieter weist einer Nachricht eine Eintrags-ID zu, wenn die Nachricht zuerst als Entwurf gespeichert oder gesendet wurde. Diese ID ändert sich, wenn die Nachricht kopiert oder in einen anderen Ordner, einen Store oder eine PST-Datei verschoben wird.

## <a name="creating-and-sending-mail"></a>Erstellen und Senden von Mail

In Outlook können Sie eine E-Mail in derselben [SendMail](../api-reference/v1.0/api/user_sendmail.md)-Aktion erstellen und senden, oder Sie können einen Entwurf [erstellen](../api-reference/v1.0/api/user_post_messages.md), anschließend [Inhalt hinzufügen](../api-reference/v1.0/api/message_update.md) und den Entwurf dann [senden](../api-reference/v1.0/api/message_send.md).

Wenn Sie auf eine E-Mail antworten, können Sie auf ähnliche Weise die Antwort in derselben Aktion erstellen und senden ([reply](../api-reference/v1.0/api/message_reply.md), [reply-all](../api-reference/v1.0/api//message_replyall.md) oder [forward](../api-reference/v1.0/api/message_forward.md)). Sie können auch einen Entwurf für die Antwort erstellen ([reply](../api-reference/v1.0/api/message_createreply.md), [reply-all](../api-reference/v1.0/api//message_createreplyall.md) oder [forward](../api-reference/v1.0/api/message_createforward.md)), [Inhalt hinzufügen](../api-reference/v1.0/api/message_update.md) und den Entwurf zu einem späteren Zeitpunkt [senden](../api-reference/v1.0/api/message_send.md).

Um programmgesteuert zwischen einem Entwurf und einer gesendeten Nachricht zu unterscheiden, überprüfen Sie die Eigenschaft **isDraft**.

Standardmäßig werden Nachrichtenentwürfe im Ordner `Drafts`gespeichert, und gesendete Nachrichten werden im Ordner `Sent Items` gespeichert. Sie können den Ordner für Entwürfe und den Ordner für gesendete Elemente auch einfach anhand ihrer [bekannten Ordnernamen](../api-reference/v1.0/resources/mailfolder.md) erkennen. Sie können z. B. Folgendes durchführen, um die [Nachrichten](../api-reference/v1.0/api/user_list_messages.md) im Ordner „Entwürfe“ abzurufen:

```http
GET /me/mailfolders('Drafts')
```

### <a name="body-format-and-malicious-script"></a>Textformat und bösartige Skripts

<!-- Remove the following 2 sections from the message.md topics
-->

Der Nachrichtentext kann entweder das HTML- oder Textformat aufweisen, wobei HTML der standardmäßige Nachrichtentexttyp ist, der bei einer GET-Antwort zurückgegeben wird.

Wenn Sie [eine Nachricht abrufen](../api-reference/v1.0/api/message_get.md), können Sie den folgenden Anforderungsheader angeben, um die Eigenschaften **body** und **uniqueBody** im Textformat zurückzugeben:

```http
Prefer: outlook.body-content-type="text"
```

Sie können den folgenden Header angeben oder ihn einfach überspringen, um den Nachrichtentext im HTML-Format zu erhalten:

```http
Prefer: outlook.body-content-type="html"
```

Wenn Sie einen der Header angeben, enthält eine erfolgreiche Antwort den entsprechenden `Preference-Applied`-Header:

- Für Textformatanforderungen: `Preference-Applied: outlook.body-content-type="text"`
- Für HTML-Formatanforderungen: `Preference-Applied: outlook.body-content-type="html"`

Wenn der Textkörper im HTML-Format vorliegt, entfernt Outlook standardmäßig alle potenziell unsicheren HTML-Elemente (z. B. JavaScript), die in der **body**-Eigenschaft eingebettet sind, vor dem Zurückgeben des Textkörperinhalts in einer REST-Antwort.

Um den gesamten ursprünglichen HTML-Inhalt abzurufen, schließen Sie den folgenden HTTP-Anforderungsheader ein:

```http
Prefer: outlook.allow-unsafe-html
```

### <a name="differentiating-the-from-and-sender-properties"></a>Unterscheiden der „Von“- und „Absender“-Eigenschaften

Wenn in Outlook eine Nachricht erstellt wird legt Outlook in den meisten Fällen denselben angemeldeten Benutzer für die Eigenschaften **from** und **sender** fest. Sie können diese Eigenschaften in den folgenden Szenarien aktualisieren:

- Die **from**-Eigenschaft kann geändert werden, wenn der Exchange-Administrator **sendAs**-Rechte des Postfachs anderen Benutzern zugewiesen hat. Der Administrator kann dies tun, indem er **Postfachberechtigungen** des Postfachbesitzers im Azure-Portal auswählt oder das Exchange Admin Center oder ein Windows PowerShell Add-ADPermission-Cmdlet verwendet. Dann können Sie programmgesteuert die **from**-Eigenschaft eines dieser Benutzer festlegen, die **sendAs**-Rechte für das Postfach haben.
- Die **sender**-Eigenschaft kann geändert werden, wenn der Postfachbesitzer das Recht, Nachrichten von diesem Postfach aus zu senden, an einen oder mehrere Benutzer delegiert hat. Der Postfachbesitzer kann in Outlook an einen Stellvertreter delegieren. Wenn ein Stellvertreter eine Nachricht im Namen des Postfachbesitzers sendet, legt Outlook die **sender**-Eigenschaft auf das Konto des Stellvertreters fest, während die **from**-Eigenschaft weiterhin den Postfachbesitzer angibt. Programmgesteuert können Sie die **sender**-Eigenschaft auf einen Benutzer festlegen, der Stellvertretungsberechtigungen für dieses Postfach besitzt.

## <a name="using-mailtips-to-check-recipient-status-and-save-time-preview"></a>Verwenden von MailTips zum Überprüfen des Empfängerstatus und Sparen von Zeit (Vorschau)

Mit [MailTips](../api-reference/beta/resources/mailtips.md) können Sie intelligente Entscheidungen treffen, bevor Sie eine E-Mail senden.
MailTips stellt Ihnen Informationen bereit, wie z. B. darüber, ob das Postfach eines Empfängers auf bestimmte Absender beschränkt ist oder ob zum Senden von E-Mails an den Empfänger eine Genehmigung erforderlich ist.

## <a name="integrating-with--social-gesture-preview"></a>Integration mit der Geste „@“ aus sozialen Netzwerken (Vorschau)

@-Erwähnungen sind Benachrichtigungen, um Benutzer darauf hinzuweisen, dass sie in Nachrichten erwähnt werden. Mit der [mention](../api-reference/beta/resources/mention.md)-Ressource können Apps die aus sozialen Netzwerken bekannte Geste, das Präfix „@“, in E-Mails festlegen und daraus abrufen.
Sie können:

- @-Erwähnungen beim [Erstellen einer Nachricht](../api-reference/beta/api/user_post_messages.md#request-2) erstellen
- [Alle Nachrichten im Postfach eines Benutzers abrufen, die eine @-Erwähnung des Benutzers beinhalten](../api-reference/beta/api/user_list_messages.md#request-2)
- [Alle @-Erwähnungen in einer Nachricht abrufen](../api-reference/beta/api/message_get.md#request-2)

## <a name="other-shared-capabilities"></a>Sonstige gemeinsam genutzte Funktionen

Nutzen Sie die Vorteile der folgenden gemeinsamen Funktionen, die von allen Entitäten in Microsoft Graph verwendet werden:

- Abonnieren Sie [Änderungsbenachrichtigungen](../api-reference/v1.0/resources/webhooks.md) für Nachrichten, wenn eine oder mehrere Typen von Änderungen auftreten, z. B. das Erstellen oder Aktualisieren von Nachrichten.
- [Verfolgen Sie diese inkrementellen Änderungen an Nachrichten in einem Ordner](delta_query_messages.md).
- Erstellen Sie [offene Erweiterungen](extensibility_overview.md#open-extensions) oder [Schemaerweiterungen](extensibility_overview.md#schema-extensions), um einer Nachrichteninstanz benutzerdefinierte Daten hinzuzufügen.
- Erstellen Sie [erweiterte Eigenschaften](../api-reference/v1.0/resources/extended-properties-overview.md) in einer Nachrichteninstanz, um benutzerdefinierte Daten für Outlook-MAPI-Eigenschaften zu speichern, wenn diese Eigenschaften in den Metadaten der Microsoft Graph-API noch nicht offengelegt wurden.

## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen:

- [Gründe für die Integration in Outlook-Mail](outlook-mail-concept-overview.md)
- [Verwenden der Mail-API](../api-reference/v1.0/resources/mail_api_overview.md) und [Anwendungsfälle](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) für diese in Microsoft Graph v1.0.


<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error: /concepts/outlook-create-send-messages.md:
        BookmarkSkippedDocFileNotFound: Link '[creating a message](../api-reference/beta/api/user_post_messages.md#request-2)'.",
    "Error: /concepts/outlook-create-send-messages.md:
      BookmarkSkippedDocFileNotFound: Link '[Get all the messages in a user's mailbox that contain an @-mention of the user](../api-reference/beta/api/user_list_messages.md#request-2)'.",
    "Error: /concepts/outlook-create-send-messages.md:
      BookmarkSkippedDocFileNotFound: Link '[Get all the @-mention is a message](../api-reference/beta/api/message_get.md#request-2)'."
  ]
}-->
