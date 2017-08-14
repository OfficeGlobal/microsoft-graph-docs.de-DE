<span data-ttu-id="f7a34-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f7a34-p103">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a><span data-ttu-id="f7a34-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f7a34-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7a34-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f7a34-131">Request</span></span>
<span data-ttu-id="f7a34-132">Hier finden Sie ein Beispiel für die Anforderung zum Löschen einer Anlage für ein Ereignis.</span><span class="sxs-lookup"><span data-stu-id="f7a34-132">Here is an example of the request to delete an attachment on an event.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_attachment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/events/{id}/attachments/{id}
```
##### <a name="response"></a><span data-ttu-id="f7a34-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f7a34-133">Response</span></span>
<span data-ttu-id="f7a34-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f7a34-134">Here is an example of the response.</span></span>
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
