<span data-ttu-id="606b5-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="606b5-p101">Bearer token. Required.</span></span>  | Bearer {token}. Erforderlich. |

## <span data-ttu-id="606b5-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="606b5-116">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="606b5-117">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="606b5-117">Do not supply a request body for this method.</span></span>
## <span data-ttu-id="606b5-118">Antwort</span><span class="sxs-lookup"><span data-stu-id="606b5-118">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="606b5-119">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="606b5-119">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <span data-ttu-id="606b5-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="606b5-120">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="606b5-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="606b5-121">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="606b5-122">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="606b5-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
```
##### <span data-ttu-id="606b5-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="606b5-123">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="606b5-124">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="606b5-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "changeType":"created,updated",
  "clientState":"subscription-identifier",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
