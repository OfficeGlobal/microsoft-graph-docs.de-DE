<span data-ttu-id="bc6a0-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc6a0-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <span data-ttu-id="bc6a0-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bc6a0-129">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="bc6a0-130">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="bc6a0-130">Here is an example of how to call this API.</span></span>
##### <span data-ttu-id="bc6a0-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc6a0-131">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="bc6a0-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bc6a0-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "event_snoozereminder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/snoozeReminder
Content-type: application/json
Content-length: 97

{
  "newReminderTime": {
    "dateTime": "dateTime-value",
    "timeZone": "timeZone-value"
  }
}
```

##### <span data-ttu-id="bc6a0-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc6a0-133">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="bc6a0-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bc6a0-134">Here is an example of the response.</span></span>
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
  "description": "event: snoozeReminder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
