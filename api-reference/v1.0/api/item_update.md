# <a name="update-driveitem-properties"></a><span data-ttu-id="cc453-101">DriveItem-Eigenschaften aktualisieren</span><span class="sxs-lookup"><span data-stu-id="cc453-101">Update DriveItem properties</span></span>

<span data-ttu-id="cc453-102">Dient zum Aktualisieren der Metadaten für ein [DriveItem](../resources/driveitem.md) anhand ID oder Pfad.</span><span class="sxs-lookup"><span data-stu-id="cc453-102">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="cc453-103">Mithilfe dieser API können Sie außerdem [Elemente unter ein anderes übergeordnetes Element verschieben](item_move.md), indem Sie die Eigenschaft **parentReference** des zu verschiebenden Elements aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="cc453-103">You can also use update to [move an item](item_move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc453-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cc453-104">Permissions</span></span>
<span data-ttu-id="cc453-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cc453-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cc453-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cc453-107">Permission type</span></span>      | <span data-ttu-id="cc453-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cc453-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc453-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cc453-109">Delegated (work or school account)</span></span> | <span data-ttu-id="cc453-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc453-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc453-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cc453-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc453-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc453-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc453-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cc453-113">Application</span></span> | <span data-ttu-id="cc453-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc453-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc453-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cc453-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="cc453-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cc453-116">Request headers</span></span>

| <span data-ttu-id="cc453-117">Name</span><span class="sxs-lookup"><span data-stu-id="cc453-117">Name</span></span>          | <span data-ttu-id="cc453-118">Typ</span><span class="sxs-lookup"><span data-stu-id="cc453-118">Type</span></span>   | <span data-ttu-id="cc453-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cc453-119">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cc453-120">if-match</span><span class="sxs-lookup"><span data-stu-id="cc453-120">if-match</span></span>      | <span data-ttu-id="cc453-121">String</span><span class="sxs-lookup"><span data-stu-id="cc453-121">String</span></span> | <span data-ttu-id="cc453-122">Wenn dieser Anforderungsheader enthalten ist und das angegebene etag (oder cTag) nicht mit dem aktuellen etag des Ordners übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cc453-122">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc453-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cc453-123">Request body</span></span>
<span data-ttu-id="cc453-p102">Geben Sie im Anforderungstext die Werte für die Eigenschaften an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Um eine optimale Leistung zu erzielen, sollte Ihre App keine Eigenschaften umfassen, die sich nicht geändert haben.</span><span class="sxs-lookup"><span data-stu-id="cc453-p102">In the request body, supply the values for properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="cc453-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="cc453-127">Response</span></span>

<span data-ttu-id="cc453-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die aktualisierte [DriveItem](../resources/driveitem.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cc453-128">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc453-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cc453-129">Example</span></span>
<span data-ttu-id="cc453-130">In diesem Beispiel wird das driveItem umbenannt.</span><span class="sxs-lookup"><span data-stu-id="cc453-130">This example renames the driveItem.</span></span>

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

##### <a name="response"></a><span data-ttu-id="cc453-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="cc453-131">Response</span></span>

<span data-ttu-id="cc453-p103">Das folgende Beispiel zeigt die Antwort. Diese Antwort wird zur besseren Lesbarkeit gekürzt.</span><span class="sxs-lookup"><span data-stu-id="cc453-p103">The following example shows the response. This response is truncated for readability.</span></span>

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
