---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Suchen von SharePoint-Websites nach Schlüsselwort
ms.openlocfilehash: c3c5ba005521e3405018e9b9403976297046f242
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066168"
---
# <a name="search-for-sites"></a><span data-ttu-id="5237f-102">Nach Websites suchen</span><span class="sxs-lookup"><span data-stu-id="5237f-102">Search for sites</span></span>

> <span data-ttu-id="5237f-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5237f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5237f-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5237f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5237f-105">Sie können in einem gesamten SharePoint-Mandanten nach [Websites][] suchen, die den angegebenen Schlüsselwörtern entsprechen.</span><span class="sxs-lookup"><span data-stu-id="5237f-105">Search across a SharePoint tenant for [sites][] that match provided keywords.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="5237f-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5237f-107">Permissions</span></span>

<span data-ttu-id="5237f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5237f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5237f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5237f-110">Permission type</span></span>                        | <span data-ttu-id="5237f-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5237f-111">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="5237f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5237f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5237f-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5237f-113">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="5237f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5237f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5237f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5237f-115">Not supported.</span></span>
|<span data-ttu-id="5237f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5237f-116">Application</span></span>                            | <span data-ttu-id="5237f-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5237f-117">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="5237f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5237f-118">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "service.sharepoint sites.readwrite.all" } -->

```http
GET https://graph.microsoft.com/beta/sites?search={query}
```

## <a name="response"></a><span data-ttu-id="5237f-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="5237f-119">Response</span></span>

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
