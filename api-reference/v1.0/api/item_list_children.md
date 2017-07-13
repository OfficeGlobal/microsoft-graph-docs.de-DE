# <span data-ttu-id="fa2c9-101">Untergeordnete Elemente eines DriveItem auflisten</span><span class="sxs-lookup"><span data-stu-id="fa2c9-101">List children of a driveItem</span></span>
<a id="list-children-of-a-driveitem" class="xliff"></a>

<span data-ttu-id="fa2c9-102">Eine Auflistung von [DriveItems](../resources/driveitem.md) im **untergeordneten** Verhältnis eines DriveItem zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="fa2c9-102">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="fa2c9-103">DriveItems mit einem nicht-NULL-Werte-**Ordner oder einer Paket**-Facette können ein oder mehrere untergeordnete DriveItems haben.</span><span class="sxs-lookup"><span data-stu-id="fa2c9-103">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <span data-ttu-id="fa2c9-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fa2c9-104">Prerequisites</span></span>
<a id="prerequisites" class="xliff"></a>
<span data-ttu-id="fa2c9-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="fa2c9-105">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="fa2c9-106">Files.Read</span><span class="sxs-lookup"><span data-stu-id="fa2c9-106">Files.Read</span></span>
* <span data-ttu-id="fa2c9-107">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fa2c9-107">Files.ReadWrite</span></span>
* <span data-ttu-id="fa2c9-108">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa2c9-108">Files.Read.All</span></span>
* <span data-ttu-id="fa2c9-109">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa2c9-109">Files.ReadWrite.All</span></span>
* <span data-ttu-id="fa2c9-110">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa2c9-110">Sites.Read.All</span></span>
* <span data-ttu-id="fa2c9-111">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa2c9-111">Sites.ReadWrite.All</span></span>

## <span data-ttu-id="fa2c9-112">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa2c9-112">HTTP request</span></span>
<a id="http-request" class="xliff"></a>
```http
GET /me/drive/root/children
GET /me/drive/items/{item-id}/children
GET /me/drive/root:/{item-path}:/children
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/root/children
GET /groups/{group-id}/drive/items/{item-id}
```

## <span data-ttu-id="fa2c9-113">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fa2c9-113">Optional query parameters</span></span>
<a id="optional-query-parameters" class="xliff"></a>
<span data-ttu-id="fa2c9-114">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fa2c9-114">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <span data-ttu-id="fa2c9-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa2c9-115">Request headers</span></span>
<a id="request-headers" class="xliff"></a>

| <span data-ttu-id="fa2c9-116">Name</span><span class="sxs-lookup"><span data-stu-id="fa2c9-116">Name</span></span>          | <span data-ttu-id="fa2c9-117">Typ</span><span class="sxs-lookup"><span data-stu-id="fa2c9-117">Type</span></span>   | <span data-ttu-id="fa2c9-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa2c9-118">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="fa2c9-119">if-none-match</span><span class="sxs-lookup"><span data-stu-id="fa2c9-119">if-none-match</span></span> | <span data-ttu-id="fa2c9-120">String</span><span class="sxs-lookup"><span data-stu-id="fa2c9-120">String</span></span> | <span data-ttu-id="fa2c9-121">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) mit dem aktuellen Tag in der Datei übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa2c9-121">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <span data-ttu-id="fa2c9-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa2c9-122">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="fa2c9-123">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fa2c9-123">Do not supply a request body for this method.</span></span>

## <span data-ttu-id="fa2c9-124">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa2c9-124">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="fa2c9-125">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa2c9-125">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="fa2c9-126">Es folgt eine Beispiel für eine Anforderung, die DriveItems in den Stammordner des aktuellen Benutzers in OneDrive zurückgibt.zugeben.</span><span class="sxs-lookup"><span data-stu-id="fa2c9-126">Here is an example request to return the DriveItems in the root folder of the current user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_children"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/children
```

## <span data-ttu-id="fa2c9-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa2c9-127">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="fa2c9-128">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fa2c9-128">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {"name": "myfile.jpg", "size": 2048, "file": {} },
    {"name": "Documents", "folder": { "childCount": 4} },
    {"name": "Photos", "folder": { "childCount": 203} },
    {"name": "my sheet(1).xlsx", "size": 197 }
  ],
  "@odata.nextLink": "https://..."
}
```

<span data-ttu-id="fa2c9-129">**Hinweis:** Wenn eine Auflistung die Standardseitengröße (200 Artikel) überschreitet, wird die Eigenschaft **@odata.nextLink** in der Antwort zurückgegeben, damit angezeigt wird, dass mehr Elemente zur Verfügung, und die Anfrage-URL für die nächste Seite von Elementen zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="fa2c9-129">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="fa2c9-130">Sie können die Seitengröße über [Optionale Abfragezeichenfolge-Parameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) steuern.</span><span class="sxs-lookup"><span data-stu-id="fa2c9-130">You can control the page size through [optional query string parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "OneDrive/DriveItem/List children"
} -->
