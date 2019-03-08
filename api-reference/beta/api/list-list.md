---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Auflisten der SharePoint-Listen einer Website
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c91d7f8f395faa48965cb8334e1cc9eba78b978c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480712"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="f1430-102">Listen einer Website auflisten</span><span class="sxs-lookup"><span data-stu-id="f1430-102">Enumerate lists in a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1430-103">Rufen Sie die Sammlung aller [Listen][] für eine [Website][] auf.</span><span class="sxs-lookup"><span data-stu-id="f1430-103">Get the collection of [lists][] for a [site][].</span></span>

[Listen]: ../resources/list.md
[lists]: ../resources/list.md
[Website]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="f1430-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f1430-106">Permissions</span></span>

<span data-ttu-id="f1430-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1430-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1430-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f1430-109">Permission type</span></span>      | <span data-ttu-id="f1430-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f1430-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1430-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f1430-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f1430-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1430-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f1430-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f1430-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1430-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1430-114">Not supported.</span></span>    |
|<span data-ttu-id="f1430-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f1430-115">Application</span></span> | <span data-ttu-id="f1430-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1430-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1430-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1430-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="f1430-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f1430-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f1430-119">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1430-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="f1430-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1430-120">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="f1430-121">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="f1430-121">Remarks</span></span>

<span data-ttu-id="f1430-122">Listen mit dem [System][]-Facet sind standardmäßig ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="f1430-122">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="f1430-123">Fügen Sie `system` in Ihre `$select`-Anweisung ein, um sie aufzulisten.</span><span class="sxs-lookup"><span data-stu-id="f1430-123">To list them, include `system` in your `$select` statement.</span></span>

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
