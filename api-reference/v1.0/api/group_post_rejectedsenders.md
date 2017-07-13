<span data-ttu-id="521fb-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="521fb-p102">Bearer token. Required.</span></span>  | Bearer {token}. Erforderlich.  |

## <span data-ttu-id="521fb-115">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="521fb-115">Request body</span></span>
<a id="request-body" class="xliff"></a>
<span data-ttu-id="521fb-116">Geben Sie im Anforderungstext die ID eines Benutzer- oder Gruppenobjekts an.</span><span class="sxs-lookup"><span data-stu-id="521fb-116">In the request body, supply the id of a user or group object.</span></span>


## <span data-ttu-id="521fb-117">Antwort</span><span class="sxs-lookup"><span data-stu-id="521fb-117">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="521fb-118">Diese Methode gibt den Antwortcode `204, No Content` ohne Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="521fb-118">This method returns `204, No Content` response code and no response body.</span></span>

## <span data-ttu-id="521fb-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="521fb-119">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="521fb-120">Anforderung</span><span class="sxs-lookup"><span data-stu-id="521fb-120">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="521fb-121">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="521fb-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
}
```
##### <span data-ttu-id="521fb-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="521fb-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="521fb-123">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="521fb-123">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
