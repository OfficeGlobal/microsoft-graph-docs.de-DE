<span data-ttu-id="6b417-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202, Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6b417-p103">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202, Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <span data-ttu-id="6b417-120">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6b417-120">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="6b417-121">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="6b417-121">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="6b417-122">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b417-122">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="6b417-123">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6b417-123">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <span data-ttu-id="6b417-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b417-124">Response</span></span>
<a id="response" class="xliff"></a>
##### <span data-ttu-id="6b417-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b417-125">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="6b417-126">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6b417-126">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
