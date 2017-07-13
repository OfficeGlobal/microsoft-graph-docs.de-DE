<span data-ttu-id="90c9b-p102">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="90c9b-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <span data-ttu-id="90c9b-123">Beispiel</span><span class="sxs-lookup"><span data-stu-id="90c9b-123">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="90c9b-124">Anforderung</span><span class="sxs-lookup"><span data-stu-id="90c9b-124">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="90c9b-125">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="90c9b-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <span data-ttu-id="90c9b-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="90c9b-126">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="90c9b-127">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="90c9b-127">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
