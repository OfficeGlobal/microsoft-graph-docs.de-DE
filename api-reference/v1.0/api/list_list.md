---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Auflisten der SharePoint-Listen einer Website
ms.openlocfilehash: 4be4c4aefc29cdcd684bc11ad086b5c0572dbe2b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2017
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="2cb71-102">Listen einer Website auflisten</span><span class="sxs-lookup"><span data-stu-id="2cb71-102">Enumerate lists in a site</span></span>

<span data-ttu-id="2cb71-103">Rufen Sie die Sammlung aller [Listen][] für eine [Website][] auf.</span><span class="sxs-lookup"><span data-stu-id="2cb71-103">Get the collection of [lists][] for a [site][].</span></span>

[Listen]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="2cb71-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2cb71-106">Permissions</span></span>

<span data-ttu-id="2cb71-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2cb71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2cb71-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2cb71-109">Permission type</span></span>      | <span data-ttu-id="2cb71-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2cb71-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2cb71-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2cb71-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2cb71-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cb71-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2cb71-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2cb71-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cb71-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2cb71-114">Not supported.</span></span>    |
|<span data-ttu-id="2cb71-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2cb71-115">Application</span></span> | <span data-ttu-id="2cb71-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cb71-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2cb71-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2cb71-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="2cb71-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2cb71-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2cb71-119">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2cb71-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="2cb71-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="2cb71-120">Response</span></span>

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
