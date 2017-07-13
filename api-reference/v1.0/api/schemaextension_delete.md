<span data-ttu-id="5e943-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5e943-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <span data-ttu-id="5e943-119">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5e943-119">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="5e943-120">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5e943-120">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="5e943-121">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5e943-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_schemaextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/schemaExtensions/{id}
```
##### <span data-ttu-id="5e943-122">Antwort</span><span class="sxs-lookup"><span data-stu-id="5e943-122">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="5e943-123">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5e943-123">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <span data-ttu-id="5e943-124">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="5e943-124">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="5e943-125">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="5e943-125">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="5e943-126">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="5e943-126">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->