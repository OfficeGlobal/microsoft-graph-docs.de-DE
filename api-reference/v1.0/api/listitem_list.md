---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Abrufen von Elementen aus einer SharePoint-Liste
ms.openlocfilehash: ff414159015b4731b76626e309418c32cb6640d4
ms.sourcegitcommit: 339070a20730bc4d363da7eb346d5f3c1e1d6c3e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/18/2017
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="9e6fc-102">Elemente in einer Liste aufzählen</span><span class="sxs-lookup"><span data-stu-id="9e6fc-102">Enumerate items in a list</span></span>

<span data-ttu-id="9e6fc-103">Rufen Sie die Sammlung von [Elementen] [ item] in einer [Liste][] ab.</span><span class="sxs-lookup"><span data-stu-id="9e6fc-103">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listItem.md

## <a name="permissions"></a><span data-ttu-id="9e6fc-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9e6fc-105">Permissions</span></span>

<span data-ttu-id="9e6fc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9e6fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9e6fc-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9e6fc-108">Permission type</span></span>      | <span data-ttu-id="9e6fc-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9e6fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e6fc-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9e6fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9e6fc-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e6fc-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9e6fc-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9e6fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e6fc-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9e6fc-113">Not supported.</span></span>    |
|<span data-ttu-id="9e6fc-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9e6fc-114">Application</span></span> | <span data-ttu-id="9e6fc-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e6fc-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e6fc-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e6fc-116">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="9e6fc-117">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9e6fc-117">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9e6fc-118">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9e6fc-118">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="9e6fc-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="9e6fc-119">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItem)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  "tocPath": "ListItem/Enumerate"
} -->
