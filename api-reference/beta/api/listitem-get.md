---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: Anfordern eines Eintrags aus einer SharePoint-Liste
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 60a413060a3b86264cd1b1ae1a2fbc632c98e7bf
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481244"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="4b49c-102">Element in einer Liste anfordern</span><span class="sxs-lookup"><span data-stu-id="4b49c-102">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b49c-103">Gibt die Metadaten für ein [Element][] in einer [Liste][] zurück.</span><span class="sxs-lookup"><span data-stu-id="4b49c-103">Returns the metadata for an [item][] in a [list][].</span></span>

[Liste]: ../resources/list.md
[list]: ../resources/list.md
[Element]: ../resources/listitem.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="4b49c-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4b49c-106">Permissions</span></span>

<span data-ttu-id="4b49c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b49c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b49c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4b49c-109">Permission type</span></span>      | <span data-ttu-id="4b49c-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4b49c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b49c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4b49c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4b49c-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b49c-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4b49c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4b49c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b49c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b49c-114">Not supported.</span></span>    |
|<span data-ttu-id="4b49c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4b49c-115">Application</span></span> | <span data-ttu-id="4b49c-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b49c-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4b49c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b49c-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="4b49c-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b49c-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4b49c-119">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b49c-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="4b49c-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b49c-120">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Get metadata",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
