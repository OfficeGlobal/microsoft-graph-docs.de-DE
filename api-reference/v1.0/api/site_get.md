# <a name="get-a-site-resource"></a>Site-Ressource abrufen

Dient zum Abrufen der Eigenschaften und Beziehungen einer [site][]-Ressource. Eine **site**-Ressource stellt eine Teamwebsite in SharePoint dar.

[site]: ../resources/site.md

Eine **site**-Ressource wird durch einen eindeutigen Bezeichner adressiert; dies ist eine aus den folgenden Werten zusammengesetzte ID:

* Hostname der Websitesammlung (contoso.SharePoint.com)
* Eindeutige ID der Websitesammlung (GUID)
* Eindeutige ID der Website (GUID)

Es gibt auch einen reservierten Websitebezeichner, `root`, der immer auf die Stammwebsite für ein angegebenes Ziel verweist, wie folgt:

* `/sites/root`: Der Stammwebsite des Mandanten.
* `/groups/{group-id}/sites/root`: Die Teamwebsite der Gruppe.

## <a name="prerequisites"></a>Anforderungen

Einer der folgenden Bereiche ist erforderlich, um diese Anforderung auszuführen:

* Sites.Read.All
* Sites.ReadWrite.All

## <a name="get-the-tenants-root-site"></a>Stammwebsite des Mandanten abrufen

So greifen Sie innerhalb eines Mandanten auf die SharePoint-Stammwebsite zu:

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a>Über eine serverrelative URL auf eine Website zugreifen

Wenn Sie über die serverrelative URL für eine **site**-Ressource verfügen, können Sie eine Anforderung wie folgt erstellen:

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a>Auf die Teamwebsite einer Gruppe zugreifen

So greifen Sie auf die Teamwebsite für eine [group](../resources/group.md)-Ressource zu:

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}
```

##### <a name="response"></a>Antwort

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "d297964f-d325-424b-a002-f54048a4622e",
    "name": "OneDrive / SharePoint Team",
    "description": "Collaboration site for the OneDrive and SharePoint team",
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Site/Get site by ID"
} -->
