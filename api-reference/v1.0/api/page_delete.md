<span data-ttu-id="eb97a-p102">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb97a-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a><span data-ttu-id="eb97a-118">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb97a-118">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eb97a-119">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb97a-119">Request</span></span>
<span data-ttu-id="eb97a-120">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eb97a-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="eb97a-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb97a-121">Response</span></span>
<span data-ttu-id="eb97a-122">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="eb97a-122">Here is an example of the response.</span></span>
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
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->