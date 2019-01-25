---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Auflisten der SharePoint-Listen einer Website
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f7adfeba7f46eb7ed8541405221a1257637c2157
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512444"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="c3a8e-102">Listen einer Website auflisten</span><span class="sxs-lookup"><span data-stu-id="c3a8e-102">Enumerate lists in a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3a8e-103">Rufen Sie die Sammlung aller [Listen][] für eine [Website][] auf.</span><span class="sxs-lookup"><span data-stu-id="c3a8e-103">Get the collection of [lists][] for a [site][].</span></span>

[Listen]: ../resources/list.md
[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="c3a8e-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c3a8e-106">Permissions</span></span>

<span data-ttu-id="c3a8e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3a8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3a8e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c3a8e-109">Permission type</span></span>      | <span data-ttu-id="c3a8e-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c3a8e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3a8e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c3a8e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c3a8e-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3a8e-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c3a8e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c3a8e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3a8e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c3a8e-114">Not supported.</span></span>    |
|<span data-ttu-id="c3a8e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c3a8e-115">Application</span></span> | <span data-ttu-id="c3a8e-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3a8e-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3a8e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3a8e-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="c3a8e-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c3a8e-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c3a8e-119">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3a8e-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="c3a8e-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="c3a8e-120">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b57af081-936c-4803-a120-d94887b03864",
      "name": "Documents",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "documentLibrary"
       }
    },
    {
      "id": "1234-112-112-4",
      "name": "MicroFeed",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "genericList"
       }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="c3a8e-121">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="c3a8e-121">Remarks</span></span>

<span data-ttu-id="c3a8e-122">Listen mit dem [System][]-Facet sind standardmäßig ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="c3a8e-122">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="c3a8e-123">Fügen Sie `system` in Ihre `$select`-Anweisung ein, um sie aufzulisten.</span><span class="sxs-lookup"><span data-stu-id="c3a8e-123">To list them, include `system` in your `$select` statement.</span></span>

[System]: ../resources/systemfacet.md
[system]: ../resources/systemfacet.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate",
  "suppressions": [
    "Error: /api-reference/beta/api/list-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
