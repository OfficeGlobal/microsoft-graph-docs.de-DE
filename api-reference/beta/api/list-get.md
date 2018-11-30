---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Abrufen einer SharePoint-Liste
ms.openlocfilehash: 8cda18e17197a6f14a3c60903fa0c4ad43ed684d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062406"
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="920dc-102">Metadaten für eine Liste abrufen</span><span class="sxs-lookup"><span data-stu-id="920dc-102">Get metadata for a list</span></span>

> <span data-ttu-id="920dc-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="920dc-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="920dc-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="920dc-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="920dc-105">Gibt die Metadaten für ein eine [Liste][] zurück.</span><span class="sxs-lookup"><span data-stu-id="920dc-105">Returns the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="920dc-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="920dc-107">Permissions</span></span>

<span data-ttu-id="920dc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="920dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="920dc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="920dc-110">Permission type</span></span>      | <span data-ttu-id="920dc-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="920dc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="920dc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="920dc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="920dc-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="920dc-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="920dc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="920dc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="920dc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="920dc-115">Not supported.</span></span>    |
|<span data-ttu-id="920dc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="920dc-116">Application</span></span> | <span data-ttu-id="920dc-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="920dc-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="920dc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="920dc-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="920dc-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="920dc-119">Request body</span></span>

<span data-ttu-id="920dc-120">Bei dieser Methode wird kein Anforderungstext angegeben.</span><span class="sxs-lookup"><span data-stu-id="920dc-120">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="920dc-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="920dc-121">Example</span></span>

#### <a name="request"></a><span data-ttu-id="920dc-122">Anforderung</span><span class="sxs-lookup"><span data-stu-id="920dc-122">Request</span></span>

<!-- { "blockType": "request", "name": "get-list" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a><span data-ttu-id="920dc-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="920dc-123">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

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
```

<span data-ttu-id="920dc-124">Mit `select`- und `expand`-Anweisungen können Sie Listen-Metadaten, Spaltendefinitionen und Listenelemente in einer einzigen Anforderung abrufen.</span><span class="sxs-lookup"><span data-stu-id="920dc-124">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="920dc-125">Anforderung</span><span class="sxs-lookup"><span data-stu-id="920dc-125">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a><span data-ttu-id="920dc-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="920dc-126">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "truncated": true, "scopes": "sites.read.all service.sharepoint" } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "name": "Inventory",
  "lastModifiedDateTime": "2016-08-30T08:32:00Z",
  "columns": [
    {
      "name": "Name",
      "description": "Customer-facing name of the SKU"
    },
    {
      "name": "Color",
      "description": "Color of the item in stock"
    },
    {
      "name": "Quantity",
      "description": "Number of items in stock"
    }
  ],
  "items": [
    {
      "id": "2",
      "fields": {
        "Name": "Gadget",
        "Color": "Red",
        "Quantity": 503
       }
    },
    {
      "id": "4",
      "fields": {
        "Name": "Widget",
        "Color": "Blue",
        "Quantity": 2357
       }
    },
    {
      "id": "7",
      "fields": {
        "Name": "Gizmo",
        "Color": "Green",
        "Quantity": 92
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
  "tocPath": "Lists/Get metadata"
} -->
