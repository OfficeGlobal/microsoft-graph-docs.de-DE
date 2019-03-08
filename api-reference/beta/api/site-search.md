---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Suchen von SharePoint-Websites nach Stichwort
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ee4aa139508e6a523ea1858c6b0598a5b8aaf9b5
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480754"
---
# <a name="search-for-sites"></a><span data-ttu-id="0d146-102">Nach Websites suchen</span><span class="sxs-lookup"><span data-stu-id="0d146-102">Search for sites</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d146-103">Sie können in einem gesamten SharePoint-Mandanten nach [Websites][] suchen, die den angegebenen Schlüsselwörtern entsprechen.</span><span class="sxs-lookup"><span data-stu-id="0d146-103">Search across a SharePoint tenant for [sites][] that match provided keywords.</span></span>

[Websites]: ../resources/site.md
[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="0d146-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0d146-105">Permissions</span></span>

<span data-ttu-id="0d146-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d146-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d146-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0d146-108">Permission type</span></span>                        | <span data-ttu-id="0d146-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0d146-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="0d146-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0d146-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d146-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d146-111">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="0d146-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0d146-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d146-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0d146-113">Not supported.</span></span>
|<span data-ttu-id="0d146-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0d146-114">Application</span></span>                            | <span data-ttu-id="0d146-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d146-115">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="0d146-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0d146-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "service.sharepoint sites.readwrite.all" } -->

```http
GET https://graph.microsoft.com/beta/sites?search={query}
```

## <a name="response"></a><span data-ttu-id="0d146-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="0d146-117">Response</span></span>

<!-- { "blockType": "response", "@type": "Collection(microsoft.graph.site)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Site",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/siteA"
    },
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Site",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/siteB"
    }
  ]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search",
  "suppressions": [
    "Error: /api-reference/beta/api/site-search.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
