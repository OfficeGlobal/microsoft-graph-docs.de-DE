---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Auflisten der Unterwebsites für eine SharePoint-Website
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: fd0b4c43ae03bd7f09ea095e2f7a73b6fa1dbc13
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481188"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="08603-102">Unterwebsites aufzählen</span><span class="sxs-lookup"><span data-stu-id="08603-102">Enumerate subsites</span></span>

<span data-ttu-id="08603-103">Dient zum Abrufen einer Sammlung von Unterwebsites, die für ein [site][]-Objekt definiert sind.</span><span class="sxs-lookup"><span data-stu-id="08603-103">Get a collection of subsites defined for a [site][].</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="08603-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="08603-105">Permissions</span></span>

<span data-ttu-id="08603-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08603-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08603-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="08603-108">Permission type</span></span>      | <span data-ttu-id="08603-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="08603-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08603-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="08603-110">Delegated (work or school account)</span></span> | <span data-ttu-id="08603-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08603-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="08603-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="08603-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08603-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="08603-113">Not supported.</span></span>    |
|<span data-ttu-id="08603-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="08603-114">Application</span></span> | <span data-ttu-id="08603-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08603-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08603-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="08603-116">HTTP request</span></span>

<!-- { "blockType": "request", "name": "list-subsites", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/sites
```

## <a name="response"></a><span data-ttu-id="08603-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="08603-117">Response</span></span>

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
