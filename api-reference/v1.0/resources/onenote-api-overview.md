# <a name="use-the-onenote-rest-api"></a>Verwenden der OneNote-REST-API

Mit Microsoft Graph erhält Ihre App autorisierten Zugriff auf die OneNote-Notizbücher, Abschnitte und Seiten eines Benutzers in einem persönlichen oder Organisationskonto. Mit den [entsprechenden Berechtigungen für delegierte oder Anwendungsberechtigungen](../../../concepts/permissions_reference.md#notes-permissions) kann Ihre App auf die OneNote-Daten des angemeldeten Benutzers oder jedes Benutzers in einem Mandanten zugreifen.

## <a name="root-url"></a>Stamm-URL
Die Stamm-URL des OneNote-Diensts verwendet das folgende Format für alle Aufrufe der OneNote-API:
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
Das Segment `version` in der URL ist die Version von Microsoft Graph, die verwendet werden soll:

- `v1.0` ist für stabilen Produktionscode.
- `beta` |||UNTRANSLATED_CONTENT_START|||is to try out a feature that's in development.|||UNTRANSLATED_CONTENT_END||| Funktionen und Funktionalität in der Betaversion ändern sich möglicherweise, sodass Sie diese nicht in Ihrem Produktionscode verwenden sollten.

Speicherort können Benutzernotizbücher in Office 365 oder dem Verbraucher-OneDrive, Gruppennotizbücher oder auf einer SharePoint-Website gehostete Teamnotizbücher in Office 365 sein. 

![OneNote-API-Entwicklungsstapel](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a>Benutzer-Notizbücher
Verwenden Sie eine der folgenden URLs, um auf persönliche Notizbücher in Consumer-OneDrive oder in OneDrive for Business zuzugreifen:

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- `me` |||UNTRANSLATED_CONTENT_START|||is for OneNote content that the current user can access (owned and shared).|||UNTRANSLATED_CONTENT_END|||
- `users/{id}` |||UNTRANSLATED_CONTENT_START|||is for OneNote content that the specified user (in the URL) has shared with the current user.|||UNTRANSLATED_CONTENT_END||| Verwenden Sie die [Benutzer](users.md)-API.
> **Hinweis:** Benutzer-IDs können Sie über eine GET-Anforderung an `https://graph.microsoft.com/v1.0/users` abrufen.

### <a name="group-notebooks"></a>Gruppen-Notizbücher
Verwenden Sie die folgende Dienststamm-URL, um auf Notizbücher zuzugreifen, die im Besitz einer Gruppe sind:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a>SharePoint Website-Notebooks

Verwenden Sie die folgende Dienststamm-URL, um auf Notizbücher zuzugreifen, die einer SharePoint-Teamwebsite gehören:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

