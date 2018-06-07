# <a name="microsoft-teams-teamwork-api-overview"></a>Überblick über die Teamarbeit-API in Microsoft Teams

Microsoft Teams ist der ultimative Hub für Zusammenarbeit und intelligente Kommunikation. Microsoft Teams, das auf den Stärken und der Größe von Office 365 aufbaut, bietet mit mehr als 120 Millionen von Benutzern chatbasierte Funktionen für Zusammenarbeit, Besprechungen, Anrufe sowie Enterprise-VoIP-Funktionen. 

## <a name="why-integrate-with-microsoft-teams"></a>Gründe für die Integration in Microsoft Teams

Dank der Integration in Microsoft Teams wird das Erstellen ihrer eigenen Dienste und Apps erleichtert. Außerdem können Sie Millionen von Unternehmenskunden erreichen und Menschen helfen, ihre Arbeit zusammen zu bewältigen. Sie können Microsoft Graph verwenden, um Teams, Kanäle, Nachrichten usw. zu erstellen und zu verwalten.

### <a name="use-microsoft-graph-in-any-kind-of-app"></a>Verwenden von Microsoft Graph in jeder Art von App

Microsoft Teams-Apps, die auf Microsoft Graph basieren, geben Arbeitsgruppen ein neues Tool an die Hand, um die Zusammenarbeit produktiver und interessanter zu gestalten. Mit Microsoft Teams können Arbeitsgruppenbenutzer Ressourcen freigeben, über Chats interagieren und Ereignisse im Teamkalender planen. Steigern Sie den Nutzen von Microsoft Teams, indem Sie Team-, Kanal- und Unterhaltungsautomatisierung über Apps hinzufügen, die auf der Microsoft Teams-API basieren.

Websites, Dienste und systemeigene Plattformanwendungen werden nicht innerhalb der Microsoft Teams-Benutzeroberfläche ausgeführt, können aber verwendet werden, um die Microsoft Teams-APIs aufzurufen, die Microsoft Teams-Automatisierungsszenarien ermöglichen.

**Typen von Apps, die für Microsoft Teams aktiviert sind**

![Rufen Sie die Microsoft Teams-API von Registerkarten, Bots, Websites und Diensten auf.](images/TeamsAppEndpoints.png)

Diese Zusammenarbeitstools umfassen Microsoft Graph-fähige Registerkarten oder Bot-Apps, die innerhalb von Microsoft Teams ausgeführt werden. Sie können Microsoft Graph auch außerhalb einer Microsoft Teams-App aufrufen, z. B. von einer Website oder einem Webdienst aus. Wenn Sie Ihre Website bereits für Microsoft Graph aktiviert haben, können Sie diese Arbeit für Microsoft Teams verwenden, indem Sie die [Microsoft Teams-Entwicklerplattform](https://docs.microsoft.com/de-DE/microsoftteams/platform/#pivot=home&panel=home-all) verwenden, um eine Registerkarten-App zu erstellen, die den vorhandenen Websitecode verwendet.

Wenn eine Microsoft Teams-Registerkarte oder Bot-App nicht ideal für Ihr Szenario ist, wählen Sie einen der folgenden App-Typen aus.

|App-Typ|Szenariobeschreibung|
|:-------|:-------------------|
|Registerkarten|Inhalte mit verbesserter Anzeige in Microsoft Teams.|
|Connectors|Für Posts optimierte Updates für Kanäle.|
|Aktionen fordernde Nachrichten|Fügen Sie Ihren Connector-Karten verbesserte Interaktion hinzu.|
|Websites|Inhalte mit verbesserter Anzeige in Ihren Webseiten.|
|Bots|Helfen Sie Benutzern, Aufgaben in Unterhaltungen zu erledigen.|
|Aktivitätsfeed|Benutzer über Feed-Benachrichtigungen einbeziehen.|
|Messaging-Erweiterungen|Zulassen, dass Benutzer erweiterte Karten in Unterhaltungen abfragen und freigeben.|
|Dienste|Verbessern Sie Ihre Clientanwendungen mit Microsoft Graph-Daten über Ihren Webdienst.|


### <a name="create-multiple-teams-and-channels"></a>Erstellen mehrerer Teams und Kanäle

Geben Sie Ihren Kunden die Möglichkeit, neue [Teams](../api-reference/beta/resources/team.md) und [Kanäle](../api-reference/beta/resources/channel.md) zu erstellen, die mit Ihrer App verknüpft sind. Vereinfachen Sie das Erstellen einer großen Anzahl von Teams und das Auffüllen dieser Teams mit Benutzern und Kanälen, indem Sie die Microsoft Teams-API verwenden.

### <a name="automate-team-lifecycles"></a>Automatisieren von Teamlebenszyklen

Verwenden Sie Microsoft Graph, um ein neues virtuelles Team zu erstellen, wenn sich ein neues Unternehmensproblem ergibt, [füllen Sie das Team](../api-reference/v1.0/api/group_post_members.md) mit den richtigen Personen, und konfigurieren Sie das Team mit Kanälen. Um eine Teamkanalbesprechung zu dem neuen Unternehmensproblem zu starten, können Sie den Kanal mit einem neuen Unterhaltungsthread anlegen, um eine Willkommensnachricht für neue Teammitglieder zu veröffentlichen. Wenn Sie das neue Team zusammenbringen möchten, um das Unternehmensproblem zu besprechen, fügen Sie dem Teamkalender ein neues Ereignis hinzu, und laden Sie dann die Teammitglieder zu dem Ereignis ein.

Wenn das Unternehmensproblem gelöst wurde und Sie das virtuelle Team nicht mehr benötigen, verwenden Sie die Microsoft Teams-API, um das Team aufzulösen. Wenn Sie die maximale Dauer des virtuellen Teams bei der Erstellung kennen, legen Sie eine [Ablaufrichtlinie für die Office 365-Gruppe](https://support.office.com/en-us/article/office-365-group-expiration-policy-8d253fe5-0e09-4b3c-8b5e-f48def064733?ui=en-US&rs=en-US&ad=US) für das Team fest, durch die das Team gemäß der Richtlinie automatisch entfernt wird.

## <a name="next-steps"></a>Nächste Schritte

- Erfahren Sie, wie Sie [die Microsoft Teams-API verwenden](../api-reference/beta/resources/teams_api_overview.md).
- Führen Sie einen Drilldown für die Methoden, Eigenschaften und Beziehungen der Ressourcen [team](../api-reference/beta/resources/team.md), [channel](../api-reference/beta/resources/channel.md) und [group](.../api-reference/v1.0/resources/group.md) aus.
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/de-DE/graph/graph-explorer) aus.
- Erfahren Sie mehr über das [Microsoft Teams-Programmiermodell](https://docs.microsoft.com/de-DE/microsoftteams/platform/concepts/concepts-overview).
- Schnelleinstieg mit [Beispielcode](https://github.com/OfficeDev/microsoft-teams-sample-graph).


