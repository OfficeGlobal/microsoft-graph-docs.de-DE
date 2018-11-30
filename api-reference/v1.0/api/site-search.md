---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Suchen von SharePoint-Websites nach Schlüsselwort
ms.openlocfilehash: 8022a49cd545f99df74157f80a133e3e5174a964
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020040"
---
# <a name="search-for-sites"></a><span data-ttu-id="50adc-102">Nach Websites suchen</span><span class="sxs-lookup"><span data-stu-id="50adc-102">Search for sites</span></span>

<span data-ttu-id="50adc-103">Sie können in einem gesamten SharePoint-Mandanten nach [Websites][] suchen, die den angegebenen Schlüsselwörtern entsprechen.</span><span class="sxs-lookup"><span data-stu-id="50adc-103">Search across a SharePoint tenant for [sites][] that match provided keywords.</span></span>

[sites]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="50adc-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="50adc-105">Permissions</span></span>

<span data-ttu-id="50adc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50adc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50adc-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="50adc-108">Permission type</span></span>                        | <span data-ttu-id="50adc-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="50adc-109">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="50adc-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="50adc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="50adc-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50adc-111">Sites.Read.All, Sites.ReadWrite.All</span></span>
|<span data-ttu-id="50adc-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="50adc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50adc-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50adc-113">Not supported.</span></span>
|<span data-ttu-id="50adc-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="50adc-114">Application</span></span>                            | <span data-ttu-id="50adc-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50adc-115">Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="50adc-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="50adc-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "search-sites", "scopes": "sites.readwrite.all", "tags": "service.sharepoint" } -->

```http
GET /sites?search={query}
```

## <a name="response"></a><span data-ttu-id="50adc-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="50adc-117">Response</span></span>

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