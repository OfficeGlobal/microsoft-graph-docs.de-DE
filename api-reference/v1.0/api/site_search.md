---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Suchen von SharePoint-Websites nach Schlüsselwort
ms.openlocfilehash: 0f9c562da7509b213e78da85d52a091d9cec421c
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265358"
---
# <a name="search-for-sites"></a><span data-ttu-id="f0f46-102">Nach Websites suchen</span><span class="sxs-lookup"><span data-stu-id="f0f46-102">Search for sites</span></span>

<span data-ttu-id="f0f46-103">Sie können in einem gesamten SharePoint-Mandanten nach [Websites][] suchen, die den angegebenen Schlüsselwörtern entsprechen.</span><span class="sxs-lookup"><span data-stu-id="f0f46-103">Search across a SharePoint tenant for [sites][] that match provided keywords.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="f0f46-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f0f46-105">Permissions</span></span>

<span data-ttu-id="f0f46-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f0f46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f0f46-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f0f46-108">Permission type</span></span>                        | <span data-ttu-id="f0f46-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f0f46-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="f0f46-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f0f46-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f0f46-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0f46-111">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="f0f46-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f0f46-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0f46-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f0f46-113">Not supported.</span></span>
|<span data-ttu-id="f0f46-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f0f46-114">Application</span></span>                            | <span data-ttu-id="f0f46-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0f46-115">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f0f46-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f0f46-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "sites.readwrite.all", "tags": "service.sharepoint" } -->

```http
GET /sites?search={query}
```

## <a name="response"></a><span data-ttu-id="f0f46-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="f0f46-117">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Search"
} -->
