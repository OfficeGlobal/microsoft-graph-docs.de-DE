<span data-ttu-id="29f6c-p102">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="29f6c-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <span data-ttu-id="29f6c-117">Beispiel</span><span class="sxs-lookup"><span data-stu-id="29f6c-117">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="29f6c-118">Anforderung</span><span class="sxs-lookup"><span data-stu-id="29f6c-118">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="29f6c-119">Im Folgenden finden Sie ein paar Beispiele für die Themenbereiche, an denen wir arbeiten:</span><span class="sxs-lookup"><span data-stu-id="29f6c-119">Here are a couple of examples of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref?$id="users/{id}"

DELETE https://graph.microsoft.com/v1.0/groups/{id}/acceptedSenders/$ref?$id="groups/{id}"
```

##### <span data-ttu-id="29f6c-120">Antwort</span><span class="sxs-lookup"><span data-stu-id="29f6c-120">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="29f6c-121">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="29f6c-121">Here is an example of the response.</span></span> 
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
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->