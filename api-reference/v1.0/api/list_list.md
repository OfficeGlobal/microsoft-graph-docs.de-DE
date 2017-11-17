---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Auflisten der SharePoint-Listen einer Website
ms.openlocfilehash: 8c3d8da3e8dc4ab3aa2f399eb09d916ea602e1c5
ms.sourcegitcommit: 339070a20730bc4d363da7eb346d5f3c1e1d6c3e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/18/2017
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="59817-102">Listen einer Website auflisten</span><span class="sxs-lookup"><span data-stu-id="59817-102">Enumerate lists in a site</span></span>

<span data-ttu-id="59817-103">Rufen Sie die Sammlung aller [Listen][] für eine [Website][] auf.</span><span class="sxs-lookup"><span data-stu-id="59817-103">Get the collection of [lists][] for a [site][].</span></span>

[Listen]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="59817-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="59817-106">Permissions</span></span>

<span data-ttu-id="59817-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="59817-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="59817-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="59817-109">Permission type</span></span>      | <span data-ttu-id="59817-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="59817-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59817-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="59817-111">Delegated (work or school account)</span></span> | <span data-ttu-id="59817-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59817-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="59817-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="59817-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59817-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="59817-114">Not supported.</span></span>    |
|<span data-ttu-id="59817-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="59817-115">Application</span></span> | <span data-ttu-id="59817-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59817-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59817-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="59817-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="59817-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="59817-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="59817-119">Anforderung</span><span class="sxs-lookup"><span data-stu-id="59817-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="59817-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="59817-120">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate"
} -->
