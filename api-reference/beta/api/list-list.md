---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Auflisten der SharePoint-Listen einer Website
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fa13fc93dcfcfc807671082be43a7c4b4eafd63d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957872"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="339de-102">Listen einer Website auflisten</span><span class="sxs-lookup"><span data-stu-id="339de-102">Enumerate lists in a site</span></span>

> <span data-ttu-id="339de-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="339de-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="339de-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="339de-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="339de-105">Rufen Sie die Sammlung aller [Listen][] für eine [Website][] auf.</span><span class="sxs-lookup"><span data-stu-id="339de-105">Get the collection of [lists][] for a [site][].</span></span>

[Listen]: ../resources/list.md
[lists]: ../resources/list.md
[Website]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="339de-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="339de-108">Permissions</span></span>

<span data-ttu-id="339de-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="339de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="339de-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="339de-111">Permission type</span></span>      | <span data-ttu-id="339de-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="339de-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="339de-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="339de-113">Delegated (work or school account)</span></span> | <span data-ttu-id="339de-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="339de-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="339de-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="339de-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="339de-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="339de-116">Not supported.</span></span>    |
|<span data-ttu-id="339de-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="339de-117">Application</span></span> | <span data-ttu-id="339de-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="339de-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="339de-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="339de-119">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="339de-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="339de-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="339de-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="339de-121">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="339de-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="339de-122">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="339de-123">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="339de-123">Remarks</span></span>

<span data-ttu-id="339de-124">Listen mit dem [System][]-Facet sind standardmäßig ausgeblendet.</span><span class="sxs-lookup"><span data-stu-id="339de-124">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="339de-125">Fügen Sie `system` in Ihre `$select`-Anweisung ein, um sie aufzulisten.</span><span class="sxs-lookup"><span data-stu-id="339de-125">To list them, include `system` in your `$select` statement.</span></span>

[System]: ../resources/systemfacet.md
[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate"
} -->
