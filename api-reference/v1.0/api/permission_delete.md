# <a name="delete-permission"></a><span data-ttu-id="170aa-101">Berechtigung löschen</span><span class="sxs-lookup"><span data-stu-id="170aa-101">Delete permission</span></span>

<span data-ttu-id="170aa-102">Entfernt den Zugriffs auf ein [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="170aa-102">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="170aa-p101">Nur die Berechtigungen, die nicht geerbt werden, können gelöscht werden. Die **inheritedFrom**-Eigenschaft muss `null` sein.</span><span class="sxs-lookup"><span data-stu-id="170aa-p101">Only permissions that are not inherited can be deleted. The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="170aa-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="170aa-105">Permissions</span></span>
<span data-ttu-id="170aa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="170aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="170aa-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="170aa-108">Permission type</span></span>      | <span data-ttu-id="170aa-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="170aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="170aa-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="170aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="170aa-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170aa-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="170aa-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="170aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="170aa-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170aa-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="170aa-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="170aa-114">Application</span></span> | <span data-ttu-id="170aa-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="170aa-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="170aa-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="170aa-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/root:/{path}:/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
```

## <a name="request-headers"></a><span data-ttu-id="170aa-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="170aa-117">Request headers</span></span>

| <span data-ttu-id="170aa-118">Name</span><span class="sxs-lookup"><span data-stu-id="170aa-118">Name</span></span>          | <span data-ttu-id="170aa-119">Typ</span><span class="sxs-lookup"><span data-stu-id="170aa-119">Type</span></span>   | <span data-ttu-id="170aa-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="170aa-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="170aa-121">if-match</span><span class="sxs-lookup"><span data-stu-id="170aa-121">if-match</span></span>      | <span data-ttu-id="170aa-122">string</span><span class="sxs-lookup"><span data-stu-id="170aa-122">string</span></span> | <span data-ttu-id="170aa-123">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) nicht mit dem aktuellen Tag des Elements übereinstimmt, wird die Antwort `412 Precondition Failed` zurückgegeben, und das Element wird nicht gelöscht.</span><span class="sxs-lookup"><span data-stu-id="170aa-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="request-body"></a><span data-ttu-id="170aa-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="170aa-124">Request body</span></span>
<span data-ttu-id="170aa-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="170aa-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="170aa-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="170aa-126">Response</span></span>

<span data-ttu-id="170aa-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="170aa-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="170aa-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="170aa-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="170aa-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="170aa-130">Request</span></span>

<span data-ttu-id="170aa-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="170aa-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_permission"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/root/items/{item-id}/permissions/{perm-id}
```

##### <a name="response"></a><span data-ttu-id="170aa-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="170aa-132">Response</span></span>

<span data-ttu-id="170aa-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="170aa-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="170aa-134">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="170aa-134">Remarks</span></span>

* <span data-ttu-id="170aa-135">[Laufwerke](../resources/drive.md) mit dem**driveType** `personal` (OneDrive Personal) können keine Berechtigungen am Stamm-DriveItem erstellen oder ändern.</span><span class="sxs-lookup"><span data-stu-id="170aa-135">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission"
}-->
