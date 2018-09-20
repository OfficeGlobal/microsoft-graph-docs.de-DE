# <a name="outlook-mail-api-overview"></a>Übersicht über die Outlook-Mail-API

Outlook ist ein Messaging-Hub in Office 365. Neben den Messagingfeatures bietet die Lösung Funktionen, mit denen Sie Ihre Kontakte verwalten, Besprechungen planen, Informationen zu Benutzern in Ihrem Unternehmen suchen, Onlineunterhaltungen initiieren, Dateien teilen und in Gruppen zusammenarbeiten können.

## <a name="why-integrate-with-outlook-mail"></a>Gründe für die Integration mit Outlook-Mail

### <a name="integrate-with-rich-features-and-reach-hundreds-of-millions-of-customers"></a>Integration von funktionsreichen Features und Zielgruppe von Hunderten Millionen Kunden

Eine Integration mit Outlook verschafft Ihnen Zugang zu dem weitreichenden Funktionsumfang, den Kunden so schätzen: einer konsistenten und intuitiven Oberfläche für E-Mails, [Kontakte](outlook-contacts-concept-overview.md) und [Kalender](outlook-calendar-concept-overview.md), die geräteunabhängig zur Verfügung steht – auf Mobilgeräten ebenso wie im Web und auf Desktop-PCs.

Möglich wird die Integration mit Outlook dank [Microsoft Graph](overview.md). Sie müssen Ihre App nur ein einziges Mal programmieren und können dann Hunderte Millionen Heimanwender sowie Unternehmenskunden im zweistelligen Millionenbereich erreichen, die Outlook als E-Mail-Client verwenden. Dabei können sich Ihre Apps auf E-Mail-Szenarien beschränken oder auch eine Vielzahl anderer Outlook-basierter und nicht Outlook-basierter Beziehungen, Ressourcen und Informationen nutzen. Auch von der Microsoft-Cloud unterstützte Szenarien lassen sich umsetzen.

### <a name="automate-message-organization-and-processing"></a>Automatisierung von Nachrichtenorganisation und -verarbeitung

Kunden schätzen, dass sie mit Outlook immer perfekt organisiert sein können. Microsoft Graph macht diese Features für App-Entwickler verfügbar. So können Sie Kundenworkflows erstellen, die die Suche optimieren und Effizienz sowie Produktivität steigern: 

- Jeder Kunde organisiert seine Nachrichten auf seine eigene Art. Manche belassen sämtliche Nachrichten im Posteingang und suchen sie bei Bedarf, andere sortieren sie in Ordner ein. Alle schätzen den flexiblen und intuitiven Ansatz von Outlook, der sowohl eine flache als auch eine ordnerbasierte Organisationsstruktur unterstützt. Apps können Nachrichten bequem [filtern, suchen oder sortieren](query_parameters.md), wahlweise innerhalb bestimmter Ordner oder im gesamten Postfach des Benutzers.

- Outlook-Kategorien haben jeweils einen eigenen Namen und eine eigene Farbe. Mithilfe von Kategorien können Kunden Nachrichten taggen und so Ordnung und Auffindbarkeit verbessern. Apps können [auf die Hauptkategorienliste des Benutzers zugreifen und sie definieren](../api-reference/v1.0/api/outlookuser_post_mastercategories.md). Besser noch: Eine solche Liste deckt alle Outlook-Nachrichten sowie Termine, Kontakte, Aufgaben und Gruppenbeiträge ab und eröffnet App-Entwicklern so kreative Szenarien. So kann ein Anbieter von Onlineschulungen beispielsweise einen Farbcode für E-Mails, Kurstermine und Folgearbeitsaufträge festlegen, für jeden Kurs, für den ein Benutzer registriert ist.

- App-Benutzer können darüber hinaus die Wichtigkeit einer Nachricht (oder eines Termins oder einer Aufgabe) ändern und Nachrichten zur Nachverfolgung kennzeichnen. (Die Kennzeichnungsfunktion in Microsoft Graph befindet sich derzeit in der [Preview-Phase](versioning_and_support.md#beta-version).)

- Die Regeln-API erlaubt eine Nachrichtenorganisation auf ganz neuem Niveau. Apps können [Posteingangsregeln](../api-reference/v1.0/resources/messagerule.md) einrichten, sodass eingehende Nachrichten schnell verarbeitet werden und die Übersichtlichkeit des Posteingangs verbessert wird. Eine App kann Nachrichten beispielsweise automatisch in einen anderen Ordner verschieben, wenn die Betreffzeile bestimmte Schlüsselwörter enthält, sowie zwecks einfacherer Nachverfolgung Kategorien und Wichtigkeit zuweisen.

### <a name="write-smarter-apps-that-leverage-intelligence"></a>Intelligentere Apps mit Zugriff auf umfangreiche Informationen 

Mit Microsoft Graph können Sie den Benutzern Ihrer App kontextbasiert Daten vorschlagen:

- Eine Integration von [Posteingang mit Relevanz](../api-reference/v1.0/resources/manage_focused_inbox.md) und [@-Erwähnungen (Preview)](../api-reference/beta/api/message_get.md#request-2) erlaubt es Ihren Benutzern, zuerst die Nachrichten zu lesen und zu beantworten, die für sie am relevantesten sind. 

- [E-Mail-Tipps](../api-reference/v1.0/resources/mailtips.md) liefern während des Verfassens einer Nachricht nützliche Statusinformationen zum Empfänger (z. B. ob der Empfänger aktuell automatische Antworten sendet oder ob sein Postfach voll ist). E-Mail-Tipps können Apps informieren, wenn bestimmte Bedingungen erfüllt sind. So kann die jeweils effizientere Follow-up-Aktion gewählt werden. 

- Über die [Personen-API](people_example.md) können Sie in Ihrer App interaktive Steuerelemente wie eine Personenauswahl bereitstellen. Die Personen-API kann dem Benutzer die für ihn relevantesten Personen vorschlagen, basierend auf seinen Kommunikations- und Zusammenarbeitsmustern sowie seinen geschäftlichen Beziehungen. 

- Stellen Sie den Benutzern Ihrer App eine intelligente Dateiauswahl zur Verfügung, die ihnen beim Verfassen einer Nachricht ihre zuletzt genutzten Dateien als mögliche Anlagen anbietet. [Insights (Vorschauversion)](../api-reference/beta/resources/insights.md) nutzt erweiterte Analysen, um dem Benutzer Dateien vorzuschlagen, die für ihn besonders relevant sind, die er kürzlich angesehen oder bearbeitet hat oder die mit ihm geteilt wurden.


### <a name="store-app-data-in-a-resource-or-resource-instance"></a>Speicherung von App-Daten in Ressourcen oder Ressourceninstanzen

Apps müssen ihre Daten oft in einem externen Datenspeicher speichern, was Overhead durch Datenverwaltung und Datenzugriff nach sich zieht. Mit Microsoft Graph lassen sich App-Daten beim [Erstellen](../api-reference/v1.0/api/user_post_messages.md#request-2) oder [Senden](../api-reference/v1.0/api/user_sendmail.md#request-2) neuer Nachrichten oder beim Beantworten von Nachrichten einfach als Kopfzeile der Internet-Nachricht eingefügen. 

Um benutzerdefinierte Daten hinzuzufügen und anschließend zu aktualisieren, können Sie [die Daten in einzelnen Ressourceninstanzen speichern](extensibility_overview.md#open-extensions). Alternativ können Sie das Schema gegebenenfalls erweitern, benutzerdefinierte Eigenschaften hinzufügen und typisierte Daten in Microsoft Graph-Ressourcen speichern. Solche [Schemaerweiterungen](extensibility_overview.md#schema-extensions) können suchbar und teilbar gemacht werden. 


## <a name="next-steps"></a>Nächste Schritte

- Wählen Sie im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0) Outlook-Mail-Beispielabfragen zum Testen aus. Klicken Sie in der Spalte links auf **Show more samples**. Aktivieren Sie über das Menü **Outlook-Mail**.
- Informieren Sie sich über folgende Themen:

  - [Erstellen und Senden von Nachrichten](outlook-create-send-messages.md)
  - Möglichkeiten zum [Organisieren von Nachrichten](outlook-organize-messages.md)
  - Wie man [freigegebene Nachrichten abruft](outlook-share-messages-folders.md)

- Informieren Sie sich über die [Arbeit mit der Mail-API](../api-reference/v1.0/resources/mail_api_overview.md) und die [Anwendungsfälle](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) der API in Microsoft Graph 1.0.


