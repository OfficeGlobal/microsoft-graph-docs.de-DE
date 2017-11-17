---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Anfordern eines Eintrags aus einer SharePoint-Liste
ms.openlocfilehash: eaa97e169a8fcfdcb676679bb6dedd3a192925d8
ms.sourcegitcommit: 339070a20730bc4d363da7eb346d5f3c1e1d6c3e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/18/2017
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="19ad1-102">Element in einer Liste anfordern</span><span class="sxs-lookup"><span data-stu-id="19ad1-102">Get an item in a list</span></span>

<span data-ttu-id="19ad1-103">Gibt die Metadaten für ein [Element][] in einer [Liste][] zurück.</span><span class="sxs-lookup"><span data-stu-id="19ad1-103">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listItem.md

## <a name="permissions"></a><span data-ttu-id="19ad1-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="19ad1-106">Permissions</span></span>

<span data-ttu-id="19ad1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="19ad1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="19ad1-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="19ad1-109">Permission type</span></span>      | <span data-ttu-id="19ad1-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="19ad1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19ad1-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="19ad1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="19ad1-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19ad1-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="19ad1-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="19ad1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19ad1-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19ad1-114">Not supported.</span></span>    |
|<span data-ttu-id="19ad1-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="19ad1-115">Application</span></span> | <span data-ttu-id="19ad1-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19ad1-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19ad1-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="19ad1-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="19ad1-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="19ad1-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="19ad1-119">Anforderung</span><span class="sxs-lookup"><span data-stu-id="19ad1-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="19ad1-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="19ad1-120">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "d14922d8-43e6-4c8a-b029-e35c5b4e0d63",
  "listItemId": 2,
  "fields": {
    "Name": "Widget",
    "Color": "Blue",
    "Quantity": 2357
    }
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata"
} -->
