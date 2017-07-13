<span data-ttu-id="e2dd8-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2dd8-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <span data-ttu-id="e2dd8-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e2dd8-130">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="e2dd8-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2dd8-131">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="e2dd8-132">Hier finden Sie ein Beispiel für die Anforderung zum Löschen einer Anlage für ein Ereignis.</span><span class="sxs-lookup"><span data-stu-id="e2dd8-132">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <span data-ttu-id="e2dd8-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2dd8-133">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="e2dd8-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e2dd8-134">Here is an example of the response.</span></span>
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
  "description": "Delete attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
