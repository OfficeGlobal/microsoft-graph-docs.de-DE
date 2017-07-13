<span data-ttu-id="03f2b-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="03f2b-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <span data-ttu-id="03f2b-125">Beispiel</span><span class="sxs-lookup"><span data-stu-id="03f2b-125">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="03f2b-126">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="03f2b-126">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="03f2b-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="03f2b-127">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="03f2b-128">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="03f2b-128">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/delete
Content-type: application/json
Content-length: 28

{
  "shift": "shift-value"
}
```

##### <span data-ttu-id="03f2b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="03f2b-129">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="03f2b-130">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="03f2b-130">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->