---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePoint-Website nach Pfad abrufen
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c81e025f8cee7acfc4eb9761d2168c200d0d4d5a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508804"
---
# <a name="get-a-site-resource-by-path"></a><span data-ttu-id="fca0b-102">Site-Ressource nach Pfad abrufen</span><span class="sxs-lookup"><span data-stu-id="fca0b-102">Get a site resource by path</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fca0b-p101">Dient zum Abrufen der Eigenschaften und Beziehungen einer [site][]-Ressource. Eine **site**-Ressource stellt eine Teamwebsite in SharePoint dar.</span><span class="sxs-lookup"><span data-stu-id="fca0b-p101">Retrieve properties and relationships for a [site][] resource. A **site** resource represents a team site in SharePoint.</span></span>

[site]: ../resources/site.md

<span data-ttu-id="fca0b-106">Zusätzlich zum Abrufen einer [Website nach ID](site-get.md) können Sie eine Website basierend auf dem serverrelativen URL-Pfad abrufen.</span><span class="sxs-lookup"><span data-stu-id="fca0b-106">In addition to retrieving a [site by ID](site-get.md) you can retrieve a site based on server-relative URL path.</span></span>

* <span data-ttu-id="fca0b-107">Hostname der Websitesammlung (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="fca0b-107">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="fca0b-108">Websitepfad relativ zum Hostnamen des Servers</span><span class="sxs-lookup"><span data-stu-id="fca0b-108">Site path, relative to server hostname.</span></span>

<span data-ttu-id="fca0b-109">Es gibt auch einen reservierten Websitebezeichner, `root`, der immer auf die Stammwebsite für ein angegebenes Ziel verweist, wie folgt:</span><span class="sxs-lookup"><span data-stu-id="fca0b-109">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="fca0b-110">`/sites/root`: Der Stammwebsite des Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fca0b-110">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="fca0b-111">`/groups/{group-id}/sites/root`: Die Teamwebsite der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="fca0b-111">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="permissions"></a><span data-ttu-id="fca0b-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fca0b-112">Permissions</span></span>

<span data-ttu-id="fca0b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fca0b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fca0b-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fca0b-115">Permission type</span></span>      | <span data-ttu-id="fca0b-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fca0b-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fca0b-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fca0b-117">Delegated (work or school account)</span></span> | <span data-ttu-id="fca0b-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fca0b-118">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fca0b-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fca0b-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fca0b-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fca0b-120">Not supported.</span></span>    |
|<span data-ttu-id="fca0b-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fca0b-121">Application</span></span> | <span data-ttu-id="fca0b-122">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fca0b-122">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fca0b-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fca0b-123">HTTP Request</span></span>

<span data-ttu-id="fca0b-124">So greifen Sie mit einem relativen Pfad auf die SharePoint-Stammwebsite zu:</span><span class="sxs-lookup"><span data-stu-id="fca0b-124">To access the root SharePoint site with a relative path:</span></span>

<!-- { "blockType": "request", "name": "get-site-by-hostname-and-path", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET /sites/{hostname}:/{relative-path}
```

## <a name="response"></a><span data-ttu-id="fca0b-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="fca0b-125">Response</span></span>

<span data-ttu-id="fca0b-126">Diese Methode gibt eine [site][]-Ressource für die Website zurück, auf die vom eindeutigen Bezeichner verwiesen wird.</span><span class="sxs-lookup"><span data-stu-id="fca0b-126">This method returns a [site][] resource for the site referenced by the unique identifier.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Get by path",
  "suppressions": [
    "Error: /api-reference/beta/api/site-getbypath.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
