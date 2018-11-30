---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Abrufen von Elementen aus einer SharePoint-Liste
ms.openlocfilehash: 3c6a8259f17091612cf10e1501a24d9eb60e28d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059415"
---
# <a name="enumerate-items-in-a-list"></a><span data-ttu-id="78474-102">Elemente in einer Liste aufzählen</span><span class="sxs-lookup"><span data-stu-id="78474-102">Enumerate items in a list</span></span>

> <span data-ttu-id="78474-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="78474-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78474-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="78474-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78474-105">Rufen Sie die Sammlung von [Elementen] [ item] in einer [Liste][] ab.</span><span class="sxs-lookup"><span data-stu-id="78474-105">Get the collection of [items][item] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="78474-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="78474-107">Permissions</span></span>

<span data-ttu-id="78474-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78474-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78474-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="78474-110">Permission type</span></span>      | <span data-ttu-id="78474-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="78474-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78474-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="78474-112">Delegated (work or school account)</span></span> | <span data-ttu-id="78474-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78474-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="78474-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="78474-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78474-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="78474-115">Not supported.</span></span>    |
|<span data-ttu-id="78474-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="78474-116">Application</span></span> | <span data-ttu-id="78474-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78474-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="78474-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="78474-118">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="78474-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="78474-119">Example</span></span>

#### <a name="request"></a><span data-ttu-id="78474-120">Anforderung</span><span class="sxs-lookup"><span data-stu-id="78474-120">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-items" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Name,Color,Quantity)
```

#### <a name="response"></a><span data-ttu-id="78474-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="78474-121">Response</span></span>

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
