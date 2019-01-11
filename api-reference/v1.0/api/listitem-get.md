---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Anfordern eines Eintrags aus einer SharePoint-Liste
localization_priority: Priority
ms.openlocfilehash: ab263c074497d43bb03ea7c69748bb1c64fd9425
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881130"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="57177-102">Element in einer Liste anfordern</span><span class="sxs-lookup"><span data-stu-id="57177-102">Get an item in a list</span></span>

<span data-ttu-id="57177-103">Gibt die Metadaten für ein [Element][] in einer [Liste][] zurück.</span><span class="sxs-lookup"><span data-stu-id="57177-103">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[Element]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="57177-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="57177-106">Permissions</span></span>

<span data-ttu-id="57177-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57177-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57177-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="57177-109">Permission type</span></span>      | <span data-ttu-id="57177-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="57177-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57177-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="57177-111">Delegated (work or school account)</span></span> | <span data-ttu-id="57177-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57177-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="57177-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="57177-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57177-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57177-114">Not supported.</span></span>    |
|<span data-ttu-id="57177-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="57177-115">Application</span></span> | <span data-ttu-id="57177-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57177-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57177-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="57177-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="57177-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="57177-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="57177-119">Anforderung</span><span class="sxs-lookup"><span data-stu-id="57177-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="57177-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="57177-120">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "5",
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
