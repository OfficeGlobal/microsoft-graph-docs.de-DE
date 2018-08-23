# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>Verwenden der Microsoft Graph-API zum Arbeiten mit Project Rome

[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) ist eine Initiative von Microsoft, um eine geräteübergreifende Plattform für Erfahrungen zu erstellen. Mit Project Rome kann eine App auf einem lokalen Client oder Dienst mit Apps und Diensten auf einem Remote-Host interagieren, wenn der Benutzer sich mit dem selben Microsoft-Konto anmeldet, das er benutzt, um sich auf dem Client-Gerät anzumelden. Dadurch können geräte- und plattformübergreifende Erfahrungen programmiert werden, bei denen die Benutzeraufgaben und nicht die Geräte im Vordergrund stehen.

Eine wichtige Komponente wird über Microsoft Graph zur Verfügung gestellt, um solche Erfahrungen zu ermöglichen: Aktivitäten.

## <a name="activities"></a>Aktivitäten

Aktivitäten in Microsoft Graph ermöglichen Ihnen, das Engagement von Benutzern in Ihren Apps unabhängig von Geräten und Plattformen voranzutreiben. Eine Aktivität ist die Einheit des Benutzerengagements und besteht aus drei Komponenten:

- Einem Deep-link
- Einer visuellen Darstellung
- Inhalts-Metadaten, die die Aktivität mithilfe des gemeinsamen [http://schema.org/](http://schema.org/) Vokabulars beschreibt

Wenn von einer Anwendung eine Sitzung erstellt wird, wird der Aktivität ein Verlaufselement hinzugefügt, das den Zeitraum des Benutzerengagements wiederspiegelt. Sobald ein Benutzer eine Aktivität wieder aufnimmt, wird der Aktivitä ein neues Verlaufselement hinzugefügt, um das Benutzerengagement weiter ansteigen zu lassen.

Wenn eine Anwendung ein Benutzeraktivitätsobjekt veröffentlich, wird dieses Objekt in einigen der neuen Benutzeroberflächen in Windows angezeigt, so etwa in Cortana-Benachrichtigungen und der Zeitachse. Sie können in Ihren Aktivitätsobjekten sowohl umfangreiche Metadaten (damit Aktivitäten genau im richtigen Kontext dargestellt werden) als auch umfangreiche visuelle Darstellungen (mit dem [Adaptive Card](http://adaptivecards.io/)-Markup) festlegen.

Mithilfe der folgenden Microsoft Graph-APIS können Sie Benutzeraktivitäten erstellen und abrufen:

- [Aktivität erstellen oder ersetzen](../api/projectrome_put_activity.md)
- [Aktivitäten abrufen](../api/projectrome_get_activities.md)
- [Aktuelle Aktivitäten abrufen](../api/projectrome_get_recent_activities.md)
- [Aktivität löschen](../api/projectrome_delete_activity.md)
- [Verlaufselement erstellen oder ersetzen](../api/projectrome_put_historyitem.md)
- [|||UNTRANSLATED_CONTENT_START|||Delete a history item|||UNTRANSLATED_CONTENT_END|||](../api/projectrome_delete_historyitem.md)