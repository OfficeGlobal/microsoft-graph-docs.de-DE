<span data-ttu-id="f5f4c-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202, Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f5f4c-p105">If successful, this method returns `202, Accepted` response code. It does not return anything in the response body.</span></span>
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `202, Accepted` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a><span data-ttu-id="f5f4c-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f5f4c-134">Example</span></span>
<span data-ttu-id="f5f4c-135">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="f5f4c-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f5f4c-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f5f4c-136">Request</span></span>
<span data-ttu-id="f5f4c-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f5f4c-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="f5f4c-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5f4c-138">Response</span></span>
##### <a name="response"></a><span data-ttu-id="f5f4c-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="f5f4c-139">Response</span></span>
<span data-ttu-id="f5f4c-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f5f4c-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
