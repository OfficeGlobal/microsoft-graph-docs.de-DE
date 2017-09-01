# <a name="get-a-driveitem-resource"></a><span data-ttu-id="e217c-101">DriveItem-Ressource abrufen</span><span class="sxs-lookup"><span data-stu-id="e217c-101">Get a DriveItem resource</span></span>

<span data-ttu-id="e217c-102">Mit dieser API können Sie die Metadaten einer Ressource des Typs [DriveItem](../resources/driveitem.md) in einer Ressource des Typs [Drive](../resources/drive.md) abrufen. Hierzu verwenden Sie den Dateisystempfad oder die ID der Ressource des Typs „DriveItem“.</span><span class="sxs-lookup"><span data-stu-id="e217c-102">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="e217c-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e217c-103">Permissions</span></span>
<span data-ttu-id="e217c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e217c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e217c-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e217c-106">Permission type</span></span>      | <span data-ttu-id="e217c-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e217c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e217c-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e217c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="e217c-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e217c-109">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e217c-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e217c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e217c-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e217c-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e217c-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e217c-112">Application</span></span> | <span data-ttu-id="e217c-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e217c-113">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e217c-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e217c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /drives/{drive-id}/items/{item-id}
GET /groups/{group-id}/drive/items/{item-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e217c-115">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e217c-115">Optional query parameters</span></span>
<span data-ttu-id="e217c-116">Diese Methode unterstützt die [OData-Abfrageparameter](../../../concepts/query_parameters.md) von `$expand` und `$select` zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e217c-116">This method supports the `$expand` and `$select` [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e217c-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e217c-117">Request headers</span></span>

| <span data-ttu-id="e217c-118">Name</span><span class="sxs-lookup"><span data-stu-id="e217c-118">Name</span></span>          | <span data-ttu-id="e217c-119">Wert</span><span class="sxs-lookup"><span data-stu-id="e217c-119">Value</span></span>  | <span data-ttu-id="e217c-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e217c-120">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e217c-121">if-none-match</span><span class="sxs-lookup"><span data-stu-id="e217c-121">if-none-match</span></span> | <span data-ttu-id="e217c-122">String</span><span class="sxs-lookup"><span data-stu-id="e217c-122">String</span></span> | <span data-ttu-id="e217c-123">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) mit dem aktuellen Tag in der Datei übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e217c-123">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e217c-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e217c-124">Request body</span></span>
<span data-ttu-id="e217c-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e217c-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e217c-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="e217c-126">Response</span></span>

<span data-ttu-id="e217c-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die aktualisierte [DriveItem](../resources/driveitem.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e217c-127">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e217c-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e217c-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e217c-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e217c-129">Request</span></span>

<span data-ttu-id="e217c-130">Nachfolgend finden Sie ein Beispiel der Anforderung für den Stammordner des OneDrive-Elements des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="e217c-130">Here is an example of the request to the root folder of the user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item"
}-->
```
GET https://graph.microsoft.com/v1.0//me/drive/root
```

##### <a name="response"></a><span data-ttu-id="e217c-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e217c-131">Response</span></span>
<span data-ttu-id="e217c-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e217c-132">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "createdDateTime": "2016-03-21T20:01:37Z",
  "cTag": "\"c:{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},0\"",
  "eTag": "\"{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},1\"",
  "folder": { "childCount": 120 },
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "lastModifiedBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "lastModifiedDateTime": "2016-03-21T20:01:37Z",
  "name": "OneDrive",
  "root": { },
  "size": 157286400,
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents"
}
```

## <a name="notes"></a><span data-ttu-id="e217c-133">Anmerkungen</span><span class="sxs-lookup"><span data-stu-id="e217c-133">Notes</span></span>

<span data-ttu-id="e217c-134">Sie können den [`$expand`Parameter der Abfragezeichenfolge](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) verwenden, um die untergeordneten Elemente eines Elements im gleichen Aufruf wie beim Abrufen der Metadaten eines Elements verwenden, wenn das Element eine **untergeordnete** Beziehung aufweist.</span><span class="sxs-lookup"><span data-stu-id="e217c-134">You can use the [`$expand` query string parameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get item"
}-->
