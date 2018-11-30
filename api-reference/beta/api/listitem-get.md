---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Anfordern eines Eintrags aus einer SharePoint-Liste
ms.openlocfilehash: 240f9f285178407f167cfb66b790224aa24c35d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063491"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="d9aa0-102">Element in einer Liste anfordern</span><span class="sxs-lookup"><span data-stu-id="d9aa0-102">Get an item in a list</span></span>

> <span data-ttu-id="d9aa0-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d9aa0-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9aa0-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d9aa0-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9aa0-105">Gibt die Metadaten für ein [Element][] in einer [Liste][] zurück.</span><span class="sxs-lookup"><span data-stu-id="d9aa0-105">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[Element]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="d9aa0-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d9aa0-108">Permissions</span></span>

<span data-ttu-id="d9aa0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9aa0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9aa0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d9aa0-111">Permission type</span></span>      | <span data-ttu-id="d9aa0-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d9aa0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9aa0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d9aa0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d9aa0-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9aa0-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d9aa0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d9aa0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9aa0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d9aa0-116">Not supported.</span></span>    |
|<span data-ttu-id="d9aa0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d9aa0-117">Application</span></span> | <span data-ttu-id="d9aa0-118">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9aa0-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9aa0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9aa0-119">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="d9aa0-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d9aa0-120">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d9aa0-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d9aa0-121">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="d9aa0-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="d9aa0-122">Response</span></span>

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