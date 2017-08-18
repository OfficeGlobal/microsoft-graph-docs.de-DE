# <a name="get-a-site-resource"></a><span data-ttu-id="36ec0-101">Site-Ressource abrufen</span><span class="sxs-lookup"><span data-stu-id="36ec0-101">Get a site resource</span></span>

<span data-ttu-id="36ec0-p101">Dient zum Abrufen der Eigenschaften und Beziehungen einer [site][]-Ressource. Eine **site**-Ressource stellt eine Teamwebsite in SharePoint dar.</span><span class="sxs-lookup"><span data-stu-id="36ec0-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

<span data-ttu-id="36ec0-104">[site]: ../resources/site.md</span><span class="sxs-lookup"><span data-stu-id="36ec0-104">[site]: ../resources/site.md</span></span>

<span data-ttu-id="36ec0-105">Eine **site**-Ressource wird durch einen eindeutigen Bezeichner adressiert; dies ist eine aus den folgenden Werten zusammengesetzte ID:</span><span class="sxs-lookup"><span data-stu-id="36ec0-105">A **site** is addressed be a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="36ec0-106">Hostname der Websitesammlung (contoso.SharePoint.com)</span><span class="sxs-lookup"><span data-stu-id="36ec0-106">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="36ec0-107">Eindeutige ID der Websitesammlung (GUID)</span><span class="sxs-lookup"><span data-stu-id="36ec0-107">Site collection unique ID (guid)</span></span>
* <span data-ttu-id="36ec0-108">Eindeutige ID der Website (GUID)</span><span class="sxs-lookup"><span data-stu-id="36ec0-108">Site unique ID (guid)</span></span>

<span data-ttu-id="36ec0-109">Es gibt auch einen reservierten Websitebezeichner, `root`, der immer auf die Stammwebsite für ein angegebenes Ziel verweist, wie folgt:</span><span class="sxs-lookup"><span data-stu-id="36ec0-109">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="36ec0-110">`/sites/root`: Der Stammwebsite des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="36ec0-110">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="36ec0-111">`/groups/{group-id}/sites/root`: Die Teamwebsite der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="36ec0-111">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36ec0-112">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="36ec0-112">Prerequisites</span></span>

<span data-ttu-id="36ec0-113">Einer der folgenden Bereiche ist erforderlich, um diese Anforderung auszuführen:</span><span class="sxs-lookup"><span data-stu-id="36ec0-113">One of the following scopes is required to execute this request:</span></span>

* <span data-ttu-id="36ec0-114">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="36ec0-114">Sites.Read.All</span></span>
* <span data-ttu-id="36ec0-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36ec0-115">Sites.ReadWrite.All</span></span>

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="36ec0-116">Stammwebsite des Mandanten abrufen</span><span class="sxs-lookup"><span data-stu-id="36ec0-116">Get the tenant's root site</span></span>

<span data-ttu-id="36ec0-117">So greifen Sie innerhalb eines Mandanten auf die SharePoint-Stammwebsite zu:</span><span class="sxs-lookup"><span data-stu-id="36ec0-117">To access the root SharePoint site within a tenant:</span></span>

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="36ec0-118">Über eine serverrelative URL auf eine Website zugreifen</span><span class="sxs-lookup"><span data-stu-id="36ec0-118">Access a site by server-relative URL</span></span>

<span data-ttu-id="36ec0-119">Wenn Sie über die serverrelative URL für eine **site**-Ressource verfügen, können Sie eine Anforderung wie folgt erstellen:</span><span class="sxs-lookup"><span data-stu-id="36ec0-119">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="36ec0-120">Auf die Teamwebsite einer Gruppe zugreifen</span><span class="sxs-lookup"><span data-stu-id="36ec0-120">Access a group team site</span></span>

<span data-ttu-id="36ec0-121">So greifen Sie auf die Teamwebsite für eine [group](../resources/group.md)-Ressource zu:</span><span class="sxs-lookup"><span data-stu-id="36ec0-121">To access the team site for a [group](../resources/group.md):</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="36ec0-122">Beispiel</span><span class="sxs-lookup"><span data-stu-id="36ec0-122">Example</span></span>

##### <a name="request"></a><span data-ttu-id="36ec0-123">Anforderung</span><span class="sxs-lookup"><span data-stu-id="36ec0-123">Request</span></span>

<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}
```

##### <a name="response"></a><span data-ttu-id="36ec0-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="36ec0-124">Response</span></span>

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
