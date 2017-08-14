<span data-ttu-id="5ec0a-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5ec0a-p101">Bearer {token}. Required.</span></span>  | Bearer {token}. Erforderlich. |


## <a name="request-body"></a><span data-ttu-id="5ec0a-118">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5ec0a-118">Request body</span></span>
<span data-ttu-id="5ec0a-119">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5ec0a-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ec0a-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ec0a-120">Response</span></span>

<span data-ttu-id="5ec0a-121">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [thumbnailSet](../resources/thumbnailset.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5ec0a-121">If successful, this method returns a `200 OK` response code and [thumbnailSet](../resources/thumbnailset.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5ec0a-122">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5ec0a-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ec0a-123">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5ec0a-123">Request</span></span>
<span data-ttu-id="5ec0a-124">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5ec0a-124">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}-->
```http
GET https://graph.microsoft.com/v1.0/drive/root/thumbnails/{id}
```
##### <a name="response"></a><span data-ttu-id="5ec0a-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="5ec0a-125">Response</span></span>
<span data-ttu-id="5ec0a-126">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5ec0a-126">Here is an example of the response.</span></span>
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
