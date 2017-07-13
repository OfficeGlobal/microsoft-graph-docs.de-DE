<span data-ttu-id="7b5bd-p101">Löscht ein [DriveItem](../resources/driveitem.md)-Element mithilfe der ID oder des Pfad. Beachten Sie, dass durch Löschen von Elementen mithilfe dieser Methode die Elemente in den Papierkorb verschoben und nicht endgültig gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="7b5bd-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

Löscht ein [DriveItem](../resources/driveitem.md)-Element mithilfe der ID oder des Pfad. Beachten Sie, dass durch Löschen von Elementen mithilfe dieser Methode die Elemente in den Papierkorb verschoben und nicht endgültig gelöscht werden.

## <span data-ttu-id="7b5bd-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7b5bd-104">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>
<span data-ttu-id="7b5bd-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="7b5bd-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="7b5bd-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7b5bd-106">Files.ReadWrite</span></span>
* <span data-ttu-id="7b5bd-107">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b5bd-107">Files.ReadWrite.All</span></span>
* <span data-ttu-id="7b5bd-108">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b5bd-108">Sites.ReadWrite.All</span></span>

## <span data-ttu-id="7b5bd-109">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b5bd-109">HTTP request</span></span>
<a id="http-request" class="xliff"></a>

<!-- { "blockType": "ignored" } -->
```
DELETE /me/drive/items/{item-id}
DELETE /me/drive/root:/{item-path}
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
```

## <span data-ttu-id="7b5bd-110">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b5bd-110">Request headers</span></span>
<a id="request-headers" class="xliff"></a>

| <span data-ttu-id="7b5bd-111">Name</span><span class="sxs-lookup"><span data-stu-id="7b5bd-111">Name</span></span>          | <span data-ttu-id="7b5bd-112">Typ</span><span class="sxs-lookup"><span data-stu-id="7b5bd-112">Type</span></span>   | <span data-ttu-id="7b5bd-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b5bd-113">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7b5bd-114">if-match</span><span class="sxs-lookup"><span data-stu-id="7b5bd-114">if-match</span></span>      | <span data-ttu-id="7b5bd-115">String</span><span class="sxs-lookup"><span data-stu-id="7b5bd-115">String</span></span> | <span data-ttu-id="7b5bd-116">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="7b5bd-116">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <span data-ttu-id="7b5bd-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b5bd-117">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="7b5bd-118">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7b5bd-118">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="7b5bd-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b5bd-119">Example</span></span>
<a id="example" class="xliff"></a>

<span data-ttu-id="7b5bd-120">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="7b5bd-120">Here is an example of how to call this API.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-item"
}-->
```
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
```

## <span data-ttu-id="7b5bd-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b5bd-121">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="7b5bd-122">Wenn die Methode erfolgreich verläuft, wird die Antwort `204 No Content` zurückgegeben, um anzugeben, dass die Ressource gelöscht wurde und keine Werte zum Zurückgeben vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="7b5bd-122">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete item"
}-->
