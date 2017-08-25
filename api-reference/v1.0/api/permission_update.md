# <a name="update-permission"></a><span data-ttu-id="d1046-101">Berechtigung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d1046-101">Update permission</span></span>

<span data-ttu-id="d1046-102">Über diese API können Sie die Eigenschaften einer Berechtigung aktualisieren, indem Sie einen Patch auf die betreffende Ressource anwenden.</span><span class="sxs-lookup"><span data-stu-id="d1046-102">Update the properties of a permission by patching the resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1046-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d1046-103">Permissions</span></span>

<span data-ttu-id="d1046-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d1046-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d1046-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d1046-106">Permission type</span></span>      | <span data-ttu-id="d1046-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d1046-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="d1046-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d1046-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d1046-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1046-109">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="d1046-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d1046-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1046-111">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1046-111">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="d1046-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d1046-112">Application</span></span> | <span data-ttu-id="d1046-113">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1046-113">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d1046-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1046-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/items/{item-id}/permissions/{perm-id}
PATCH /me/drive/root:/{path}:/permissions/{perm-id}
PATCH /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
PATCH /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="request-headers"></a><span data-ttu-id="d1046-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d1046-115">Request headers</span></span>

| <span data-ttu-id="d1046-116">Name</span><span class="sxs-lookup"><span data-stu-id="d1046-116">Name</span></span>          | <span data-ttu-id="d1046-117">Typ</span><span class="sxs-lookup"><span data-stu-id="d1046-117">Type</span></span>   | <span data-ttu-id="d1046-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1046-118">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d1046-119">if-match</span><span class="sxs-lookup"><span data-stu-id="d1046-119">if-match</span></span>      | <span data-ttu-id="d1046-120">string</span><span class="sxs-lookup"><span data-stu-id="d1046-120">string</span></span> | <span data-ttu-id="d1046-121">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="d1046-121">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d1046-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d1046-122">Request body</span></span>
<span data-ttu-id="d1046-p102">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="d1046-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d1046-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d1046-126">Property</span></span>     | <span data-ttu-id="d1046-127">Typ</span><span class="sxs-lookup"><span data-stu-id="d1046-127">Type</span></span>   | <span data-ttu-id="d1046-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1046-128">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="d1046-129">**roles**</span><span class="sxs-lookup"><span data-stu-id="d1046-129">**roles**</span></span>    | <span data-ttu-id="d1046-130">String</span><span class="sxs-lookup"><span data-stu-id="d1046-130">String</span></span> | <span data-ttu-id="d1046-131">Ein Array von Berechtigungstypen.</span><span class="sxs-lookup"><span data-stu-id="d1046-131">An array of permission types.</span></span> |

## <a name="response"></a><span data-ttu-id="d1046-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1046-132">Response</span></span>

<span data-ttu-id="d1046-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [permission](../resources/permission.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d1046-133">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1046-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d1046-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d1046-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d1046-135">Request</span></span>

<span data-ttu-id="d1046-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d1046-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_permission"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
##### <a name="response"></a><span data-ttu-id="d1046-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="d1046-137">Response</span></span>

<span data-ttu-id="d1046-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d1046-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "read" ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
