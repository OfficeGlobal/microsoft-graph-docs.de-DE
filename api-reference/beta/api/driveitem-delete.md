---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Eine Datei oder einen Ordner löschen
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5317cee9288bb4a78b66d497b4a4b58f945c9198
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529019"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="c860a-102">Ein DriveItem-Element löschen</span><span class="sxs-lookup"><span data-stu-id="c860a-102">Delete a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c860a-p101">Löscht ein [DriveItem](../resources/driveitem.md)-Element mithilfe der ID oder des Pfad. Beachten Sie, dass durch Löschen von Elementen mithilfe dieser Methode die Elemente in den Papierkorb verschoben und nicht endgültig gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="c860a-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="c860a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c860a-105">Permissions</span></span>

<span data-ttu-id="c860a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c860a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c860a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c860a-108">Permission type</span></span>      | <span data-ttu-id="c860a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c860a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c860a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c860a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c860a-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c860a-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c860a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c860a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c860a-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c860a-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c860a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c860a-114">Application</span></span> | <span data-ttu-id="c860a-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c860a-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c860a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c860a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="c860a-117">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c860a-117">Optional request headers</span></span>

| <span data-ttu-id="c860a-118">Name</span><span class="sxs-lookup"><span data-stu-id="c860a-118">Name</span></span>          | <span data-ttu-id="c860a-119">Typ</span><span class="sxs-lookup"><span data-stu-id="c860a-119">Type</span></span>   | <span data-ttu-id="c860a-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c860a-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c860a-121">if-match</span><span class="sxs-lookup"><span data-stu-id="c860a-121">if-match</span></span>      | <span data-ttu-id="c860a-122">String</span><span class="sxs-lookup"><span data-stu-id="c860a-122">String</span></span> | <span data-ttu-id="c860a-123">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="c860a-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="c860a-124">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c860a-124">Example</span></span>

<span data-ttu-id="c860a-125">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c860a-125">Here is an example of how to call this API.</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE /me/drive/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="c860a-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="c860a-126">Response</span></span>

<span data-ttu-id="c860a-127">Bei erfolgreicher Ausführung gibt dieser Aufruf eine Antwort des Typs `204 No Content` zurück, die angibt, dass die Ressource gelöscht wurde und daher keine Ressource zurückgegeben werden kann.</span><span class="sxs-lookup"><span data-stu-id="c860a-127">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a><span data-ttu-id="c860a-128">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="c860a-128">Error responses</span></span>

<span data-ttu-id="c860a-129">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="c860a-129">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
