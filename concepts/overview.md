# <a name="overview-of-microsoft-graph"></a>Übersicht über Microsoft Graph

Microsoft Graph ist das Gateway zu Daten und Intelligence in Microsoft 365. Microsoft Graph bietet ein einheitliches Programmiermodell, das Sie verwenden können, um die enorme Menge von Daten in Office 365, Enterprise Mobility + Security und Windows 10 zu nutzen. 

Mit der Microsoft Graph-API können Sie Apps für Organisationen und Heimanwender erstellen, die mit den Daten von Millionen von Benutzern interagieren. Mit Microsoft Graph können Sie eine Verbindung mit einer Vielzahl von Ressourcen, Beziehungen und Intelligence über einen einzelnen Endpunkt herstellen: `https://graph.microsoft.com`.

## <a name="whats-in-the-graph"></a>Was ist im Diagramm zu sehen?
Microsoft Graph bietet APIs für:

- Azure Active Directory
- Office 365-Dienste: SharePoint, OneDrive, Outlook/Exchange, Microsoft Teams, OneNote, Planner und Excel
- Enterprise Mobility + Security-Dienste: Identity Manager, Intune, Advanced Threat Analytics und Advanced Threat Protection.
- Windows 10-Dienste: Aktivitäten und Geräte
- Schulung und Weiterbildung

Weitere Informationen finden Sie unter [Wesentliche Dienste und Features in Microsoft Graph](../concepts/overview-major-services.md).

Microsoft Graph verbindet alle Ressourcen in diesen Diensten durch Beziehungen. Beispielsweise kann ein Benutzer mit einer Gruppe über eine [memberOf](../api-reference/v1.0/api/user_list_memberof.md)-Beziehung und mit einem anderen Benutzer über eine [manager](../api-reference/v1.0/api/user_list_manager.md)-Beziehung verbunden sein. Ihre App kann diese Beziehungen durchlaufen, um über die API auf diese verbundenen Ressourcen zuzugreifen und Aktionen für sie auszuführen.

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

>**Hinweis:** Wenn Sie die Microsoft Graph-API verwenden, stimmen Sie den [Microsoft Graph-Nutzungsbedingungen](https://developer.microsoft.com/en-us/graph/docs/misc/terms-of-use) und den [Microsoft-Datenschutzbestimmungen](https://go.microsoft.com/fwlink/?LinkId=521839) zu.

### <a name="popular-requests"></a>Beliebte Anforderungen

Sehen Sie sich diese allgemeinen Szenarios für das Arbeiten mit der Microsoft Graph-API an. Über die Links gelangen Sie zum [Graph-Tester](https://developer.microsoft.com/en-us/graph/graph-explorer).

| **Vorgang** | **URL** |
|:--------------------------|:----------------------------------------|
|   Eigenes Profil mit GET abrufen |    [`https://graph.microsoft.com/v1.0/me`](https://developer.microsoft.com/graph/graph-explorer/?request=me&version=v1.0) |
|   Eigene Dateien mit GET abrufen | [`https://graph.microsoft.com/v1.0/me/drive/root/children`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fdrive%2Froot%2Fchildren&version=v1.0) |
|   Eigenes Foto mit GET abrufen	 | [`https://graph.microsoft.com/v1.0/me/photo/$value`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fphoto%2F%24value&version=v1.0) |
|   Eigene E-Mail mit GET abrufen |   [`https://graph.microsoft.com/v1.0/me/messages`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0) |
|   Eigene E-Mails mit Wichtigkeit „Hoch“ mit GET abrufen | [`https://graph.microsoft.com/v1.0/me/messages?$filter=importance%20eq%20'high'`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages%3F%24filter%3Dimportance%2520eq%2520'high'&version=v1.0) |
|   Eigene Kalenderereignisse mit GET abrufen |    [`https://graph.microsoft.com/v1.0/me/events`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fevents&version=v1.0) |
|   Eigenen Vorgesetzten mit GET abrufen  | [`https://graph.microsoft.com/v1.0/me/manager`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmanager&version=v1.0) |
|   Letzten Benutzer zum Ändern der Datei „foo.txt“ mit GET abrufen |  [`https://graph.microsoft.com/v1.0/me/drive/root/children/foo.txt/lastModifiedByUser`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fdrive%2Froot%2Fchildren%2Ffoo.txt%2FlastModifiedByUser&version=v1.0) |
|   Office 365-Gruppen, bei denen ich Mitglied bin, mit GET abrufen| [`https://graph.microsoft.com/v1.0/me/memberOf/$/microsoft.graph.group?$filter=groupTypes/any(a:a%20eq%20'unified')`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2FmemberOf%2F%24%2Fmicrosoft.graph.group%3F%24filter%3DgroupTypes%2Fany(a%3Aa%2520eq%2520'unified')&version=v1.0) |
|   Benutzer in meiner Organisation mit GET abrufen     | [`https://graph.microsoft.com/v1.0/users`](https://developer.microsoft.com/graph/graph-explorer/?request=users&version=v1.0) |
|   Gruppen in meiner Organisation mit GET abrufen | [`https://graph.microsoft.com/v1.0/groups`](https://developer.microsoft.com/graph/graph-explorer/?request=groups&version=v1.0) |
|   Verwandte Personen mit GET abrufen    | [`https://graph.microsoft.com/v1.0/me/people`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fpeople&version=beta)  |
|   Populäre Elemente mit GET abrufen |  [`https://graph.microsoft.com/beta/me/insights/trending`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Finsights%2Ftrending&version=beta) |
|   Eigene Notizen mit GET abrufen |  [`https://graph.microsoft.com/v1.0/me/onenote/notebooks`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fonenote%2Fnotebooks&version=beta) |

## <a name="next-steps"></a>Nächste Schritte

- Sehen Sie sich [ausgewählte Szenarios](../concepts/featured_scenarios.md) an.
- Starten Sie eine Beispielanforderung im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer).
- Nutzen Sie den [Schnellstart](https://developer.microsoft.com/graph/quick-start), um eine sofort ausführbare Beispiel-App einzurichten.
- Sehen Sie im Inhaltsverzeichnis unter **Lernen** nach, um mehr über die Dienste und Features zu erfahren, die Sie in diesen Szenarios verwenden können. 
- Erfahren Sie, wie Sie [ein Authentifizierungstoken](../concepts/auth_overview.md) in Ihrer App erhalten.
- Beginnen Sie damit, die [API zu verwenden](../concepts/use_the_api.md).

## <a name="feedback"></a>Feedback?

Ihr Feedback ist uns wichtig. Nehmen Sie auf [Stack Overflow](http://stackoverflow.com/questions/tagged/office365+or+microsoftgraph) Kontakt mit uns auf. Taggen Sie Ihre Fragen mit {MicrosoftGraph}.

