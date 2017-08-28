# <a name="list-permissions-on-a-driveitem"></a><span data-ttu-id="f316c-101">Auflisten von Berechtigungen für DriveItem</span><span class="sxs-lookup"><span data-stu-id="f316c-101">List permissions on a DriveItem</span></span>

<span data-ttu-id="f316c-102">Listen Sie geltende Berechtigungen für ein [DriveItem](../resources/driveitem.md)-Objekt auf.</span><span class="sxs-lookup"><span data-stu-id="f316c-102">List the effective permissions of on a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="f316c-p101">Die **permissions**-Beziehungen eines DriveItem-Elements können nicht im Rahmen eines Aufrufs von [get DriveItem](item_get.md) oder einer Sammlung von DriveItems erweitert werden. Sie müssen direkt auf die permissions-Eigenschaft zugreifen.</span><span class="sxs-lookup"><span data-stu-id="f316c-p101">The **permissions** relationship of DriveItem cannot be expanded as part of a call to [get DriveItem](item_get.md) or a collection of DriveItems. You must access the permissions property directly.</span></span>

## <a name="access-to-permissions"></a><span data-ttu-id="f316c-105">Zugriff auf Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f316c-105">Access to Permissions</span></span>

<span data-ttu-id="f316c-106">Die Berechtigungssammlung umfasst potenziell vertrauliche Informationen und ist möglicherweise nicht für alle Aufrufer verfügbar.</span><span class="sxs-lookup"><span data-stu-id="f316c-106">The permissions collection includes potentially sensitive information and may not be available for every caller.</span></span>

* <span data-ttu-id="f316c-p102">Für den Besitzer des Elements werden alle Berechtigungen zurückgegeben. Dies umfasst Mitbesitzer.</span><span class="sxs-lookup"><span data-stu-id="f316c-p102">For the owner of the item, all permissions will be returned. This includes co-owners.</span></span>
* <span data-ttu-id="f316c-109">Für Aufrufer, die keine Besitzer sind, werden nur die Berechtigungen zurückgegeben, die für den Aufrufer gelten.</span><span class="sxs-lookup"><span data-stu-id="f316c-109">For a non-owner caller, only the permissions that apply to the caller are returned.</span></span>
* <span data-ttu-id="f316c-110">Berechtigungseigenschaften, die Geheimnisse enthalten (z. B. `shareId` und `webUrl`), werden nur für Aufrufer zurückgegeben, die Berechtigungen erstellen können.</span><span class="sxs-lookup"><span data-stu-id="f316c-110">Permission properties that contain secrets (e.g. `shareId` and `webUrl`) are only returned for callers that are able to create the Permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="f316c-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f316c-111">Permissions</span></span>
<span data-ttu-id="f316c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f316c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f316c-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f316c-114">Permission type</span></span>      | <span data-ttu-id="f316c-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f316c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f316c-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f316c-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f316c-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f316c-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f316c-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f316c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f316c-119">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f316c-119">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f316c-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f316c-120">Application</span></span> | <span data-ttu-id="f316c-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f316c-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f316c-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f316c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
```

## <a name="request-headers"></a><span data-ttu-id="f316c-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f316c-123">Request headers</span></span>

| <span data-ttu-id="f316c-124">Name</span><span class="sxs-lookup"><span data-stu-id="f316c-124">Name</span></span>          | <span data-ttu-id="f316c-125">Typ</span><span class="sxs-lookup"><span data-stu-id="f316c-125">Type</span></span>   | <span data-ttu-id="f316c-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f316c-126">Description</span></span>                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f316c-127">if-none-match</span><span class="sxs-lookup"><span data-stu-id="f316c-127">if-none-match</span></span> | <span data-ttu-id="f316c-128">string</span><span class="sxs-lookup"><span data-stu-id="f316c-128">string</span></span> | <span data-ttu-id="f316c-129">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag mit dem aktuellen eTag in dem Element übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f316c-129">If this request header is included and the etag provided matches the current etag on the item, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="f316c-130">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f316c-130">Optional query parameters</span></span>
<span data-ttu-id="f316c-131">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f316c-131">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="f316c-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f316c-132">Request body</span></span>
<span data-ttu-id="f316c-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f316c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f316c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f316c-134">Response</span></span>

<span data-ttu-id="f316c-135">Bei Erfolg gibt diese Methode den Antwortcode `200 OK` und eine Sammlung von [Permission](../resources/permission.md)-Ressourcen im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="f316c-135">If successful, this method returns a `200 OK` response code and collection of [Permission](../resources/permission.md) resources in the response body.</span></span>

<span data-ttu-id="f316c-136">Geltende Berechtigungen eines Elements können aus zwei Quellen stammen:</span><span class="sxs-lookup"><span data-stu-id="f316c-136">Effective permissions of an item can come from two sources:</span></span>

* <span data-ttu-id="f316c-137">Berechtigungen, die direkt für das Element selbst gelten</span><span class="sxs-lookup"><span data-stu-id="f316c-137">Permissions applied directly on the item itself</span></span>
* <span data-ttu-id="f316c-138">Berechtigungen, die von Vorgängerelementen geerbt werden</span><span class="sxs-lookup"><span data-stu-id="f316c-138">Permissions inherited from the item's ancestors</span></span>

<span data-ttu-id="f316c-p104">Aufrufer können prüfen, ob die Berechtigung geerbt wurde, indem sie die **inheritedFrom**-Eigenschaft prüfen. Diese Eigenschaft ist eine [**itemReference**](../resources/itemreference.md)-Ressource, die auf das Vorgängerelement verweist, von dem die Berechtigung vererbt wurde.</span><span class="sxs-lookup"><span data-stu-id="f316c-p104">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

## <a name="example"></a><span data-ttu-id="f316c-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f316c-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f316c-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f316c-142">Request</span></span>
<span data-ttu-id="f316c-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f316c-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_permissions"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions
```


##### <a name="response"></a><span data-ttu-id="f316c-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="f316c-144">Response</span></span>
<span data-ttu-id="f316c-145">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f316c-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "TimeTravelPlus"
        }
      }
    }
  ]
}
```

<span data-ttu-id="f316c-146">Weitere Informationen zum Abrufen einer einzelnen Berechtigungsressource finden Sie unter [Abrufen von Berechtigungen](permission_get.md).</span><span class="sxs-lookup"><span data-stu-id="f316c-146">See [Get permission](permission_get.md) for more details on retrieving a single permission resource.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List permissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List permissions"
}-->
