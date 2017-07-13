<span data-ttu-id="29826-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="29826-p102">Bearer token. Required.</span></span>  | Bearer {token}. Erforderlich. |

## <span data-ttu-id="29826-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="29826-117">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="29826-118">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [subscription](../resources/subscription.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29826-118">If successful, this method returns a `200 OK` response code and [subscription](../resources/subscription.md) object in the response body.</span></span>
## <span data-ttu-id="29826-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="29826-119">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="29826-120">Anforderung</span><span class="sxs-lookup"><span data-stu-id="29826-120">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="29826-121">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="29826-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{subscriptionId}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```

##### <span data-ttu-id="29826-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="29826-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="29826-123">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="29826-123">Here is an example of the response.</span></span>
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
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```


<!-- {
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
