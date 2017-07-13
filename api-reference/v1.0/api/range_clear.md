<span data-ttu-id="aa2a0-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aa2a0-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <span data-ttu-id="aa2a0-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aa2a0-126">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="aa2a0-127">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="aa2a0-127">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="aa2a0-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aa2a0-128">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="aa2a0-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aa2a0-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_clear"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/clear
Content-type: application/json
Content-length: 32

{
  "applyTo": "applyTo-value"
}
```

##### <span data-ttu-id="aa2a0-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="aa2a0-130">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="aa2a0-131">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="aa2a0-131">Here is an example of the response.</span></span> 
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
  "description": "Range: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->