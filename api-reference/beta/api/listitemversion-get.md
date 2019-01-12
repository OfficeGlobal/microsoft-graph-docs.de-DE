---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Abrufen einer früheren Version eines Listenelements – SharePoint-API
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4068ebd1e8a245f2418954ce04bad1f78530acd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983877"
---
# <a name="get-a-listitemversion-resource-preview"></a><span data-ttu-id="34f35-102">ListItemVersion-Ressource erhalten (Vorschau)</span><span class="sxs-lookup"><span data-stu-id="34f35-102">Get a ListItemVersion resource (preview)</span></span>

> <span data-ttu-id="34f35-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="34f35-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34f35-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34f35-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34f35-105">Rufen Sie die Metadaten für eine bestimmte Version eines [ListItem](../resources/listitem.md) ab.</span><span class="sxs-lookup"><span data-stu-id="34f35-105">Retrieve the metadata for a specific version of a [ListItem](../resources/listitem.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="34f35-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="34f35-106">Permissions</span></span>

<span data-ttu-id="34f35-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34f35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|            <span data-ttu-id="34f35-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="34f35-109">Permission type</span></span>             | <span data-ttu-id="34f35-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="34f35-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="34f35-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="34f35-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="34f35-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34f35-112">Sites.Read.All, Sites.ReadWrite.All</span></span>         |
| <span data-ttu-id="34f35-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="34f35-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34f35-114">N/V</span><span class="sxs-lookup"><span data-stu-id="34f35-114">n/a</span></span>                                         |
| <span data-ttu-id="34f35-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="34f35-115">Application</span></span>                            | <span data-ttu-id="34f35-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34f35-116">Sites.Read.All, Sites.ReadWrite.All</span></span>         |


## <a name="http-request"></a><span data-ttu-id="34f35-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="34f35-117">HTTP request</span></span>

<!-- { "blockType": "ignored"} -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}
GET /sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}
```


## <a name="response"></a><span data-ttu-id="34f35-118">Antwort</span><span class="sxs-lookup"><span data-stu-id="34f35-118">Response</span></span>

<span data-ttu-id="34f35-119">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [ListItemVersion](../resources/listitemversion.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="34f35-119">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/listitemversion.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="34f35-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="34f35-120">Example</span></span>

<span data-ttu-id="34f35-121">In diesem Beispiel wird eine Version eines listItem abgerufen und die Fields-Auflistung erweitert, um die Werte der Felder im listItem anzufordern.</span><span class="sxs-lookup"><span data-stu-id="34f35-121">This example retrieves a version of a listItem and expands the fields collection to request the values of fields in the listItem.</span></span>

### <a name="http-request"></a><span data-ttu-id="34f35-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="34f35-122">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-single-version-listItem", "scopes": "files.read" } -->

```http
GET /sites/{site-id}/items/{item-id}/versions/{version-id}?expand=fields
```

### <a name="response"></a><span data-ttu-id="34f35-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="34f35-123">Response</span></span>

<span data-ttu-id="34f35-124">Dadurch wird eine Sammlung von Versionen zurückgegeben:</span><span class="sxs-lookup"><span data-stu-id="34f35-124">This returns a collection of versions:</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "List, review, and download previous versions of a driveItem",
  "keywords": "version, version history, versions",
  "section": "documentation",
  "tocPath": "Items/Version history"
} -->
