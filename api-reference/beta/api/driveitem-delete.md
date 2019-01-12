---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Eine Datei oder einen Ordner löschen
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 40b29bee213da3693917a37b14368112ea295c12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926239"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="c6b76-102">Ein DriveItem-Element löschen</span><span class="sxs-lookup"><span data-stu-id="c6b76-102">Delete a DriveItem</span></span>

> <span data-ttu-id="c6b76-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c6b76-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6b76-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c6b76-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c6b76-p102">Löscht ein [DriveItem](../resources/driveitem.md)-Element mithilfe der ID oder des Pfad. Beachten Sie, dass durch Löschen von Elementen mithilfe dieser Methode die Elemente in den Papierkorb verschoben und nicht endgültig gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="c6b76-p102">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6b76-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c6b76-107">Permissions</span></span>

<span data-ttu-id="c6b76-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6b76-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6b76-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c6b76-110">Permission type</span></span>      | <span data-ttu-id="c6b76-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c6b76-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6b76-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c6b76-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c6b76-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6b76-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c6b76-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c6b76-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6b76-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6b76-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c6b76-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c6b76-116">Application</span></span> | <span data-ttu-id="c6b76-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6b76-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6b76-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6b76-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="c6b76-119">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c6b76-119">Optional request headers</span></span>

| <span data-ttu-id="c6b76-120">Name</span><span class="sxs-lookup"><span data-stu-id="c6b76-120">Name</span></span>          | <span data-ttu-id="c6b76-121">Typ</span><span class="sxs-lookup"><span data-stu-id="c6b76-121">Type</span></span>   | <span data-ttu-id="c6b76-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6b76-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c6b76-123">if-match</span><span class="sxs-lookup"><span data-stu-id="c6b76-123">if-match</span></span>      | <span data-ttu-id="c6b76-124">String</span><span class="sxs-lookup"><span data-stu-id="c6b76-124">String</span></span> | <span data-ttu-id="c6b76-125">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="c6b76-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="c6b76-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c6b76-126">Example</span></span>

<span data-ttu-id="c6b76-127">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="c6b76-127">Here is an example of how to call this API.</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE /me/drive/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="c6b76-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6b76-128">Response</span></span>

<span data-ttu-id="c6b76-129">Bei erfolgreicher Ausführung gibt dieser Aufruf eine Antwort des Typs `204 No Content` zurück, die angibt, dass die Ressource gelöscht wurde und daher keine Ressource zurückgegeben werden kann.</span><span class="sxs-lookup"><span data-stu-id="c6b76-129">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a><span data-ttu-id="c6b76-130">Fehlerantworten</span><span class="sxs-lookup"><span data-stu-id="c6b76-130">Error responses</span></span>

<span data-ttu-id="c6b76-131">Weitere Informationen dazu, wie Fehler zurückgegeben werden, finden Sie unter [Fehlerantworten][error-response].</span><span class="sxs-lookup"><span data-stu-id="c6b76-131">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete"
} -->
