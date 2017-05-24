# <a name="featured-scenarios-for-microsoft-graph"></a>Ausgewählte Szenarios für Microsoft Graph

Sehen Sie sich einige allgemeine und ausgewählte Szenarios für das Arbeiten mit der Microsoft Graph-API an. Erkunden Sie die Themen in diesem Abschnitt, und probieren Sie einige der in der folgenden Tabelle aufgeführten beliebten Anforderungen aus. Über die Links gelangen Sie zu unserem [Graph-Tester](https://developer.microsoft.com/en-us/graph/graph-explorer).


## <a name="popular-requests"></a>Beliebte Anforderungen
| **Vorgang**    | **URL** |
|:--------------------------|:----------------------------------------|
|   Eigenes Profil mit GET abrufen |    [`https://graph.microsoft.com/v1.0/me`](https://developer.microsoft.com/graph/graph-explorer/?request=me&version=v1.0) |
|   Eigene Dateien mit GET abrufen | [`https://graph.microsoft.com/v1.0/me/drive/root/children`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fdrive%2Froot%2Fchildren&version=v1.0) |
|   Eigenes Foto mit GET abrufen	 | [`https://graph.microsoft.com/v1.0/me/photo/$value`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fphoto%2F%24value&version=v1.0) |
|   Eigene E-Mail mit GET abrufen |    [`https://graph.microsoft.com/v1.0/me/messages`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0) |
|   Eigene E-Mails mit Wichtigkeit „Hoch“ mit GET abrufen | [`https://graph.microsoft.com/v1.0/me/messages?$filter=importance%20eq%20'high'`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages%3F%24filter%3Dimportance%2520eq%2520'high'&version=v1.0) |
|   Eigene Kalenderereignisse mit GET abrufen |    [`https://graph.microsoft.com/v1.0/me/events`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fevents&version=v1.0) |
|   Eigenen Vorgesetzten mit GET abrufen    | [`https://graph.microsoft.com/v1.0/me/manager`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmanager&version=v1.0) |
|   Letzten Benutzer zum Ändern der Datei „foo.txt“ mit GET abrufen |    [`https://graph.microsoft.com/v1.0/me/drive/root/children/foo.txt/lastModifiedByUser`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fdrive%2Froot%2Fchildren%2Ffoo.txt%2FlastModifiedByUser&version=v1.0) |
|   Office 365-Gruppen, bei denen ich Mitglied bin, mit GET abrufen|    [`https://graph.microsoft.com/v1.0/me/memberOf/$/microsoft.graph.group?$filter=groupTypes/any(a:a%20eq%20'unified')`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2FmemberOf%2F%24%2Fmicrosoft.graph.group%3F%24filter%3DgroupTypes%2Fany(a%3Aa%2520eq%2520'unified')&version=v1.0) |
|   Benutzer in meiner Organisation mit GET abrufen     | [`https://graph.microsoft.com/v1.0/users`](https://developer.microsoft.com/graph/graph-explorer/?request=users&version=v1.0) |
|   Gruppen in meiner Organisation mit GET abrufen |    [`https://graph.microsoft.com/v1.0/groups`](https://developer.microsoft.com/graph/graph-explorer/?request=groups&version=v1.0) |
|   Verwandte Personen mit GET abrufen    | [`https://graph.microsoft.com/beta/me/people`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fpeople&version=beta)  |
|   Populäre Elemente mit GET abrufen |    [`https://graph.microsoft.com/beta/me/insights/trending`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Finsights%2Ftrending&version=beta) |
|   Eigene Notizen mit GET abrufen |    [`https://graph.microsoft.com/beta/me/onenote/notebooks`](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fonenote%2Fnotebooks&version=beta) |

## <a name="next-steps"></a>Nächste Schritte

Probieren Sie einige weitere Aufrufe im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus, und verwenden Sie unseren [Schnellstart](https://developer.microsoft.com/graph/quick-start) für einen schnellen und einfachen Einstieg. Erfahren Sie mehr darüber, wie Sie [die API verwenden](use_the_api.md), um Ihre erste App zu erstellen.