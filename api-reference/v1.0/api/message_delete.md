<span data-ttu-id="5cd42-p102">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5cd42-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <span data-ttu-id="5cd42-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5cd42-119">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="5cd42-120">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5cd42-120">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="5cd42-121">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5cd42-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_message"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
##### <span data-ttu-id="5cd42-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="5cd42-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="5cd42-123">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5cd42-123">Here is an example of the response.</span></span> 
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
  "description": "Delete message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->