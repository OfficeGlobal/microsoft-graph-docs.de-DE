# <a name="overview-of-microsoft-graph"></a>Übersicht über Microsoft Graph

Die Microsoft Graph-API können Sie für die Interaktion mit den Daten von Millionen von Benutzern in der Microsoft-Cloud verwenden. Verwenden Sie Microsoft Graph zum Erstellen von Apps für Organisationen und Heimanwender, die über einen einzelnen Endpunkt Zugriff auf eine Vielzahl von Ressourcen, Beziehungen und Daten haben möchten: `https://graph.microsoft.com`.

## <a name="whats-in-the-graph"></a>Was ist im Diagramm zu sehen?

Microsoft Graph besteht aus Ressourcen, die durch Beziehungen verbunden sind. Beispielsweise kann ein Benutzer mit einer Gruppe über eine [memberOf](../api-reference/v1.0/api/user_list_memberof.md)-Beziehung und mit einem anderen Benutzer über eine [manager](../api-reference/v1.0/api/user_list_manager.md)-Beziehung verbunden sein. Ihre App kann diese Beziehungen durchlaufen, um über die API auf diese verbundenen Ressourcen zuzugreifen und Aktionen für sie auszuführen.

Mit Microsoft Graph können Sie außerdem wertvolle Erkenntnisse aus den Daten gewinnen. Sie können z. B. herausfinden, welche Dateien eines bestimmten Benutzers [besonders beliebt](../api-reference/beta/resources/insights_trending.md) sind oder mit welchen [Personen](../api-reference/beta/api/user_list_people.md) er eng zusammenarbeitet.

Entdecken Sie die Möglichkeiten der Beziehungen innerhalb von Microsoft Graph.

![Ein Bild mit den primären Ressourcen und Beziehungen, die Teil des Diagramms sind](images/microsoft_graph.png)

## <a name="what-can-you-do-with-microsoft-graph"></a>Was können Sie mit Microsoft Graph tun? 

Sie können Microsoft Graph verwenden, um Benutzer zielgerichtet mit für sie relevanten Informationen zu versorgen und ihnen so zu helfen, produktiver zu arbeiten. Stellen Sie sich eine App vor, die ...

- auf Ihr nächstes Meeting schaut und Ihnen hilft, sich darauf vorzubereiten, indem sie Profilinformationen für Teilnehmer, einschließlich ihrer Jobtitel und deren Arbeit, sowie Informationen über die neuesten Dokumente und Projekte, an denen sie arbeiten, bereitstellt.
- Ihren Kalender überprüft und die beste Zeit für Ihre nächstes Teammeeting vorschlägt.
- die neueste Verkaufsprognose aus einer Excel-Datei in Ihrem OneDrive abruft, damit Sie sie in Echtzeit aktualisieren können - auf Ihrem Mobiltelefon.
- Änderungen in Ihrem Kalender abonniert, Ihnen eine Warnung sendet, wenn Sie zu viel Zeit in Meetings verbringen, und Vorschläge macht, welche Meetings sie getrost verpassen oder delegieren können, abhängig von den anderen Teilnehmern und davon, wie eng sie mit diesen zusammenarbeiten.
- Ihnen hilft, persönliche und geschäftliche Informationen auf Ihrem Mobiltelefon zu sortieren. Beispielsweise sollten Bilder in Ihrem persönlichen OneDrive gespeichert werden und Geschäftsbelege in Ihrem OneDrive for Business.

Mit der Microsoft Graph-API können Sie all dies und mehr erledigen.

## <a name="next-steps"></a>Nächste Schritte

- Sehen Sie sich [ausgewählte Szenarios](../concepts/featured_scenarios.md) an.
- Starten Sie eine Beispielanforderung im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer).
- Nutzen Sie den [Schnellstart](https://developer.microsoft.com/graph/quick-start), um eine sofort ausführbare Beispiel-App einzurichten.
- Erfahren Sie, wie Sie [ein Authentifizierungstoken](../concepts/auth_overview.md) in Ihrer App erhalten.
- Beginnen Sie damit, die [API zu verwenden](../concepts/use_the_api.md).

## <a name="feedback"></a>Feedback?

Ihr Feedback ist uns wichtig. Nehmen Sie auf [Stack Overflow](http://stackoverflow.com/questions/tagged/office365+or+microsoftgraph) Kontakt mit uns auf. Taggen Sie Ihre Fragen mit {MicrosoftGraph}.

