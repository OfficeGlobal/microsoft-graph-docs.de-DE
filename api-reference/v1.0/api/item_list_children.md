# <a name="list-children-of-a-driveitem"></a><span data-ttu-id="24620-101">Untergeordnete Elemente eines DriveItem auflisten</span><span class="sxs-lookup"><span data-stu-id="24620-101">List children of a driveItem</span></span>

<span data-ttu-id="24620-102">Eine Auflistung von [DriveItems](../resources/driveitem.md) im **untergeordneten** Verhältnis eines DriveItem zurückgeben.</span><span class="sxs-lookup"><span data-stu-id="24620-102">Return a collection of [DriveItems](../resources/driveitem.md) in the **children** relationship of a DriveItem.</span></span>

<span data-ttu-id="24620-103">Ressourcen des Typs „DriveItems“ mit einer Facette des Typs **folder** oder **package**, die einen anderen Wert als „null“ hat, können eine oder mehrere untergeordnete Ressourcen des Typs „DriveItems“ haben.</span><span class="sxs-lookup"><span data-stu-id="24620-103">DriveItems with a non-null **folder** or **package** facet can have one or more child DriveItems.</span></span>


## <a name="permissions"></a><span data-ttu-id="24620-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="24620-104">Permissions</span></span>
<span data-ttu-id="24620-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="24620-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="24620-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="24620-107">Permission type</span></span>      | <span data-ttu-id="24620-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="24620-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24620-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="24620-109">Delegated (work or school account)</span></span> | <span data-ttu-id="24620-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24620-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="24620-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="24620-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24620-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24620-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="24620-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="24620-113">Application</span></span> | <span data-ttu-id="24620-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24620-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="24620-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="24620-115">HTTP request</span></span>
```http
GET /me/drive/root/children
GET /me/drive/items/{item-id}/children
GET /me/drive/root:/{item-path}:/children
GET /drives/{drive-id}/items/{item-id}/children
GET /groups/{group-id}/drive/root/children
GET /groups/{group-id}/drive/items/{item-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24620-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="24620-116">Optional query parameters</span></span>
<span data-ttu-id="24620-117">Diese Methode unterstützt `$expand`, `$select`, `$skipToken`, `$top` und `$orderby` [OData-Abfrageparameter](../../../concepts/query_parameters.md) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="24620-117">This method supports the `$expand` and `$orderby` [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24620-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="24620-118">Request headers</span></span>

| <span data-ttu-id="24620-119">Name</span><span class="sxs-lookup"><span data-stu-id="24620-119">Name</span></span>          | <span data-ttu-id="24620-120">Typ</span><span class="sxs-lookup"><span data-stu-id="24620-120">Type</span></span>   | <span data-ttu-id="24620-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24620-121">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="24620-122">if-none-match</span><span class="sxs-lookup"><span data-stu-id="24620-122">if-none-match</span></span> | <span data-ttu-id="24620-123">String</span><span class="sxs-lookup"><span data-stu-id="24620-123">String</span></span> | <span data-ttu-id="24620-124">Wenn dieser Anforderungsheader enthalten ist und das angegebene eTag (oder cTag) mit dem aktuellen Tag in der Datei übereinstimmt, wird die Antwort `HTTP 304 Not Modified` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="24620-124">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24620-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="24620-125">Request body</span></span>
<span data-ttu-id="24620-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="24620-126">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="24620-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="24620-127">Example</span></span>

##### <a name="request"></a><span data-ttu-id="24620-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="24620-128">Request</span></span>
<span data-ttu-id="24620-129">Es folgt eine Beispiel für eine Anforderung, die DriveItems in den Stammordner des aktuellen Benutzers in OneDrive zurückgibt.zugeben.</span><span class="sxs-lookup"><span data-stu-id="24620-129">Here is an example request to return the DriveItems in the root folder of the current user's OneDrive.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_children"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/children
```

## <a name="response"></a><span data-ttu-id="24620-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="24620-130">Response</span></span>

<span data-ttu-id="24620-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="24620-131">Here is an example of the response.</span></span>
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

<span data-ttu-id="24620-132">**Hinweis:** Wenn eine Auflistung die Standardseitengröße (200 Artikel) überschreitet, wird die Eigenschaft **@odata.nextLink** in der Antwort zurückgegeben, damit angezeigt wird, dass mehr Elemente zur Verfügung, und die Anfrage-URL für die nächste Seite von Elementen zurückzugeben.</span><span class="sxs-lookup"><span data-stu-id="24620-132">**Note:** If a collection exceeds the default page size (200 items), the **@odata.nextLink** property is returned in the response to indicate more items are available and provide the request URL for the next page of items.</span></span>

<span data-ttu-id="24620-133">Sie können die Seitengröße über [Optionale Abfragezeichenfolge-Parameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) steuern.</span><span class="sxs-lookup"><span data-stu-id="24620-133">You can control the page size through [optional query string parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List the children of an item.",
  "keywords": "list,children,collection",
  "section": "documentation",
  "tocPath": "OneDrive/DriveItem/List children"
} -->
