<span data-ttu-id="9fb0d-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9fb0d-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a><span data-ttu-id="9fb0d-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9fb0d-119">Example</span></span>
<span data-ttu-id="9fb0d-120">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="9fb0d-120">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9fb0d-121">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9fb0d-121">Request</span></span>
<span data-ttu-id="9fb0d-122">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9fb0d-122">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookpivottable_refreshall"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/pivotTables/refreshAll
```

##### <a name="response"></a><span data-ttu-id="9fb0d-123">Antwort</span><span class="sxs-lookup"><span data-stu-id="9fb0d-123">Response</span></span>
<span data-ttu-id="9fb0d-124">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9fb0d-124">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```
