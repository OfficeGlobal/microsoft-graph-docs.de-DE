# <a name="move-a-driveitem"></a><span data-ttu-id="4b344-101">DriveItem-Element verschieben</span><span class="sxs-lookup"><span data-stu-id="4b344-101">Move a DriveItem</span></span>

<span data-ttu-id="4b344-p101">Zum Verschieben eines DriveItem-Elements zu einem neuen übergeordneten Element fordert die App die Aktualisierung von **ParentReference** des zu verschiebenden DriveItem-Elements an. Dies ist ein Sonderfall der [Update](item_update.md)-Methode. Die App kann das Verschieben eines Elements zu einem neuen Container und das Aktualisieren anderer Eigenschaften des Elements in einer einzigen Anforderung verbinden.</span><span class="sxs-lookup"><span data-stu-id="4b344-p101">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move. This is a special case of the [Update](item_update.md) method. Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="4b344-105">Elemente können mit dieser Anforderung nicht zwischen [Laufwerken](../resources/drive.md)  verschoben werden.</span><span class="sxs-lookup"><span data-stu-id="4b344-105">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b344-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4b344-106">Prerequisites</span></span>
<span data-ttu-id="4b344-107">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="4b344-107">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="4b344-108">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4b344-108">Files.ReadWrite</span></span>
* <span data-ttu-id="4b344-109">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b344-109">Files.ReadWrite.All</span></span>
* <span data-ttu-id="4b344-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b344-110">Sites.ReadWrite.All</span></span>


## <a name="http-request"></a><span data-ttu-id="4b344-111">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b344-111">HTTP request</span></span>

```http
PATCH /me/drive/items/{item-id}
PATCH /me/drive/root:/{item-path}
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="4b344-112">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4b344-112">Request headers</span></span>

| <span data-ttu-id="4b344-113">Name</span><span class="sxs-lookup"><span data-stu-id="4b344-113">Name</span></span>          | <span data-ttu-id="4b344-114">Typ</span><span class="sxs-lookup"><span data-stu-id="4b344-114">Type</span></span>   | <span data-ttu-id="4b344-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b344-115">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4b344-116">if-match</span><span class="sxs-lookup"><span data-stu-id="4b344-116">if-match</span></span>      | <span data-ttu-id="4b344-117">String</span><span class="sxs-lookup"><span data-stu-id="4b344-117">String</span></span> | <span data-ttu-id="4b344-118">Wenn dieser Anforderungsheader enthalten ist und das angegebene etag (oder cTag) nicht mit dem aktuellen etag des Ordners übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b344-118">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4b344-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4b344-119">Request body</span></span>
<span data-ttu-id="4b344-p102">Geben Sie im Anforderungstext den neuen Wert für die **parentReference**-Eigenschaft an. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="4b344-p102">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="4b344-p103">**Hinweis:** Die `"id:" "root"`-Syntax kann nicht beim Verschieben von Elementen in den Stammordner einer OneDrive-Umgebung verwendet werden. Sie müssen entweder die echte ID des Stammordners oder `{"path": "/drive/root"}` für die übergeordnete Referenz verwenden.</span><span class="sxs-lookup"><span data-stu-id="4b344-p103">**Note:** When moving items to the root of a OneDrive you cannot use the `"id:" "root"` syntax. You either need to use the real ID of the root folder, or use `{"path": "/drive/root"}` for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="4b344-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b344-125">Response</span></span>

<span data-ttu-id="4b344-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die aktualisierte [DriveItem](../resources/driveitem.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b344-126">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b344-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b344-127">Example</span></span>
<span data-ttu-id="4b344-128">In diesem Beispiel wird ein durch {item-id} angegebenes Element in den Ordner **Dokumente** in der OneDrive-Umgebung des Benutzers verschoben.</span><span class="sxs-lookup"><span data-stu-id="4b344-128">This example moves an item specified by {item-id} into the **Documents** folder in the user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_item"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}
Content-type: application/json

{
    "name": "new-item-name",
    "parentReference" : {"path": "/drive/root:/Documents"}
}
```

##### <a name="response"></a><span data-ttu-id="4b344-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b344-129">Response</span></span>

<span data-ttu-id="4b344-130">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="4b344-130">The following example shows an Autodiscover error response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0123456789abc",
    "name": "new-item-name",
    "folder": { "childCount": 3 },
  "parentReference": {
    "id": "507DE6D5-0201-496A-AA87-5E2563247982",
    "path": "/drive/root:/Documents"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Move item",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
