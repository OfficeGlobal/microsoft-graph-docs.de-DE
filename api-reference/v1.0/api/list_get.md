---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Abrufen einer SharePoint-Liste
ms.openlocfilehash: e0e0ccdc0836c40ac4f5a719cd64f02178030ccd
ms.sourcegitcommit: 339070a20730bc4d363da7eb346d5f3c1e1d6c3e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/18/2017
---
# <a name="get-metadata-for-a-list"></a><span data-ttu-id="23e10-102">Metadaten für eine Liste abrufen</span><span class="sxs-lookup"><span data-stu-id="23e10-102">Get metadata for a list</span></span>

<span data-ttu-id="23e10-103">Gibt die Metadaten für ein eine [Liste][] zurück.</span><span class="sxs-lookup"><span data-stu-id="23e10-103">Returns the metadata for a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="23e10-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="23e10-105">Permissions</span></span>

<span data-ttu-id="23e10-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="23e10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="23e10-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="23e10-108">Permission type</span></span>      | <span data-ttu-id="23e10-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="23e10-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23e10-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="23e10-110">Delegated (work or school account)</span></span> | <span data-ttu-id="23e10-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23e10-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="23e10-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="23e10-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23e10-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23e10-113">Not supported.</span></span>    |
|<span data-ttu-id="23e10-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="23e10-114">Application</span></span> | <span data-ttu-id="23e10-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23e10-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23e10-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="23e10-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}?expand=columns,items(expand=fields)
```

## <a name="request-body"></a><span data-ttu-id="23e10-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="23e10-117">Request body</span></span>

<span data-ttu-id="23e10-118">Bei dieser Methode wird kein Anforderungstext angegeben.</span><span class="sxs-lookup"><span data-stu-id="23e10-118">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="23e10-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="23e10-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="23e10-120">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23e10-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-list" } -->

```http
GET /sites/{site-id}/lists/{list-id}
```

#### <a name="response"></a><span data-ttu-id="23e10-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="23e10-121">Response</span></span>

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

<span data-ttu-id="23e10-122">Mit `select`- und `expand`-Anweisungen können Sie Listen-Metadaten, Spaltendefinitionen und Listenelemente in einer einzigen Anforderung abrufen.</span><span class="sxs-lookup"><span data-stu-id="23e10-122">With `select` and `expand` statements, you can retrieve list metadata, column definitions, and list items in a single request.</span></span>

#### <a name="request"></a><span data-ttu-id="23e10-123">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23e10-123">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-multi-expand" } -->

```http
GET /sites/{site-id}/lists/{list-id}?select=name,lastModifiedDateTime&expand=columns(select=name,description),items(expand=fields(select=Name,Color,Quantity))
```

#### <a name="response"></a><span data-ttu-id="23e10-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="23e10-124">Response</span></span>

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
