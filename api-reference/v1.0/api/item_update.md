# <a name="update-driveitem-properties"></a><span data-ttu-id="4e761-101">DriveItem-Eigenschaften aktualisieren</span><span class="sxs-lookup"><span data-stu-id="4e761-101">Update DriveItem properties</span></span>

<span data-ttu-id="4e761-102">Dient zum Aktualisieren der Metadaten für ein [DriveItem](../resources/driveitem.md) anhand ID oder Pfad.</span><span class="sxs-lookup"><span data-stu-id="4e761-102">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="4e761-103">Sie können die Aktualisierung auch so vornehmen, dass [ein Element](item_move.md) durch Aktualisieren der **parentReference**-Eigenschaft des Elements in ein anderes Element verschoben wird.</span><span class="sxs-lookup"><span data-stu-id="4e761-103">You can also use update to [move an item](item_move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e761-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4e761-104">Prerequisites</span></span>
<span data-ttu-id="4e761-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="4e761-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="4e761-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4e761-106">Files.ReadWrite</span></span>
* <span data-ttu-id="4e761-107">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e761-107">Files.ReadWrite.All</span></span>
* <span data-ttu-id="4e761-108">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e761-108">Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="4e761-109">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e761-109">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="4e761-110">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4e761-110">Request headers</span></span>

| <span data-ttu-id="4e761-111">Name</span><span class="sxs-lookup"><span data-stu-id="4e761-111">Name</span></span>          | <span data-ttu-id="4e761-112">Typ</span><span class="sxs-lookup"><span data-stu-id="4e761-112">Type</span></span>   | <span data-ttu-id="4e761-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e761-113">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4e761-114">if-match</span><span class="sxs-lookup"><span data-stu-id="4e761-114">if-match</span></span>      | <span data-ttu-id="4e761-115">String</span><span class="sxs-lookup"><span data-stu-id="4e761-115">String</span></span> | <span data-ttu-id="4e761-116">Wenn dieser Anforderungsheader enthalten ist und das angegebene etag (oder cTag) nicht mit dem aktuellen etag des Ordners übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e761-116">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e761-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4e761-117">Request body</span></span>
<span data-ttu-id="4e761-p101">Geben Sie im Anforderungstext die Werte für die Eigenschaften an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Um eine optimale Leistung zu erzielen, sollte Ihre App keine Eigenschaften umfassen, die sich nicht geändert haben.</span><span class="sxs-lookup"><span data-stu-id="4e761-p101">In the request body, supply the values for properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="4e761-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e761-121">Response</span></span>

<span data-ttu-id="4e761-122">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die aktualisierte [DriveItem](../resources/driveitem.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e761-122">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e761-123">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4e761-123">Example</span></span>
<span data-ttu-id="4e761-124">In diesem Beispiel wird das driveItem umbenannt.</span><span class="sxs-lookup"><span data-stu-id="4e761-124">This example renames the driveItem.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-file-name.docx"
}
```

##### <a name="response"></a><span data-ttu-id="4e761-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e761-125">Response</span></span>

<span data-ttu-id="4e761-p102">Das folgende Beispiel zeigt die Antwort. Diese Antwort wird zur besseren Lesbarkeit gekürzt.</span><span class="sxs-lookup"><span data-stu-id="4e761-p102">The following example shows the response. This response is truncated for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
    "name": "new-file-name.docx",
    "file": { }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update item"
}-->
