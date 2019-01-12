---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Abrufen einer früheren Version eines SharePoint-Listendatensatzes
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 8b8e6a1b49a5e1ab387f18fecb98212dbbc975f6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954351"
---
# <a name="listing-versions-of-a-listitem-preview"></a><span data-ttu-id="b8fef-102">Auflisten von ListItem-Versionen (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="b8fef-102">Listing versions of a ListItem (preview)</span></span>

> <span data-ttu-id="b8fef-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b8fef-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8fef-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8fef-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8fef-105">SharePoint kann auch so konfiguriert werden, dass für Listenelemente ein Verlauf beibehalten wird.</span><span class="sxs-lookup"><span data-stu-id="b8fef-105">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="b8fef-106">Vorherige Versionen können je nach Administratoreinstellungen für einen begrenzten Zeitraum beibehalten werden, diese können pro Benutzer oder Speicherort eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="b8fef-106">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8fef-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b8fef-107">Permissions</span></span>

<span data-ttu-id="b8fef-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8fef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="b8fef-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8fef-110">Permission type</span></span>             | <span data-ttu-id="b8fef-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8fef-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="b8fef-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8fef-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b8fef-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8fef-113">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="b8fef-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8fef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8fef-115">N/V</span><span class="sxs-lookup"><span data-stu-id="b8fef-115">n/a</span></span>                                         |
| <span data-ttu-id="b8fef-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8fef-116">Application</span></span>                            | <span data-ttu-id="b8fef-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8fef-117">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="b8fef-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8fef-118">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="b8fef-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8fef-119">Response</span></span>

<span data-ttu-id="b8fef-120">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [ListItemVersion](../resources/listitemversion.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8fef-120">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="b8fef-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8fef-121">Example</span></span>

<span data-ttu-id="b8fef-122">In diesem Beispiel werden die Versionen eines ListItem in einer SharePoint-Liste abgerufen:</span><span class="sxs-lookup"><span data-stu-id="b8fef-122">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="b8fef-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8fef-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="b8fef-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8fef-124">Response</span></span>

<span data-ttu-id="b8fef-125">Dadurch wird eine Sammlung von Versionen zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="b8fef-125">This returns a collection of versions:</span></span>

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
