<span data-ttu-id="414de-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="414de-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

### <span data-ttu-id="414de-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="414de-119">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="414de-120">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="414de-120">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="414de-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="414de-121">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="414de-122">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="414de-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refresh"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/pivotTables/{id}/refresh
```

##### <span data-ttu-id="414de-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="414de-123">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="414de-124">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="414de-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
