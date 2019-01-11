---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Auflisten der Unterwebsites für eine SharePoint-Website
localization_priority: Normal
ms.openlocfilehash: b773dc217836fe2474c244917773d9496d158a6a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835427"
---
# <a name="enumerate-subsites"></a><span data-ttu-id="8a07d-102">Unterwebsites aufzählen</span><span class="sxs-lookup"><span data-stu-id="8a07d-102">Enumerate subsites</span></span>

> <span data-ttu-id="8a07d-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8a07d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a07d-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8a07d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8a07d-105">Dient zum Abrufen einer Sammlung von Unterwebsites, die für ein [site][]-Objekt definiert sind.</span><span class="sxs-lookup"><span data-stu-id="8a07d-105">Get a collection of subsites defined for a [site][].</span></span>

[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="8a07d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8a07d-107">Permissions</span></span>

<span data-ttu-id="8a07d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a07d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a07d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8a07d-110">Permission type</span></span>      | <span data-ttu-id="8a07d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8a07d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a07d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8a07d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8a07d-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a07d-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8a07d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8a07d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a07d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a07d-115">Not supported.</span></span>    |
|<span data-ttu-id="8a07d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8a07d-116">Application</span></span> | <span data-ttu-id="8a07d-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a07d-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a07d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a07d-118">HTTP request</span></span>

<!-- { "blockType": "request", "name": "list-subsites", "scopes": "service.sharepoint sites.read.all" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/sites
```

## <a name="response"></a><span data-ttu-id="8a07d-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a07d-119">Response</span></span>

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
