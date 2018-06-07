# <a name="microsoft-graph-reports-api-overview"></a>Übersicht über die Berichts-API von Microsoft Graph

Anhand von Nutzungsberichten im Microsoft 365-Administrationscenter können Administratoren die Nutzung von Office 365-Diensten in ihrem Unternehmen besser verstehen. Mit der Berichts-API in Microsoft Graph haben Sie die Möglichkeit der Integration mit Office 365-Nutzungsberichten.

## <a name="why-use-the-reports-api"></a>Warum sollte ich die Berichts-API verwenden?

### <a name="integrate-office-365-usage-reporting-into-your-organizations-existing-reporting-solution"></a>Integrieren von Office 365-Nutzungsberichten in die bestehende Berichterstellungslösung Ihres Unternehmens
Viele Unternehmen verfügen über bestehende Berichterstellungslösungen, die eine Anwendung oder ein Webportal zur Berichtserstellung nutzen. Mit der Berichts-API können Sie Office 365-Nutzungsdaten in die bestehende Berichterstellungslösung Ihres Unternehmens integrieren, sodass sich alle IT-Dienstberichte an einem zentralen Ort befinden.  

### <a name="retain-usage-reports-for-historical-analysis"></a>Aufbewahren von Nutzungsberichten für die Verlaufsanalyse
Mit der Berichts-API können Sie die Daten aus allen Nutzungsberichten abrufen, einschließlich Zusammenfassungen auf Unternehmensebene nach Dienst- und Entitätsebene (Benutzer, Sites, Konten) für die letzten 7/30/90/180 Tage sowie tägliche Aggregate. Auf diese Weise können Sie ältere Nutzungsdaten so lange wie erforderlich beibehalten.

## <a name="what-data-can-i-access-by-using-the-reports-api"></a>Auf welche Daten kann ich mit der Berichts-API zugreifen?

Mit der Berichts-API können Sie auf die in der folgenden Tabelle aufgeführten Datensätze zugreifen.

|Office 365-App|Datensatz|
|:--------|:--------|
|Microsoft Teams|[Gerätenutzung](../api-reference/v1.0/resources/microsoft_teams_device_usage_reports.md)<br/>|[Benutzeraktivität](../api-reference/v1.0/resources/microsoft_teams_user_activity_reports.md)|
|Office 365 (allgemein) |[Aktivierungen](../api-reference/v1.0/resources/office_365_activations_reports.md)<br/>[Aktive Benutzer](../api-reference/v1.0/resources/office_365_active_users_reports.md)<br/>[Gruppenaktivität](../api-reference/v1.0/resources/office_365_groups_activity_reports.md)|
|OneDrive |[Aktivität](../api-reference/v1.0/resources/onedrive_activity_reports.md)<br/>[Nutzung](../api-reference/v1.0/resources/onedrive_usage_reports.md)|
|Outlook|[Aktivität](../api-reference/v1.0/resources/email_activity_reports.md)<br/>[App-Nutzung](../api-reference/v1.0/resources/email_app_usage_reports.md)<br/>[Postfachnutzung](../api-reference/v1.0/resources/mailbox_usage_reports.md)|
|SharePoint |[Aktivität](../api-reference/v1.0/resources/sharepoint_activity_reports.md)<br/>[Websiteverwendung](../api-reference/v1.0/resources/sharepoint_site_usage_reports.md)|
|Skype for Business |[Aktivität](../api-reference/v1.0/resources/skype_for_business_activity_reports.md)<br/>[Gerätenutzung](../api-reference/v1.0/resources/skype_for_business_device_usage_reports.md)<br/>[Gerätenutzung](../api-reference/v1.0/resources/skype_for_business_device_usage_reports.md)<br/>[Teilnehmeraktivität](../api-reference/v1.0/resources/skype_for_business_participant_activity_reports.md)<br/>[Peer-to-Peer-Aktivität](../api-reference/v1.0/resources/skype_for_business_peer_to_peer_activity.md)|
|Yammer |[Aktivität](../api-reference/v1.0/resources/yammer_activity_reports.md)<br/>[Gerätenutzung](../api-reference/v1.0/resources/yammer_device_usage_reports.md)<br/>[Gruppenaktivität](../api-reference/v1.0/resources/yammer_groups_activity_reports.md)|

## <a name="next-steps"></a>Nächste Schritte

* Sehen Sie sich die APIs im [Graph-Tester](https://developer.microsoft.com/de-DE/graph/graph-explorer) an.
* Weitere Informationen über die [Verwendung der REST-API für Berichte](../api-reference/v1.0/resources/report.md).
