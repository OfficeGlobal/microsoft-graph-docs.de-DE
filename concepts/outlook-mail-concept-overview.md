---
title: Übersicht über die Outlook-Mail-API
description: Outlook ist ein Messaging-Hub in Office 365. Es erlaubt ferner das Verwalten von Kontakten, das Planen von Besprechungen, das Suchen von Informationen über Benutzer in einer Organisation,
ms.openlocfilehash: a4ae3c00b578cf2f3bce7a23b73ec47dadc81cf8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092323"
---
# <a name="outlook-mail-api-overview"></a>Übersicht über die Outlook-Mail-API

Outlook ist ein Messaging-Hub in Office 365. Neben den Messagingfeatures bietet die Lösung Funktionen, mit denen Sie Ihre Kontakte verwalten, Besprechungen planen, Informationen zu Benutzern in Ihrem Unternehmen suchen, Onlineunterhaltungen initiieren, Dateien teilen und in Gruppen zusammenarbeiten können.

## <a name="why-integrate-with-outlook-mail"></a>Gründe für die Integration mit Outlook-Mail

### <a name="integrate-with-rich-features-and-reach-hundreds-of-millions-of-customers"></a>Integration von funktionsreichen Features und Zielgruppe von Hunderten Millionen Kunden

Eine Integration mit Outlook verschafft Ihnen Zugang zu dem weitreichenden Funktionsumfang, den Kunden so schätzen: einer konsistenten und intuitiven Oberfläche für E-Mails, [Kontakte](outlook-contacts-concept-overview.md) und [Kalender](outlook-calendar-concept-overview.md), die geräteunabhängig zur Verfügung steht – auf Mobilgeräten ebenso wie im Web und auf Desktop-PCs.

Möglich wird die Integration mit Outlook dank [Microsoft Graph](overview.md). Sie müssen Ihre App nur ein einziges Mal programmieren und können dann Hunderte Millionen Heimanwender sowie Unternehmenskunden im zweistelligen Millionenbereich erreichen, die Outlook als E-Mail-Client verwenden. Dabei können sich Ihre Apps auf E-Mail-Szenarien beschränken oder auch eine Vielzahl anderer Outlook-basierter und nicht Outlook-basierter Beziehungen, Ressourcen und Informationen nutzen. Auch von der Microsoft-Cloud unterstützte Szenarien lassen sich umsetzen.

### <a name="automate-message-organization-and-processing"></a>Automatisierung von Nachrichtenorganisation und -verarbeitung

Kunden schätzen, dass sie mit Outlook immer perfekt organisiert sein können. Microsoft Graph macht diese Features für App-Entwickler verfügbar. So können Sie Kundenworkflows erstellen, die die Suche optimieren und Effizienz sowie Produktivität steigern:

- Jeder Kunde organisiert seine Nachrichten auf seine eigene Art. Manche belassen sämtliche Nachrichten im Posteingang und suchen sie bei Bedarf, andere sortieren sie in Ordner ein. Alle schätzen den flexiblen und intuitiven Ansatz von Outlook, der sowohl eine flache als auch eine ordnerbasierte Organisationsstruktur unterstützt. Apps können Nachrichten bequem [filtern, suchen oder sortieren](query-parameters.md), wahlweise innerhalb bestimmter Ordner oder im gesamten Postfach des Benutzers.

- Outlook-Kategorien haben jeweils einen eigenen Namen und eine eigene Farbe. Mithilfe von Kategorien können Kunden Nachrichten taggen und so Ordnung und Auffindbarkeit verbessern. Apps können [auf die Hauptkategorienliste des Benutzers zugreifen und sie definieren](/graph/api/outlookuser-post-mastercategories?view=graph-rest-1.0). Besser noch: Eine solche Liste deckt alle Outlook-Nachrichten sowie Termine, Kontakte, Aufgaben und Gruppenbeiträge ab und eröffnet App-Entwicklern so kreative Szenarien. So kann ein Anbieter von Onlineschulungen beispielsweise einen Farbcode für E-Mails, Kurstermine und Folgearbeitsaufträge festlegen, für jeden Kurs, für den ein Benutzer registriert ist.

- App-Benutzer können darüber hinaus die Wichtigkeit einer Nachricht (oder eines Termins oder einer Aufgabe) ändern und Nachrichten zur Nachverfolgung kennzeichnen. (Die Kennzeichnungsfunktion in Microsoft Graph befindet sich derzeit in der [Preview-Phase](versioning-and-support.md#beta-version).)

- Die Regeln-API erlaubt eine Nachrichtenorganisation auf ganz neuem Niveau. Apps können [Posteingangsregeln](/graph/api/resources/messagerule?view=graph-rest-1.0) einrichten, sodass eingehende Nachrichten schnell verarbeitet werden und die Übersichtlichkeit des Posteingangs verbessert wird. Eine App kann Nachrichten beispielsweise automatisch in einen anderen Ordner verschieben, wenn die Betreffzeile bestimmte Schlüsselwörter enthält, sowie zwecks einfacherer Nachverfolgung Kategorien und Wichtigkeit zuweisen.

### <a name="write-smarter-apps-that-leverage-intelligence"></a>Intelligentere Apps mit Zugriff auf umfangreiche Informationen

Mit Microsoft Graph können Sie den Benutzern Ihrer App kontextbasiert Daten vorschlagen:

- Eine Integration von [Posteingang mit Relevanz](/graph/api/resources/manage-focused-inbox?view=graph-rest-1.0) und [@-Erwähnungen (Preview)](/graph/api/message-get?view=graph-rest-beta#request-2) erlaubt es Ihren Benutzern, zuerst die Nachrichten zu lesen und zu beantworten, die für sie am relevantesten sind.

- [E-Mail-Tipps](/graph/api/resources/mailtips?view=graph-rest-1.0) liefern während des Verfassens einer Nachricht nützliche Statusinformationen zum Empfänger (z. B. ob der Empfänger aktuell automatische Antworten sendet oder ob sein Postfach voll ist). E-Mail-Tipps können Apps informieren, wenn bestimmte Bedingungen erfüllt sind. So kann die jeweils effizientere Follow-up-Aktion gewählt werden.

- Über die [Personen-API](people-example.md) können Sie in Ihrer App interaktive Steuerelemente wie eine Personenauswahl bereitstellen. Die Personen-API kann dem Benutzer die für ihn relevantesten Personen vorschlagen, basierend auf seinen Kommunikations- und Zusammenarbeitsmustern sowie seinen geschäftlichen Beziehungen.

- Stellen Sie den Benutzern Ihrer App eine intelligente Dateiauswahl zur Verfügung, die ihnen beim Verfassen einer Nachricht ihre zuletzt genutzten Dateien als mögliche Anlagen anbietet. [Insights](/graph/api/resources/insights?view=graph-rest-beta) nutzt erweiterte Analysen, um dem Benutzer Dateien vorzuschlagen, die für ihn besonders relevant sind, die er kürzlich angesehen oder bearbeitet hat oder die mit ihm geteilt wurden.


### <a name="store-app-data-in-a-resource-or-resource-instance"></a>Speicherung von App-Daten in Ressourcen oder Ressourceninstanzen

Apps müssen ihre Daten oft in einem externen Datenspeicher speichern, was Mehraufwand durch Datenverwaltung und Datenzugriff nach sich zieht. Mit Microsoft Graph können Sie beim [Erstellen](/graph/api/user-post-messages?view=graph-rest-1.0#request-2) oder [Senden](/graph/api/user-sendmail?view=graph-rest-1.0#request-2) einer neuen Nachricht oder beim Antworten auf eine Nachricht App-Daten einfach als Internet-Nachrichtenköpfe einschließen.

Wenn Sie benutzerdefinierte Daten hinzufügen und später aktualisieren müssen, können Sie [die Daten in einzelnen Ressourceninstanzen speichern](extensibility-overview.md#open-extensions). Gegebenenfalls können Sie alternativ das Schema erweitern, benutzerdefinierte Eigenschaften hinzufügen und typisierte Daten in Microsoft Graph-Ressourcen speichern. Solche [Schemaerweiterungen](extensibility-overview.md#schema-extensions) können suchbar und teilbar gemacht werden.

## <a name="api-reference"></a>API-Referenz
Suchen Sie die API-Referenz für diesen Dienst?

- [Outlook-Mail-API in Microsoft Graph v1.0](/graph/api/resources/mail-api-overview?view=graph-rest-1.0)
- [Outlook-Mail-API in Microsoft Graph Beta](/graph/api/resources/mail-api-overview?view=graph-rest-beta)


## <a name="next-steps"></a>Nächste Schritte

- Wählen Sie im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0) Outlook-Mail-Beispielabfragen zum Testen aus. Klicken Sie in der Spalte links auf **Show more samples**. Aktivieren Sie über das Menü **Outlook-Mail**.
- Informieren Sie sich über folgende Themen:

  - [Erstellen und Senden von Nachrichten](outlook-create-send-messages.md)
  - Möglichkeiten zum [Organisieren von Nachrichten](outlook-organize-messages.md)
  - [Abrufen freigegebener Nachrichten](outlook-share-messages-folders.md)
  - [Abrufen von unveränderlichen Bezeichnern für Outlook-Ressourcen](outlook-immutable-id.md)

- Informieren Sie sich über die [Arbeit mit der Mail-API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) und die [Anwendungsfälle](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) der API in Microsoft Graph 1.0.


