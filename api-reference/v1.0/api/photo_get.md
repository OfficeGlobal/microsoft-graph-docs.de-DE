<span data-ttu-id="4fe36-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4fe36-p101">Bearer token. Required.</span></span>  | Bearer {token}. Erforderlich. |

## <span data-ttu-id="4fe36-117">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4fe36-117">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="4fe36-118">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4fe36-118">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="4fe36-119">Antwort</span><span class="sxs-lookup"><span data-stu-id="4fe36-119">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="4fe36-120">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [photo](../resources/photo.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4fe36-120">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <span data-ttu-id="4fe36-121">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4fe36-121">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="4fe36-122">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4fe36-122">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="4fe36-123">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4fe36-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <span data-ttu-id="4fe36-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="4fe36-124">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="4fe36-125">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4fe36-125">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
