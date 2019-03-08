---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Anfordern eines Eintrags aus einer SharePoint-Liste
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: e9d747e5405a5aeaf97dfdf7e9a97f6236164a5a
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480642"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="3c2de-102">Element in einer Liste anfordern</span><span class="sxs-lookup"><span data-stu-id="3c2de-102">Get an item in a list</span></span>

<span data-ttu-id="3c2de-103">Gibt die Metadaten für ein [Element][] in einer [Liste][] zurück.</span><span class="sxs-lookup"><span data-stu-id="3c2de-103">Returns the metadata for an [item][] in a [list][].</span></span>

[Liste]: ../resources/list.md
[list]: ../resources/list.md
[Element]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="3c2de-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3c2de-106">Permissions</span></span>

<span data-ttu-id="3c2de-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c2de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c2de-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3c2de-109">Permission type</span></span>      | <span data-ttu-id="3c2de-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3c2de-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c2de-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3c2de-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3c2de-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c2de-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3c2de-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3c2de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c2de-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3c2de-114">Not supported.</span></span>    |
|<span data-ttu-id="3c2de-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3c2de-115">Application</span></span> | <span data-ttu-id="3c2de-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c2de-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c2de-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3c2de-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="3c2de-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3c2de-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3c2de-119">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3c2de-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item", "scopes": "sites.read.all" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="3c2de-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="3c2de-120">Response</span></span>

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
