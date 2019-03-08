---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Abrufen einer früheren Version eines SharePoint-Listendatensatzes
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: b8a9078bb0e56f3c3068a92bab9835f2a4964f79
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481342"
---
# <a name="listing-versions-of-a-listitem-preview"></a><span data-ttu-id="c7fda-102">Auflisten von ListItem-Versionen (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="c7fda-102">Listing versions of a ListItem (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7fda-103">SharePoint kann auch so konfiguriert werden, dass für Listenelemente ein Verlauf beibehalten wird.</span><span class="sxs-lookup"><span data-stu-id="c7fda-103">SharePoint can be configured to retain the history for list items.</span></span>

<span data-ttu-id="c7fda-104">Vorherige Versionen können je nach Administratoreinstellungen für einen begrenzten Zeitraum beibehalten werden, diese können pro Benutzer oder Speicherort eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="c7fda-104">Previous versions may be retained for a finite period of time depending on admin settings which may be unique per user or location.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7fda-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c7fda-105">Permissions</span></span>

<span data-ttu-id="c7fda-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7fda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="c7fda-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c7fda-108">Permission type</span></span>             | <span data-ttu-id="c7fda-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c7fda-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c7fda-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c7fda-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7fda-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7fda-111">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="c7fda-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c7fda-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7fda-113">N/V</span><span class="sxs-lookup"><span data-stu-id="c7fda-113">n/a</span></span>                                         |
| <span data-ttu-id="c7fda-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c7fda-114">Application</span></span>                            | <span data-ttu-id="c7fda-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7fda-115">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="c7fda-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7fda-116">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions
```

## <a name="response"></a><span data-ttu-id="c7fda-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7fda-117">Response</span></span>

<span data-ttu-id="c7fda-118">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [ListItemVersion](../resources/listitemversion.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c7fda-118">If successful, this method returns a `200 OK` response code and collection of [ListItemVersion](../resources/listitemversion.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="c7fda-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c7fda-119">Example</span></span>

<span data-ttu-id="c7fda-120">In diesem Beispiel werden die Versionen eines ListItem in einer SharePoint-Liste abgerufen:</span><span class="sxs-lookup"><span data-stu-id="c7fda-120">This example retrieves the versions of a listItem in a SharePoint list:</span></span>

### <a name="http-request"></a><span data-ttu-id="c7fda-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7fda-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-previous-versions-listitem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions
```

### <a name="response"></a><span data-ttu-id="c7fda-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7fda-122">Response</span></span>

<span data-ttu-id="c7fda-123">Dadurch wird eine Sammlung von Versionen zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="c7fda-123">This returns a collection of versions:</span></span>

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


<!--
{
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history",
  "suppressions": [
    "Error: /api-reference/beta/api/listitem-list-versions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
