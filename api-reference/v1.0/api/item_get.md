# <span data-ttu-id="a3ae7-101">DriveItem-Ressource abrufen</span><span class="sxs-lookup"><span data-stu-id="a3ae7-101">Get a DriveItem resource</span></span>
<a id="get-a-driveitem-resource" class="xliff"></a>

<span data-ttu-id="a3ae7-102">Ruft die Metadaten für ein [DriveItem](../resources/driveitem.md)-Element in einem [Laufwerk](../resources/drive.md) nach Systempfad oder ID ab.</span><span class="sxs-lookup"><span data-stu-id="a3ae7-102">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <span data-ttu-id="a3ae7-103">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a3ae7-103">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>
<span data-ttu-id="a3ae7-104">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="a3ae7-104">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="a3ae7-105">Files.Read</span><span class="sxs-lookup"><span data-stu-id="a3ae7-105">Files.Read</span></span>
* <span data-ttu-id="a3ae7-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a3ae7-106">Files.ReadWrite</span></span>
* <span data-ttu-id="a3ae7-107">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3ae7-107">Files.Read.All</span></span>
* <span data-ttu-id="a3ae7-108">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3ae7-108">Files.ReadWrite.All</span></span>
* <span data-ttu-id="a3ae7-109">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3ae7-109">Sites.Read.All</span></span>
* <span data-ttu-id="a3ae7-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3ae7-110">Sites.ReadWrite.All</span></span>

## <span data-ttu-id="a3ae7-111">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3ae7-111">HTTP request</span></span>
<a id="http-request" class="xliff"></a>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /drives/{drive-id}/items/{item-id}
GET /groups/{group-id}/drive/items/{item-id}
```

## <span data-ttu-id="a3ae7-112">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a3ae7-112">Optional query parameters</span></span>
<a id="optional-query-parameters" class="xliff"></a>
<span data-ttu-id="a3ae7-113">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a3ae7-113">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <span data-ttu-id="a3ae7-114">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a3ae7-114">Request headers</span></span>
<a id="request-headers" class="xliff"></a>

| <span data-ttu-id="a3ae7-115">Name</span><span class="sxs-lookup"><span data-stu-id="a3ae7-115">Name</span></span>          | <span data-ttu-id="a3ae7-116">Wert</span><span class="sxs-lookup"><span data-stu-id="a3ae7-116">Value</span></span>  | <span data-ttu-id="a3ae7-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a3ae7-117">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a3ae7-118">if-none-match</span><span class="sxs-lookup"><span data-stu-id="a3ae7-118">if-none-match</span></span> | <span data-ttu-id="a3ae7-119">String</span><span class="sxs-lookup"><span data-stu-id="a3ae7-119">String</span></span> | <span data-ttu-id="a3ae7-120">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) mit dem aktuellen Tag in der Datei übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a3ae7-120">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |


## <span data-ttu-id="a3ae7-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a3ae7-121">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="a3ae7-122">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a3ae7-122">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="a3ae7-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3ae7-123">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="a3ae7-124">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und die aktualisierte [DriveItem](../resources/driveitem.md)-Ressource im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a3ae7-124">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <span data-ttu-id="a3ae7-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a3ae7-125">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="a3ae7-126">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3ae7-126">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="a3ae7-127">Nachfolgend finden Sie ein Beispiel der Anforderung für den Stammordner des OneDrive-Elements des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="a3ae7-127">Here is an example of the request to the root folder of the user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_item"
}-->
```
GET https://graph.microsoft.com/v1.0//me/drive/root
```

##### <span data-ttu-id="a3ae7-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3ae7-128">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="a3ae7-129">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a3ae7-129">Here is an example of the response.</span></span>

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

## <span data-ttu-id="a3ae7-130">Anmerkungen</span><span class="sxs-lookup"><span data-stu-id="a3ae7-130">Notes</span></span>
<a id="notes" class="xliff"></a>

<span data-ttu-id="a3ae7-131">Sie können den [`$expand`Parameter der Abfragezeichenfolge](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) verwenden, um die untergeordneten Elemente eines Elements im gleichen Aufruf wie beim Abrufen der Metadaten eines Elements verwenden, wenn das Element eine **untergeordnete** Beziehung aufweist.</span><span class="sxs-lookup"><span data-stu-id="a3ae7-131">You can use the [`$expand` query string parameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get item",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Get item"
}-->
