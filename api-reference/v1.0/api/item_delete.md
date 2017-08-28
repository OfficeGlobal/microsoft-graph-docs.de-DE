# <a name="delete-a-driveitem"></a><span data-ttu-id="51224-101">Ein DriveItem-Element löschen</span><span class="sxs-lookup"><span data-stu-id="51224-101">Delete a DriveItem</span></span>

<span data-ttu-id="51224-p101">Löscht ein [DriveItem](../resources/driveitem.md)-Element mithilfe der ID oder des Pfad. Beachten Sie, dass durch Löschen von Elementen mithilfe dieser Methode die Elemente in den Papierkorb verschoben und nicht endgültig gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="51224-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="51224-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="51224-104">Permissions</span></span>
<span data-ttu-id="51224-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="51224-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="51224-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="51224-107">Permission type</span></span>      | <span data-ttu-id="51224-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="51224-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51224-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="51224-109">Delegated (work or school account)</span></span> | <span data-ttu-id="51224-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51224-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="51224-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="51224-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51224-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51224-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="51224-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="51224-113">Application</span></span> | <span data-ttu-id="51224-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51224-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51224-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="51224-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```
DELETE /me/drive/items/{item-id}
DELETE /me/drive/root:/{item-path}
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="51224-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="51224-116">Request headers</span></span>

| <span data-ttu-id="51224-117">Name</span><span class="sxs-lookup"><span data-stu-id="51224-117">Name</span></span>          | <span data-ttu-id="51224-118">Typ</span><span class="sxs-lookup"><span data-stu-id="51224-118">Type</span></span>   | <span data-ttu-id="51224-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51224-119">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="51224-120">if-match</span><span class="sxs-lookup"><span data-stu-id="51224-120">if-match</span></span>      | <span data-ttu-id="51224-121">String</span><span class="sxs-lookup"><span data-stu-id="51224-121">String</span></span> | <span data-ttu-id="51224-122">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="51224-122">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51224-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="51224-123">Request body</span></span>
<span data-ttu-id="51224-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="51224-124">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="51224-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="51224-125">Example</span></span>

<span data-ttu-id="51224-126">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="51224-126">Here is an example of how to call this API.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-item"
}-->
```
DELETE https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="51224-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="51224-127">Response</span></span>

<span data-ttu-id="51224-128">Wenn die Methode erfolgreich verläuft, wird die Antwort `204 No Content` zurückgegeben, um anzugeben, dass die Ressource gelöscht wurde und keine Werte zum Zurückgeben vorhanden waren.</span><span class="sxs-lookup"><span data-stu-id="51224-128">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

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
