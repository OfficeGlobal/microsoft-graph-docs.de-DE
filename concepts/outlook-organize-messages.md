# <a name="organize-outlook-messages"></a>Organisieren von Outlook-Nachrichten

In Outlook können Kunden ihre Nachrichten so organisieren, wie sie möchten: alle Nachrichten im gleichen Posteingangsordner, oder Nachrichten werden in Abhängigkeit von den jeweiligen Anforderungen in einer Ordnerstruktur unter dem Posteingang gespeichert. Nachrichten im gesamten Postfach des Benutzers oder in speziellen Ordner können ganz praktisch [gefiltert, gesucht oder sortiert](query_parameters.md) werden.

## <a name="accessing-mail-folders"></a>Zugreifen auf E-Mail-Ordner

Nachrichtenordner werden programmgesteuert von der [mailFolder](../api-reference/v1.0/resources/mailfolder.md)-Ressource dargestellt, und der Posteingang ist einer der Ordner am Stamm der Ordnerstruktur. Die `/users/{id}/mailfolders`-Verknüpfung stellt den Stamm dar. 

Jeder **mailFolder** wird durch seine Ordner-ID identifiziert und weist eine schreibbare **displayName**-Eigenschaft auf. Outlook erstellt standardmäßig ein paar andere Ordner für Kunden. Sie können auf diese Standardordner anhand ihrer Ordner-IDs oder anhand ihrer bekannten Namen verweisen: `ArchiveRoot`, `ConversationHistory`, `DeletedItems`, `Drafts`, `Inbox`, `JunkEmail`, `Outbox` und `SentItems`. 

Wenn Sie bei einem benutzerdefinierten, nicht standardmäßigen Ordner dessen Ordnerpfad kennen, können Sie auf den Ordner zugreifen, indem Sie zuerst die `/users/{id}/mailfolders` -Verknüpfung verwenden, um zur Stammebene zu gelangen, und dann alle Ordner der oberen Ebene abrufen:

```http
GET https://graph.microsoft.com/v1.0/users/{id}/mailFolders
```
Geben Sie dann die entsprechende Ordner-ID (`{folder_id}`) an, wenn Sie durch die einzelnen Ebenen der Ordnerstruktur navigieren:

```
GET https://graph.microsoft.com/v1.0/users/{id}/mailFolders/{folder_id}/childfolders
```
Wiederholen Sie diese Schritte, bis Sie schließlich zum benutzerdefinierten Ordner in der Struktur gelangen.

## <a name="creating-and-organizing-the-folder-tree"></a>Erstellen und Organisieren der Ordnerstruktur

Sie können [E-Mail-Ordner unter dem Posteingang erstellen](../api-reference/v1.0/api/user_post_mailfolders.md) oder [als untergeordnete Ordner von anderen Ordnern](../api-reference/v1.0/api/mailfolder_post_childfolders.md). Wenn Sie einen Ordner und seine Inhalte erstellen, [kopieren](../api-reference/v1.0/api/mailfolder_copy.md) oder [verschieben](../api-reference/v1.0/api/mailfolder_move.md), aktualisiert Outlook die schreibgeschützten Eigenschaften **parentFolderId** und **childFolderCount** der beteiligten Ordner. Wenn die Inhalte eines Ordners in einen anderen Ordner kopiert oder verschoben werden, ändern sich standardmäßig auch die einzelnen Eintrags-IDs der Inhalte.

Auf der Inhaltsebene erhalten Sie durch **totalItemCount** bzw. **unreadItemCount** die Anzahl der Elemente und die Anzahl der ungelesenen Elemente in einem E-Mail-Ordner.
Auf der Ebene der untergeordneten Ordner können Sie [die untergeordneten Ordner](../api-reference/v1.0/api/user_list_mailfolders.md) unter dem Posteingang oder einem beliebigen anderen Ordner auflisten. Die **childFolderCount**-Eigenschaft gibt die Anzahl der unmittelbar untergeordneten Ordner an.

Beachten Sie, dass Outlook-E-Mail-Ordner Nachrichtenelemente und Nicht-Nachrichtenelemente wie Ereignisse und Kontakte enthalten können. Im Allgemeinen können Outlook-Ordner heterogene Elemente enthalten.

## <a name="using-rules-to-automate-copying-or-moving-messages"></a>Verwenden von Regel zum Automatisieren des Kopierens oder Verschiebens von Nachrichten

<!-- Change links for rules API to v1 once it GAs in Feb. -->

In Outlook können Kunden Regeln einrichten, um bestimmte Aktionen für eingehende Nachrichten zu automatisieren, wenn einige zuvor festgelegten Bedingungen erfüllt sind. Sie können [eine Regel](../api-reference/beta/api/mailfolder_post_messagerules.md) für den Posteingang als eine [messageRule](../api-reference/beta/resources/messagerule.md) erstellen, um eine Nachricht bei bestimmten Bedingungen in einen bestimmten Ordner zu kopieren oder zu verschieben. Kriterien sind [messageRulePredicates](../api-reference/beta/resources/messagerulepredicates.md). Sie können den Nachrichtenbetreff oder -text mit bestimmten Formulierungen, die von bestimmten E-Mail-Adressen gesendeten Nachrichten oder eine als wichtig markierte Nachricht enthalten. 

## <a name="directing-only-the-messages-you-care-for-to-the-focused-inbox"></a>Weiterleiten der für Sie wichtigen Nachrichten an den Posteingang mit Relevanz 

Über den Posteingang mit Relevanz können Kunden Outlook so trainieren, dass nur die eingehenden Nachrichten von Absendern, die Ihnen wichtig sind, auf der Registerkarte **Relevant** und die restlichen Nachrichten auf der Registerkarte **Andere** angezeigt werden. Zu Beginn werden die Posteingangsnachrichten vom Klassifizierungssystem von Outlook standardmäßig organisiert. Im Laufe der Zeit können Sie das System über die Benutzeroberfläche oder programmgesteuert korrigieren oder trainieren. Je mehr Sie den Posteingang mit Relevanz verwenden, umso besser kann das Klassifizierungssystem ableiten, welche eingehenden Nachrichten auf der Registerkarte **Relevant** angezeigt werden sollen.

Sie können die **inferenceClassification**-Eigenschaft einer [Nachricht](../api-reference/v1.0/resources/message.md) programmgesteuert so aktualisieren, dass angegeben wird, ob die Nachricht auf der Registerkarte **Relevant** oder **Andere** angezeigt werden soll. Dies ist eine einmalige Bezeichnung für eine bestimmte Nachricht. Wenn Sie andererseits Nachrichten von einem bestimmten Absender immer auf der Registerkarte **Relevant** oder auf der Registerkarte **Sonstige** sehen möchten, können Sie für Outlook eine [Anweisung festlegen](../api-reference/v1.0/api/inferenceclassification_post_overrides.md). Jede Anweisung ist eine [inferenceClassificationOverride](../api-reference/v1.0/resources/inferenceclassificationoverride.md)-Instanz, die den Namen des Absenders und Ihre Bezeichnung für Nachrichten von diesem Absender als immer `focused` oder `other` angibt. Die Anweisungen jedes Benutzers für den Posteingang mit Relevanz des Benutzers werden als eine Sammlung von [inferenceClassificationOverride](../api-reference/v1.0/resources/inferenceclassificationoverride.md)-Instanzen für das [user](../api-reference/v1.0/resources/user.md)-Objekt gespeichert.

## <a name="keeping-messages-and-mail-folders-up-to-date-in-apps"></a>Nachrichten und E-Mail-Ordner in Apps auf dem neuesten Stand halten

Apps müssen häufig synchronisiert werden und die E-Mail-Daten eines Benutzers im lokalen App-Speicher auf dem neuesten Stand halten. Mit Microsoft Graph können Sie Änderungsbenachrichtigungen abonnieren, um eine Benachrichtigung zu erhalten, wenn sich Daten ändern, und tatsächliche Änderungen direkt bei ihrem Auftreten abzufragen.

Benachrichtigungen werden über [Webhooks](../api-reference/v1.0/resources/webhooks.md) asynchron gesendet, wenn die Änderungen auftreten, sodass den Apps der Aufwand des häufigen Abfragens erspart bleibt. Sie können [Änderungsbenachrichtigungen](../api-reference/v1.0/api/subscription_post_subscriptions.md) zu Ergänzungen, Updates oder Löschungen im Zusammenhang mit den E-Mail-Daten eines Benutzers abonnieren. Sie können z. B. ein Abonnement für Nachrichten in einem bestimmten Ordner (d. h. `/me/mailFolders('{folderId'}')`) oder auf der Stammebene (d. h. `/me/messages`) erstellen. Das Abonnement gibt eine **notificationUrl** an, unter der Microsoft Graph die App benachrichtigt, wenn die angeforderten Arten von Änderungen auftreten.

Um das Postfach eines Benutzers zum ersten Mal zu synchronisieren, führen Sie zunächst eine [Delta-Abfrage für E-Mail-Ordner, die auf der Stammebene beginnen, aus](../api-reference/v1.0/api/mailfolder_delta.md), um alle E-Mail-Ordner zu synchronisieren. Führen Sie dann eine [Delta-Abfrage für Nachrichten in den einzelnen Ordnern aus](../api-reference/v1.0/api/message_delta.md), um einzelnen Nachrichten zu synchronisieren.

Um die genauen Entitäten zu finden, die geändert wurden, ohne die gesamte Ressource bei jeder Benachrichtigung zu lesen, können Sie die [Delta-Abfrage](delta_query_overview.md) verwenden, um die Änderungen zu verfolgen, die Ihnen wichtig sind, und Ihren lokalen Speicher mit diesen Änderungen zu synchronisieren. Sie können [Änderungen an Nachrichten in einem bestimmten Ordner nachverfolgen](delta_query_messages.md). Es können auch Änderungen an E-Mail-Ordnern auf der Stammebene nachverfolgt werden (d. h. `/me/mailfolders`). 


## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen:

- [Gründe für die Integration in Outlook-Mail](outlook-mail-concept-overview.md)
- [Verwenden der Mail-API](../api-reference/v1.0/resources/mail_api_overview.md) und [Anwendungsfälle](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) für diese in Microsoft Graph v1.0.
