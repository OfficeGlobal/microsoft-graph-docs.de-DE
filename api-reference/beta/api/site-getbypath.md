---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePoint-Website nach Pfad abrufen
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: afded48114342e8bf5eb76d25f1361f67686af54
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936186"
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="25288-102">Site-Ressource nach Pfad abrufen</span><span class="sxs-lookup"><span data-stu-id="25288-102">Get a site resource by path</span></span>

> <span data-ttu-id="25288-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="25288-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="25288-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="25288-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="25288-p102">Dient zum Abrufen der Eigenschaften und Beziehungen einer [site][]-Ressource. Eine **site**-Ressource stellt eine Teamwebsite in SharePoint dar.</span><span class="sxs-lookup"><span data-stu-id="25288-p102">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="25288-108">Zusätzlich zum Abrufen einer [Website nach ID](site-get.md) können Sie eine Website basierend auf dem serverrelativen URL-Pfad abrufen.</span><span class="sxs-lookup"><span data-stu-id="25288-108">In addition to retrieving a [site by ID](site-get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="25288-109">Hostname der Websitesammlung (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="25288-109">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="25288-110">Websitepfad relativ zum Hostnamen des Servers</span><span class="sxs-lookup"><span data-stu-id="25288-110">Site path, relative to server hostname.</span></span>

<span data-ttu-id="25288-111">Es gibt auch einen reservierten Websitebezeichner, `root`, der immer auf die Stammwebsite für ein angegebenes Ziel verweist, wie folgt:</span><span class="sxs-lookup"><span data-stu-id="25288-111">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="25288-112">`/sites/root`: Der Stammwebsite des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="25288-112">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="25288-113">`/groups/{group-id}/sites/root`: Die Teamwebsite der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="25288-113">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="25288-114">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="25288-114">Permissions</span></span>

<span data-ttu-id="25288-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25288-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25288-117">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="25288-117">Permission type</span></span>      | <span data-ttu-id="25288-118">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="25288-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25288-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="25288-119">Delegated (work or school account)</span></span> | <span data-ttu-id="25288-120">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25288-120">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="25288-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="25288-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25288-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="25288-122">Not supported.</span></span>    |
|<span data-ttu-id="25288-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="25288-123">Application</span></span> | <span data-ttu-id="25288-124">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25288-124">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="25288-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="25288-125">HTTP Request</span></span>

<span data-ttu-id="25288-126">So greifen Sie mit einem relativen Pfad auf die SharePoint-Stammwebsite zu:</span><span class="sxs-lookup"><span data-stu-id="25288-126">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a><span data-ttu-id="25288-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="25288-127">Response</span></span>

<span data-ttu-id="25288-128">Diese Methode gibt eine [site][]-Ressource für die Website zurück, auf die vom eindeutigen Bezeichner verwiesen wird.</span><span class="sxs-lookup"><span data-stu-id="25288-128">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.site" } -->

```http
HTTP/1.1 200 OK

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
  "tocPath": "Sites/Get by path"
} -->
