---
title: Auflisten von einer ListItem-Versionen
description: SharePoint kann auch so konfiguriert werden, dass für Listenelemente ein Verlauf beibehalten wird.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 0da37c65c4f7cf737d7e37b0ed50305aa19b3e53
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921374"
---
# <a name="listing-versions-of-a-listitem"></a><span data-ttu-id="25526-103">Auflisten von einer ListItem-Versionen</span><span class="sxs-lookup"><span data-stu-id="25526-103">Listing versions of a ListItem</span></span>

<span data-ttu-id="25526-104">SharePoint kann auch so konfiguriert werden, dass für Listenelemente ein Verlauf beibehalten wird.</span><span class="sxs-lookup"><span data-stu-id="25526-104">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="25526-105">Vorherige Versionen können je nach Administratoreinstellungen für einen begrenzten Zeitraum beibehalten werden, diese können pro Benutzer oder Speicherort eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="25526-105">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="25526-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="25526-106">Permissions</span></span>

<span data-ttu-id="25526-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25526-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="25526-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="25526-109">Permission type</span></span>             | <span data-ttu-id="25526-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="25526-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="25526-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="25526-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="25526-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25526-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="25526-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="25526-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25526-114">N/V</span><span class="sxs-lookup"><span data-stu-id="25526-114">n/a</span></span>                                         |
| <span data-ttu-id="25526-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="25526-115">Application</span></span>                            | <span data-ttu-id="25526-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25526-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="25526-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="25526-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="25526-118">Antwort</span><span class="sxs-lookup"><span data-stu-id="25526-118">Response</span></span>

<span data-ttu-id="25526-119">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [ListItemVersion](../resources/listitemversion.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="25526-119">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="25526-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="25526-120">Example</span></span>

<span data-ttu-id="25526-121">In diesem Beispiel werden die Versionen eines ListItem in einer SharePoint-Liste abgerufen:</span><span class="sxs-lookup"><span data-stu-id="25526-121">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="25526-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="25526-122">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read sites.read.all" } -->

```http
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="25526-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="25526-123">Response</span></span>

<span data-ttu-id="25526-124">Dadurch wird eine Sammlung von Versionen zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="25526-124">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.listItemVersion)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value":
  [
    {
      "id": "3.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-14T12:34:53.912Z"
    },
    {
      "id": "2.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-11T10:21:03.000Z"
    },
    {
      "id": "1.0",
      "lastModifiedBy": {
        "user": {
          "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
          "displayName": "Ryan Gregg"
        }
      },
      "lastModifiedDateTime": "2017-09-10T15:20:01.125Z"
    }
  ]
}
```


<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
