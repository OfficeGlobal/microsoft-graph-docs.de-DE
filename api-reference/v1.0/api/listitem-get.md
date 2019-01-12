---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Anfordern eines Eintrags aus einer SharePoint-Liste
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 1a1117717a0afc0d715da2297d69b0453ef2025e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950543"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="98d3d-102">Element in einer Liste anfordern</span><span class="sxs-lookup"><span data-stu-id="98d3d-102">Get an item in a list</span></span>

<span data-ttu-id="98d3d-103">Gibt die Metadaten für ein [Element][] in einer [Liste][] zurück.</span><span class="sxs-lookup"><span data-stu-id="98d3d-103">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[Element]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="98d3d-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="98d3d-106">Permissions</span></span>

<span data-ttu-id="98d3d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98d3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98d3d-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="98d3d-109">Permission type</span></span>      | <span data-ttu-id="98d3d-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="98d3d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98d3d-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="98d3d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="98d3d-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98d3d-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="98d3d-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="98d3d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98d3d-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="98d3d-114">Not supported.</span></span>    |
|<span data-ttu-id="98d3d-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="98d3d-115">Application</span></span> | <span data-ttu-id="98d3d-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98d3d-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98d3d-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="98d3d-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="98d3d-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="98d3d-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="98d3d-119">Anforderung</span><span class="sxs-lookup"><span data-stu-id="98d3d-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="98d3d-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="98d3d-120">Response</span></span>

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
