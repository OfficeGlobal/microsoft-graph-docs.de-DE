---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Auflisten der Unterwebsites für eine SharePoint-Website
localization_priority: Priority
ms.openlocfilehash: 438394a5a5e55b2352e4e42495f6a626817e128d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845056"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="13ce2-102">Unterwebsites aufzählen</span><span class="sxs-lookup"><span data-stu-id="13ce2-102">Enumerate subsites</span></span>

<span data-ttu-id="13ce2-103">Dient zum Abrufen einer Sammlung von Unterwebsites, die für ein [site][]-Objekt definiert sind.</span><span class="sxs-lookup"><span data-stu-id="13ce2-103">Get a collection of subsites defined for a [site][].</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="13ce2-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="13ce2-105">Permissions</span></span>

<span data-ttu-id="13ce2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13ce2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13ce2-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="13ce2-108">Permission type</span></span>      | <span data-ttu-id="13ce2-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="13ce2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="13ce2-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="13ce2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="13ce2-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13ce2-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="13ce2-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="13ce2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13ce2-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="13ce2-113">Not supported.</span></span>    |
|<span data-ttu-id="13ce2-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="13ce2-114">Application</span></span> | <span data-ttu-id="13ce2-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13ce2-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="13ce2-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="13ce2-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "list-subsites", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/sites
```

## <a name="response"></a><span data-ttu-id="13ce2-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="13ce2-117">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740",
      "name": "Team A Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteA"
    },
    {
      "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851",
      "name": "Team B Subsite",
      "description": "",
      "createdDateTime": "2016-10-18T03:05:59Z",
      "lastModifiedDateTime": "2016-10-18T10:40:59Z",
      "webUrl": "https://contoso.sharepoint.com/sites/site/subsiteB"
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/List subsites"
} -->
