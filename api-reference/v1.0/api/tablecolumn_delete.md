<span data-ttu-id="8a6f5-p102">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a6f5-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a><span data-ttu-id="8a6f5-117">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8a6f5-117">Example</span></span>
<span data-ttu-id="8a6f5-118">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="8a6f5-118">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8a6f5-119">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a6f5-119">Request</span></span>
<span data-ttu-id="8a6f5-120">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8a6f5-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablecolumn_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/delete
```

##### <a name="response"></a><span data-ttu-id="8a6f5-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a6f5-121">Response</span></span>
<span data-ttu-id="8a6f5-122">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8a6f5-122">Here is an example of the response.</span></span> 
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
  "description": "TableColumn: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->