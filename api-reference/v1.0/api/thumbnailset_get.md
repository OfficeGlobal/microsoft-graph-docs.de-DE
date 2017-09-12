# <a name="get-thumbnailset"></a><span data-ttu-id="9c4ce-101">thumbnailSet abrufen</span><span class="sxs-lookup"><span data-stu-id="9c4ce-101">Get thumbnailSet</span></span>

<span data-ttu-id="9c4ce-102">Dient zum Abrufen der Eigenschaften und der Beziehungen eines [thumbnailSet](../resources/thumbnailset.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9c4ce-102">Retrieve the properties and relationships of a [thumbnailSet](../resources/thumbnailset.md) object.</span></span>

<span data-ttu-id="9c4ce-103">Weitere Informationen finden Sie unter [Miniaturansichten auflisten](item_list_thumbnails.md).</span><span class="sxs-lookup"><span data-stu-id="9c4ce-103">For more info, see [List thumbnails](item_list_thumbnails.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9c4ce-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9c4ce-104">Permissions</span></span>
<span data-ttu-id="9c4ce-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9c4ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9c4ce-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9c4ce-107">Permission type</span></span>      | <span data-ttu-id="9c4ce-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9c4ce-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="9c4ce-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9c4ce-109">Delegated (work or school account)</span></span> | <span data-ttu-id="9c4ce-110">Files.Read</span><span class="sxs-lookup"><span data-stu-id="9c4ce-110">Files.Read</span></span>    | 
|<span data-ttu-id="9c4ce-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9c4ce-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c4ce-112">Files.Read</span><span class="sxs-lookup"><span data-stu-id="9c4ce-112">Files.Read</span></span>    | 
|<span data-ttu-id="9c4ce-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9c4ce-113">Application</span></span> | <span data-ttu-id="9c4ce-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9c4ce-114">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9c4ce-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c4ce-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /drive/root/thumbnails/{id}
GET /drive/items/{id}/thumbnails/{id}
GET /drives/{id}/root/thumbnails/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9c4ce-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9c4ce-116">Optional query parameters</span></span>
<span data-ttu-id="9c4ce-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9c4ce-117">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c4ce-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9c4ce-118">Request headers</span></span>
| <span data-ttu-id="9c4ce-119">Name</span><span class="sxs-lookup"><span data-stu-id="9c4ce-119">Name</span></span>       | <span data-ttu-id="9c4ce-120">Typ</span><span class="sxs-lookup"><span data-stu-id="9c4ce-120">Type</span></span> | <span data-ttu-id="9c4ce-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c4ce-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9c4ce-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c4ce-122">Authorization</span></span>  | <span data-ttu-id="9c4ce-123">string</span><span class="sxs-lookup"><span data-stu-id="9c4ce-123">string</span></span>  | <span data-ttu-id="9c4ce-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9c4ce-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="9c4ce-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9c4ce-126">Request body</span></span>
<span data-ttu-id="9c4ce-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9c4ce-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c4ce-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c4ce-128">Response</span></span>

<span data-ttu-id="9c4ce-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [thumbnailSet](../resources/thumbnailset.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9c4ce-129">If successful, this method returns a `200 OK` response code and [thumbnailSet](../resources/thumbnailset.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9c4ce-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9c4ce-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c4ce-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9c4ce-131">Request</span></span>
<span data-ttu-id="9c4ce-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9c4ce-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/thumbnails/{id}
```
##### <a name="response"></a><span data-ttu-id="9c4ce-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="9c4ce-133">Response</span></span>
<span data-ttu-id="9c4ce-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9c4ce-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.thumbnailSet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 456

{
  "id": "id-value",
  "large": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "medium": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "small": {
    "height": 99,
    "url": "url-value",
    "width": 99
  },
  "source": {
    "height": 99,
    "url": "url-value",
    "width": 99
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get thumbnailSet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
