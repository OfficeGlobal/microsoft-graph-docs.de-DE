<span data-ttu-id="33acc-p102">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="33acc-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <span data-ttu-id="33acc-117">Beispiel</span><span class="sxs-lookup"><span data-stu-id="33acc-117">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="33acc-118">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="33acc-118">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="33acc-119">Anforderung</span><span class="sxs-lookup"><span data-stu-id="33acc-119">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="33acc-120">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="33acc-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/delete
```

##### <span data-ttu-id="33acc-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="33acc-121">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="33acc-122">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="33acc-122">Here is an example of the response.</span></span> 
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
  "description": "Chart: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->