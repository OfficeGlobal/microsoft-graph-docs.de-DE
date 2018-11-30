---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePoint-Website abrufen
ms.openlocfilehash: a9fc304c52413a53d3fa352fa8e950a9f9ed8a77
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064563"
---
# <a name="get-a-site-resource"></a><span data-ttu-id="4c61f-102">Site-Ressource abrufen</span><span class="sxs-lookup"><span data-stu-id="4c61f-102">Get a site resource</span></span>

> <span data-ttu-id="4c61f-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4c61f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c61f-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4c61f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4c61f-p102">Dient zum Abrufen der Eigenschaften und Beziehungen einer [site][]-Ressource. Eine **site**-Ressource stellt eine Teamwebsite in SharePoint dar.</span><span class="sxs-lookup"><span data-stu-id="4c61f-p102">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="4c61f-108">Eine **site**-Ressource wird durch einen eindeutigen Bezeichner adressiert; dies ist eine aus den folgenden Werten zusammengesetzte ID:</span><span class="sxs-lookup"><span data-stu-id="4c61f-108">A **site** is addressed be a unique identifier which is a composite ID of the following values:</span></span>

* <span data-ttu-id="4c61f-109">Hostname der Websitesammlung (contoso.SharePoint.com)</span><span class="sxs-lookup"><span data-stu-id="4c61f-109">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="4c61f-110">Eindeutige ID der Websitesammlung (GUID)</span><span class="sxs-lookup"><span data-stu-id="4c61f-110">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="4c61f-111">Eindeutige ID der Website (GUID)</span><span class="sxs-lookup"><span data-stu-id="4c61f-111">Site unique ID (GUID)</span></span>

<span data-ttu-id="4c61f-112">Es gibt auch einen reservierten Websitebezeichner, `root`, der immer auf die Stammwebsite für ein angegebenes Ziel verweist, wie folgt:</span><span class="sxs-lookup"><span data-stu-id="4c61f-112">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="4c61f-113">`/sites/root`: Der Stammwebsite des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4c61f-113">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="4c61f-114">`/groups/{group-id}/sites/root`: Die Teamwebsite der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="4c61f-114">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c61f-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4c61f-115">Permissions</span></span>

<span data-ttu-id="4c61f-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c61f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c61f-118">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4c61f-118">Permission type</span></span>      | <span data-ttu-id="4c61f-119">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4c61f-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c61f-120">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4c61f-120">Delegated (work or school account)</span></span> | <span data-ttu-id="4c61f-121">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c61f-121">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c61f-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4c61f-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c61f-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4c61f-123">Not supported.</span></span>    |
|<span data-ttu-id="4c61f-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4c61f-124">Application</span></span> | <span data-ttu-id="4c61f-125">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c61f-125">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-the-tenants-root-site"></a><span data-ttu-id="4c61f-126">Abrufen der Stammwebsite eines Mandanten</span><span class="sxs-lookup"><span data-stu-id="4c61f-126">Get the tenant's root site</span></span>

<span data-ttu-id="4c61f-127">So greifen Sie innerhalb eines Mandanten auf die SharePoint-Stammwebsite zu:</span><span class="sxs-lookup"><span data-stu-id="4c61f-127">To access the root SharePoint site within a tenant:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/root
GET /sites/contoso.sharepoint.com
```

## <a name="access-a-site-by-server-relative-url"></a><span data-ttu-id="4c61f-128">Über eine serverrelative URL auf eine Website zugreifen</span><span class="sxs-lookup"><span data-stu-id="4c61f-128">Access a site by server-relative URL</span></span>

<span data-ttu-id="4c61f-129">Wenn Sie über die serverrelative URL für eine **site**-Ressource verfügen, können Sie eine Anforderung wie folgt erstellen:</span><span class="sxs-lookup"><span data-stu-id="4c61f-129">If you have the server-relative URL for a **site** resource, you can construct a request as follows:</span></span>

```http
GET /sites/{hostname}:/{server-relative-path}
```

## <a name="access-a-group-team-site"></a><span data-ttu-id="4c61f-130">Auf die Teamwebsite einer Gruppe zugreifen</span><span class="sxs-lookup"><span data-stu-id="4c61f-130">Access a group team site</span></span>

<span data-ttu-id="4c61f-131">So greifen Sie auf die Teamwebsite für eine  Gruppe zu:</span><span class="sxs-lookup"><span data-stu-id="4c61f-131">To access the team site for a group:</span></span>

```http
GET /groups/{group-id}/sites/root
```

## <a name="example"></a><span data-ttu-id="4c61f-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4c61f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c61f-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c61f-133">Request</span></span>

<!-- { "blockType": "request", "name": "get-site" } -->

```http
GET /sites/{site-id}
```

### <a name="response"></a><span data-ttu-id="4c61f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c61f-134">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "contoso.sharepoint.com,2C712604-1370-44E7-A1F5-426573FDA80A,2D2244C3-251A-49EA-93A8-39E1C3A060FE",
  "owner": {
    "user": {
      "displayName": "Daron Spektor",
      "id": "5280E7FE-DC7A-4486-9490-E790D81DFEB3"
    }
  },
  "displayName": "OneDrive Team Site",
  "name": "1drvteam",
  "createdDateTime": "2017-05-09T20:56:00Z",
  "lastModifiedDateTime": "2017-05-09T20:56:01Z",
  "webUrl": "https://contoso.sharepoint.com/teams/1drvteam"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by ID"
} -->
