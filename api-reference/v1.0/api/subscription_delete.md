<span data-ttu-id="995e9-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="995e9-p101">Bearer token. Required.</span></span>  | Bearer {token}. Erforderlich. |

## <span data-ttu-id="995e9-114">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="995e9-114">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="995e9-115">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="995e9-115">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="995e9-116">Antwort</span><span class="sxs-lookup"><span data-stu-id="995e9-116">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="995e9-117">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="995e9-117">If successful, this method returns a `204 No Content` response code.</span></span>
## <span data-ttu-id="995e9-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="995e9-118">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="995e9-119">Anforderung</span><span class="sxs-lookup"><span data-stu-id="995e9-119">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="995e9-120">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="995e9-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_subscription"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <span data-ttu-id="995e9-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="995e9-121">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="995e9-122">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="995e9-122">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Delete subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
