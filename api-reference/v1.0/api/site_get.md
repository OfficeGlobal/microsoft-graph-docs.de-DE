# <a name="get-a-site-resource"></a><span data-ttu-id="dfe9b-101">Site-Ressource abrufen</span><span class="sxs-lookup"><span data-stu-id="dfe9b-101">Get a site resource</span></span>

<span data-ttu-id="dfe9b-p101">Dient zum Abrufen der Eigenschaften und Beziehungen einer [site][]-Ressource. Eine **site**-Ressource stellt eine Teamwebsite in SharePoint dar.</span><span class="sxs-lookup"><span data-stu-id="dfe9b-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

<span data-ttu-id="dfe9b-104">[site]: ../resources/site.md</span><span class="sxs-lookup"><span data-stu-id="dfe9b-104">[site]: ../resources/site.md</span></span>

<span data-ttu-id="dfe9b-105">Eine **site**-Ressource wird durch einen eindeutigen Bezeichner adressiert; dies ist eine aus den folgenden Werten zusammengesetzte ID:</span><span class="sxs-lookup"><span data-stu-id="dfe9b-105">A **site** is addressed be a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="dfe9b-106">Hostname der Websitesammlung (contoso.SharePoint.com)</span><span class="sxs-lookup"><span data-stu-id="dfe9b-106">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="dfe9b-107">Eindeutige ID der Websitesammlung (GUID)</span><span class="sxs-lookup"><span data-stu-id="dfe9b-107">Site collection unique ID (guid)</span></span>
* <span data-ttu-id="dfe9b-108">Eindeutige ID der Website (GUID)</span><span class="sxs-lookup"><span data-stu-id="dfe9b-108">Site unique ID (guid)</span></span>

<span data-ttu-id="dfe9b-109">Es gibt auch einen reservierten Websitebezeichner, `root`, der immer auf die Stammwebsite für ein angegebenes Ziel verweist, wie folgt:</span><span class="sxs-lookup"><span data-stu-id="dfe9b-109">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="dfe9b-110">`/sites/root`: Der Stammwebsite des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="dfe9b-110">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="dfe9b-111">`/groups/{group-id}/sites/root`: Die Teamwebsite der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="dfe9b-111">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfe9b-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="dfe9b-112">Permissions</span></span>

<span data-ttu-id="dfe9b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="dfe9b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dfe9b-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dfe9b-115">Permission type</span></span>      | <span data-ttu-id="dfe9b-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dfe9b-116">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="dfe9b-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dfe9b-117">Delegated (work or school account)</span></span> | <span data-ttu-id="dfe9b-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfe9b-118">Sites.Read.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="dfe9b-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dfe9b-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfe9b-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dfe9b-120">Not supported.</span></span>    | 
|<span data-ttu-id="dfe9b-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dfe9b-121">Application</span></span> | <span data-ttu-id="dfe9b-122">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfe9b-122">Sites.Read.All, Sites.ReadWrite.All</span></span> | 

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="dfe9b-123">Abrufen der Stammwebsite eines Mandanten</span><span class="sxs-lookup"><span data-stu-id="dfe9b-123">Get the tenant's root site</span></span>

<span data-ttu-id="dfe9b-124">So greifen Sie innerhalb eines Mandanten auf die SharePoint-Stammwebsite zu:</span><span class="sxs-lookup"><span data-stu-id="dfe9b-124">To access the root SharePoint site within a tenant:</span></span>

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="dfe9b-125">Über eine serverrelative URL auf eine Website zugreifen</span><span class="sxs-lookup"><span data-stu-id="dfe9b-125">Access a site by server-relative URL</span></span>

<span data-ttu-id="dfe9b-126">Wenn Sie über die serverrelative URL für eine **site**-Ressource verfügen, können Sie eine Anforderung wie folgt erstellen:</span><span class="sxs-lookup"><span data-stu-id="dfe9b-126">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="dfe9b-127">Auf die Teamwebsite einer Gruppe zugreifen</span><span class="sxs-lookup"><span data-stu-id="dfe9b-127">Access a group team site</span></span>

<span data-ttu-id="dfe9b-128">So greifen Sie auf die Teamwebsite für eine [group](../resources/group.md)-Ressource zu:</span><span class="sxs-lookup"><span data-stu-id="dfe9b-128">To access the team site for a [group](../resources/group.md):</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="dfe9b-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dfe9b-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dfe9b-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dfe9b-130">Request</span></span>

<!-- { "blockType": "request", "name": "get-site", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}
```

##### <a name="response"></a><span data-ttu-id="dfe9b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="dfe9b-131">Response</span></span>

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
