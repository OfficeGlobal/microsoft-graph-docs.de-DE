<span data-ttu-id="5cdd1-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202, Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5cdd1-p104">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202, Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <span data-ttu-id="5cdd1-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5cdd1-127">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="5cdd1-128">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="5cdd1-128">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="5cdd1-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5cdd1-129">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="5cdd1-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5cdd1-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```

##### <span data-ttu-id="5cdd1-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="5cdd1-131">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="5cdd1-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5cdd1-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
