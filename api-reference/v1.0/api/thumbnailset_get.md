# <a name="get-thumbnailset"></a><span data-ttu-id="8fcf3-101">thumbnailSet abrufen</span><span class="sxs-lookup"><span data-stu-id="8fcf3-101">Get thumbnailSet</span></span>

<span data-ttu-id="8fcf3-102">Dient zum Abrufen der Eigenschaften und der Beziehungen eines [thumbnailSet](../resources/thumbnailset.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8fcf3-102">Retrieve the properties and relationships of a [thumbnailSet](../resources/thumbnailset.md) object.</span></span>

<span data-ttu-id="8fcf3-103">Weitere Informationen finden Sie unter [Miniaturansichten auflisten](item_list_thumbnails.md).</span><span class="sxs-lookup"><span data-stu-id="8fcf3-103">For more info, see [List thumbnails](item_list_thumbnails.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fcf3-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8fcf3-104">Prerequisites</span></span>
<span data-ttu-id="8fcf3-105">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen:</span><span class="sxs-lookup"><span data-stu-id="8fcf3-105">One of the following **scopes** is required to execute this API:</span></span>

  * <span data-ttu-id="8fcf3-106">Files.Read</span><span class="sxs-lookup"><span data-stu-id="8fcf3-106">Files.Read</span></span>

## <a name="http-request"></a><span data-ttu-id="8fcf3-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fcf3-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /drive/root/thumbnails/{id}
GET /drive/items/{id}/thumbnails/{id}
GET /drives/{id}/root/thumbnails/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8fcf3-108">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8fcf3-108">Optional query parameters</span></span>
<span data-ttu-id="8fcf3-109">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8fcf3-109">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8fcf3-110">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8fcf3-110">Request headers</span></span>
| <span data-ttu-id="8fcf3-111">Name</span><span class="sxs-lookup"><span data-stu-id="8fcf3-111">Name</span></span>       | <span data-ttu-id="8fcf3-112">Typ</span><span class="sxs-lookup"><span data-stu-id="8fcf3-112">Type</span></span> | <span data-ttu-id="8fcf3-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8fcf3-113">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8fcf3-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fcf3-114">Authorization</span></span>  | <span data-ttu-id="8fcf3-115">string</span><span class="sxs-lookup"><span data-stu-id="8fcf3-115">string</span></span>  | <span data-ttu-id="8fcf3-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8fcf3-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8fcf3-118">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8fcf3-118">Request body</span></span>
<span data-ttu-id="8fcf3-119">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8fcf3-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fcf3-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fcf3-120">Response</span></span>

<span data-ttu-id="8fcf3-121">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [thumbnailSet](../resources/thumbnailset.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8fcf3-121">If successful, this method returns a `200 OK` response code and [thumbnailSet](../resources/thumbnailset.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8fcf3-122">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8fcf3-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8fcf3-123">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8fcf3-123">Request</span></span>
<span data-ttu-id="8fcf3-124">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8fcf3-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/thumbnails/{id}
```
##### <a name="response"></a><span data-ttu-id="8fcf3-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="8fcf3-125">Response</span></span>
<span data-ttu-id="8fcf3-126">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8fcf3-126">Here is an example of the response.</span></span>
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
