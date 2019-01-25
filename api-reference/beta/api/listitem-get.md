---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Anfordern eines Eintrags aus einer SharePoint-Liste
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 248208542b954c11992908529d4f21a9b7d96673
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512192"
---
# <a name="get-an-item-in-a-list"></a><span data-ttu-id="64fdb-102">Element in einer Liste anfordern</span><span class="sxs-lookup"><span data-stu-id="64fdb-102">Get an item in a list</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64fdb-103">Gibt die Metadaten für ein [Element][] in einer [Liste][] zurück.</span><span class="sxs-lookup"><span data-stu-id="64fdb-103">Returns the metadata for an [item][] in a [list][].</span></span>

[list]: ../resources/list.md
[item]: ../resources/listitem.md

## <a name="permissions"></a><span data-ttu-id="64fdb-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="64fdb-106">Permissions</span></span>

<span data-ttu-id="64fdb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64fdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64fdb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="64fdb-109">Permission type</span></span>      | <span data-ttu-id="64fdb-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="64fdb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64fdb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="64fdb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="64fdb-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64fdb-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="64fdb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="64fdb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64fdb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="64fdb-114">Not supported.</span></span>    |
|<span data-ttu-id="64fdb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="64fdb-115">Application</span></span> | <span data-ttu-id="64fdb-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64fdb-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64fdb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="64fdb-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields(select=Column1,Column2)
```

## <a name="example"></a><span data-ttu-id="64fdb-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="64fdb-118">Example</span></span>

##### <a name="request"></a><span data-ttu-id="64fdb-119">Anforderung</span><span class="sxs-lookup"><span data-stu-id="64fdb-119">Request</span></span>

<!-- { "blockType": "request", "name": "get-list-item" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}?expand=fields
```

##### <a name="response"></a><span data-ttu-id="64fdb-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="64fdb-120">Response</span></span>

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
