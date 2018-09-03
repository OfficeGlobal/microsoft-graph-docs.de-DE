# <a name="outlook-calendar-api-overview"></a>Übersicht über die Outlook-Kalender-API

Der Outlook-Kalender ist Teil des Messaging-Hubs von Outlook in Office 365, mit dem Sie ebenfalls Ihre E-Mails und Kontakte verwalten, Informationen zu Benutzern in Ihrem Unternehmen suchen, Onlineunterhaltungen initiieren, Dateien teilen und in Gruppen zusammenarbeiten können.

## <a name="why-integrate-with-outlook-calendar"></a>Vorteile der Integration mit dem Outlook-Kalender

### <a name="reach-hundreds-of-millions-of-customers-and-build-rich-scenarios"></a>Erreichen Sie mehreren hundert Millionen Kunden, und erstellen Sie umfassende Szenarien.

Viele Millionen von Kunden verwenden den Outlook-Kalender als Teil eines integrierten Hubs, mit dem sie effektiv kommunizieren und produktiv arbeiten können. Sie können Besprechungen planen, E-Mails verwalten, Informationen zu Kontakten und anderen Benutzern suchen sowie Unterhalten oder Online-Meetings initiieren, und das alles an einem Ort, entweder im Internet, auf Mobilgeräten oder vom Desktop aus. Microsoft Graph verknüpft Apps nicht nur mit den Kalender-, Mail und Kontaktdaten dieser Kunden, sondern ermöglicht Apps auch die [Integration mit den besten Funktionen von Microsoft 365](overview-major-services.md) und unterstützt eine breite Palette von Szenarien, mit denen sich die Produktivität steigern und die Zusammenarbeit verbessern lassen.

### <a name="automate-appointment-organization-and-calendaring"></a>Automatisieren der Terminorganisation und Kalendereinträge

Kunden schätzen die Möglichkeiten in Outlook zum Organisieren ihrer Zeit für Arbeit, Familie und eigene Aktivitäten. Die Microsoft Graph-REST-API hält sich eng an die Benutzererfahrung und ermöglicht es, dass Apps genauso einfach Ereignisse erstellen, verwalten und darauf reagieren können:

- In Outlook können Kunden einzelnen Kalender für Arbeit, Familie und andere Zwecke erstellen und diese dann als Kalendergruppen organisieren. Sie können die kostenlosen **Geburtstags**- und **Feiertagskalender** aktivieren, damit sie an die Geburtstage ihrer Kontakte und Feiertage erinnert werden. Sie können Kalender hinzufügen, die ihren Interessen entsprechen, z. B. Kalender für Sportmannschaften und TV-Programme. Kunden können Kalender auswählen und sie überlagern, sodass ihre Termine in derselben Ansicht angezeigt werden. Mit der Kalender-API kann Ihre App [Kalender](../api-reference/v1.0/resources/calendar.md) auf ähnliche Weise in [Kalendergruppen](../api-reference/v1.0/resources/calendargroup.md) organisieren und ebenfalls mit anderen Kalendern von Interesse interagieren, genau wie jeder andere **Kalender** im Postfach des Benutzers. 

- Kunden mit Outlook können Kategorien einheitlich auf Ereignisse, Nachrichten, Kontakte, Aufgaben und Gruppenbeiträge anwenden, um die Organisation und Ermittlung zu verbessern. Mit der Kalender-API können Sie außerdem auf die [Masterliste von Kategorien eines Benutzers zugreifen und diese definieren](../api-reference/v1.0/api/outlookuser_post_mastercategories.md), sodass Sie weiteren kreative Szenarien erstellen können. So kann zum Beispiel ein Sportverein einen Wettkampf organisieren und eine App anbieten, in der E-Mail und Events für die einzelnen Sportarten jeweils unterschiedlich farblich markiert werden. Wenn kurzfristige Änderungen auftreten, sich z. B. die Wettkampfzeiten unvorhergesehen ändern, kann die App auch die **Wichtig**-Eigenschaft dieser Events und E-Mails festlegen, um Kunden darüber zu benachrichtigen.

- Im Kalenderordner haben Sie die Möglichkeit zum [Erstellen](../api-reference/v1.0/api/user_post_events.md) und [Aktualisieren](../api-reference/v1.0/api/event_update.md) von Einzelinstanz-[Events](../api-reference/v1.0/resources/event.md), oder [Sie können wiederkehrende Events planen und pflegen](outlook-schedule-recurring-events.md). Sie haben die Möglichkeit, dass Kunden auf [Besprechungsanfragen](../api-reference/v1.0/resources/eventmessage.md) antworten sowie zum [erneuten Erinnern](../api-reference/v1.0/api/event_snoozereminder.md) oder [Schließen](../api-reference/v1.0/api/event_dismissreminder.md) von [Erinnerungen](../api-reference/v1.0/resources/reminder.md) mit der zugehörigen **Ereignis**-Navigationseigenschaft.


### <a name="help-customers-stay-synchronized-and-navigate-their-day"></a>Helfen Sie Ihren Kunden, auf dem neuesten Stand zu bleiben und ihren Tag im Blick haben

Die Kalender-API unterstützt Ihre Kunden dabei, ihren Tag im Blick zu behalten und ihre Produktivität zu steigern:

<!-- change link to notifications to the concept topic once it's created. In general, try staying in the conceptual level in these overview topics, if conceptual topics are available for the link destination. 
-->

- Sie können den lokalen App-Speicher synchronisieren, indem Sie [Änderungsbenachrichtigungen](../api-reference/v1.0/resources/webhooks.md) abonnieren und [Ereignisänderungen](delta_query_events.md) im Kalender eines Benutzers nachverfolgen.
- Sie können die Agenda des Benutzers basierend auf einer einfachen [Erinnerungsansicht](../api-reference/v1.0/api/user_reminderview.md) anzeigen. 
- Sie können ermöglichen, dass der Benutzer einer Besprechung bequem online [zusagt](../api-reference/v1.0/api/event_accept.md) und über die **webLink**-Eigenschaft, mit der die Besprechnung in Outlook im Web geöffnet wird, online daran teilnimmt.
- Benutzer können einer Besprechung von unterwegs auch [mit Vorbehalt zusagen](../api-reference/v1.0/api/event_tentativelyaccept.md) oder sie [ablehnen](../api-reference/v1.0/api/event_decline.md).

### <a name="enhance-collaboration"></a>Verbessern der Zusammenarbeit

- In Outlook können Kunden Kalender für andere freigeben und ihnen die Berechtigung zum Lesen, Schreiben oder Löschen von Kalenderinhalten gewähren. Alternativ können sie einen Kalender auch an eine andere Person delegieren, damit diese in ihrem Namen auf Besprechungsanfragen antworten kann. Obwohl Sie die Freigabe oder Delegierung einer Aktion im Namen eines anderen Benutzers nicht programmgesteuert initiieren können, können Sie einen Eigenschaftensatz verwenden, um den Freigabestatus zu prüfen und Szenarien zu freigegebenen oder delegierten Kalendern zu aktivieren: **CanEdit**, **CanShare**, **CanViewPrivateItems**, **IsShared** und **IsSharedWithMe**.
- Mit der Kalender-API können Sie Kalenderelemente des angemeldeten Benutzers oder von Benutzern, die ihre Kalender für den angemeldeten Benutzer freigegeben oder an ihn delegiert haben, abrufen. Wenn Garth beispielsweise einen Kalenderordner für John freigegeben hat oder wenn Garth John Zugriff erteilt hat, so würden Sie über [delegierte Berechtigungen](permissions_reference.md#delegated-permissions-application-permissions-and-effective-permissions) von John Lesezugriff auf den freigegebenen Kalender und auch auf die Inhalte erhalten.
- ** Office 365-Gruppen erleichtert den Gruppenmitgliedern die Zusammenarbeit und den Zugriff auf Gruppenunterhaltung und Kalender direkt in Outlook. Abgesehen von einigen kleineren Unterschieden zwischen Gruppenkalendern und Benutzerkalendern, ermöglicht die Kalender-API Ihnen die Interaktion mit Gruppenkalendern auf die gleiche Weise wie mit Benutzerkalendern. Weitere Informationen finden Sie in der [Kalenderressource](../api-reference/v1.0/resources/calendar.md).

** Kennzeichnet Features, die speziell für Outlook-Kalender in Geschäfts-, Schul- oder Unikonten gelten.


### <a name="schedule-smart"></a>Intelligente Planung

Outlook und die Kalender-API bieten zahlreiche intelligente Funktionen zum Planen von Ereignissen:

- Mit den App-Einstellungen für Outlook-Kalender können Kunden das automatische Hinzufügen von Ereignissen aus E-Mails aktivieren, wie z. B. Flug-, Hotel- oder Restaurantreservierungen und Rechnungen. Nachdem sie hinzugefügt wurden, können Sie diese Ereignisse genau wie jedes andere [Ereignis](../api-reference/v1.0/resources/event.md)-Objekte im Postfach des Benutzers verwenden und kreative Szenarien für diese Outlook-Funktion erstellen.
- ** In Outlook ist das Buchen eines Besprechungsraums so einfach wie das Hinzufügen eines Teilnehmers zum **Ereignis**. Die Kalender-API stellt einen Besprechungsraum als ein [emailAddress](../api-reference/v1.0/resources/emailaddress.md)-Objekt dar. Sie können [Räume abrufen (Vorschau)](../api-reference/beta/api/user_findrooms.md) und [Raumlisten abrufen (Vorschau)](../api-reference/beta/api/user_findroomlists.md), die in einem Mandanten verfügbar sind. Um eine Besprechung in einem bestimmten Raum zu organisieren, weisen Sie sie der **location**-Eigenschaft des **Ereignisses** zu.
- ** Sie können [die Frei/Gebucht-Informationen für Benutzer und Ressourcen (Vorschau)](outlook-get-free-busy-schedule.md) für einen bestimmten Zeitraum nachschlagen. Diese Daten können Sie dann auf verschiedene Szenarien einschließlich Ressourcenplanung und Ereignisplanung anwenden. 
- ** Wenn Ihr Szenario das Planen von Besprechungen zu einem optimalen Zeitpunkt beinhaltet, können Sie [mithilfe von FindMeetingTimes die möglichen Zeiten oder Besprechungsorte identifizieren](findmeetingtimes_example.md). Die Funktion [findMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) berücksichtigt den Frei-/Gebucht-Status der Teilnehmer sowie die bevorzugten Räume, Zeiten und anderen angegebenen Einschränkungen. Wenn beim ersten Versuch keine gemeinsame Besprechungszeit zurückgegeben wird, überprüfen Sie den Grund, passen Sie Ihre Kriterien an, und rufen Sie **FindMeetingTimes** erneut auf.


### <a name="teleconference-across-multiple-locations-and-time-zones"></a>Telefonkonferenz an mehreren Standorten und in verschiedenen Zeitzonen

Durch die Globalisierung nehmen an geschäftlichen Besprechungen heutzutage auch häufig Teilnehmer an verschiedenen Orten und in unterschiedlichen Zeitzonen teil. Nachfolgend erfahren Sie, wie Sie Besprechungen dieser Art mit der Kalender-API verwalten können:

- Kunden können beispielsweise in Outlook eine Besprechung organisieren und Teilnehmer aus einem Konferenzraum in Seattle, in einem Café in Paris und im Heimbüro in China einbeziehen. Die **locations**-Eigenschaft des Ereignisses, die eine Sammlung von [location](../api-reference/v1.0/resources/location.md)-Objekten ist, kann programmgesteuert diese Detailebene in **displayName** und **locationType** für das jeweilige **location**-Objekt widergeben. Sehen Sie sich das [Beispiel](../api-reference/v1.0/api/event_get.md#request-2) an.
- Outlook bietet Kunden die Flexibilität, Ereignisse zu organisieren und eine Zeitzone für die Start- und Endzeiten des Ereignisses anzugeben. Um diese Flexibilität zu unterstützen, gibt die Kalender-API standardmäßig die **Start**- und **End**-Zeiten eines **Ereignisses** in UTC an und stellt die Eigenschaften **originalStartTimeZone** und **originalEndTimeZone** bereit, um so die beim Erstellen des Ereignisses verwendeten Zeitzonen anzugeben. 
- Alternativ können Sie den `Prefer: outlook.timezone="{time zone name}"`-Header angeben, damit ein GET-Ereignisvorgang **Start** und **Ende** in der angegebenen Zeitzone zurückgibt. Der Name der Zeitzone kann einer der von Windows unterstützten Namen sein, sowie einer der in dieser [Liste](../api-reference/v1.0/resources/datetimetimezone.md) aufgeführten Namen. Sehen Sie sich ein [Beispiel](../api-reference/v1.0/api/event_get.md#request-1) für die Verwendung des `Prefer`-Headers an.


### <a name="take-advantage-of-social-intelligence-and-other-developer-conveniences-in-microsoft-graph"></a>Nutzen der Vorteile von Informationen aus sozialen Netzwerken und andere Vorteile für Entwickler in Microsoft Graph

Mit der [Personen-API](people_example.md) in Microsoft Graph können Sie eine Verbindung zu [Personendaten](../api-reference/v1.0/resources/person.md) herstellen, die auf den Kommunikations- und Zusammenarbeitsmustern eines Benutzer und den Geschäftsbeziehungen basieren. Sie können z. B. Steuerelemente wie eine Personenauswahl implementieren und Personen vorschlagen, die für den Benutzer relevant sind, wenn Sie Besprechungen im Namen des Benutzers organisieren.

Verringern Sie den Aufwand, indem Sie die App-Daten in externen Datenspeichern speichern und verwalten. Mit Microsoft Graph können Sie benutzerdefinierte App-Daten als [offene Erweiterungen](extensibility_overview.md#open-extensions) in einer einzelnen Ressourceninstanz speichern. Wenn die Daten eingegeben werden müssen oder das typisierte Schema freigegeben werden soll, können Sie benutzerdefinierte App-Daten in [Schemaerweiterungen](extensibility_overview.md#schema-extensions) speichern.


## <a name="next-steps"></a>Nächste Schritte

- Wählen Sie Beispielabfragen für Kalender im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fevents&version=v1.0) aus, und probieren Sie sie aus.
- Informieren Sie sich über folgende Themen:
  - [Suchen nach möglichen Besprechungszeiten im Outlook-Kalender](findmeetingtimes_example.md)
  - [Planen wiederkehrender Termine als wiederkehrende Ereignisse in Outlook](outlook-schedule-recurring-events.md)
- Sehen Sie sich die Referenz zur Outlook-[Kalender-API](../api-reference/v1.0/resources/calendar.md) an.

<!-- Replace the last item with the calendar API overview when it's published.
-->
