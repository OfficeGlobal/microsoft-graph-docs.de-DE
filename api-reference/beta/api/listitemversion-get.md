---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Abrufen einer früheren Version eines Listenelements – SharePoint-API
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a23a8218b2be3ff36d719ee25e6fb0c960c5750f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526256"
---
# <a name="get-a-listitemversion-resource-preview"></a><span data-ttu-id="37b87-102">ListItemVersion-Ressource erhalten (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="37b87-102">Get a ListItemVersion resource (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37b87-103">Rufen Sie die Metadaten für eine bestimmte Version eines [ListItem](../resources/listitem.md) ab.</span><span class="sxs-lookup"><span data-stu-id="37b87-103">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="37b87-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="37b87-104">Permissions</span></span>

<span data-ttu-id="37b87-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37b87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="37b87-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="37b87-107">Permission type</span></span>             | <span data-ttu-id="37b87-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="37b87-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="37b87-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="37b87-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="37b87-110">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37b87-110">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="37b87-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="37b87-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37b87-112">N/V</span><span class="sxs-lookup"><span data-stu-id="37b87-112">n/a</span></span>                                         |
| <span data-ttu-id="37b87-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="37b87-113">Application</span></span>                            | <span data-ttu-id="37b87-114">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37b87-114">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="37b87-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="37b87-115">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="37b87-116">Antwort</span><span class="sxs-lookup"><span data-stu-id="37b87-116">Response</span></span>

<span data-ttu-id="37b87-117">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [ListItemVersion](../resources/listitemversion.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="37b87-117">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="37b87-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="37b87-118">Example</span></span>

<span data-ttu-id="37b87-119">In diesem Beispiel wird eine Version eines listItem abgerufen und die Fields-Auflistung erweitert, um die Werte der Felder im listItem anzufordern.</span><span class="sxs-lookup"><span data-stu-id="37b87-119">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="37b87-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="37b87-120">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="37b87-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="37b87-121">Response</span></span>

<span data-ttu-id="37b87-122">Dadurch wird eine Sammlung von Versionen zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="37b87-122">This returns a collection of versions:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItemVersion", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "id": "1.0",
    "lastModifiedBy": {
    "user": {
        "id": "CE251278-EF9E-4FE5-833C-1D89EEAE68E0",
        "displayName": "Ryan Gregg"
    }
    },
    "lastModifiedDateTime": "2017-09-14T12:34:53.912Z",
    "fields": {  }
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
    "Error: /api-reference/beta/api/listitemversion-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
