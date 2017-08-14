<span data-ttu-id="66c54-p102">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="66c54-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.

## <a name="example"></a><span data-ttu-id="66c54-123">Beispiel</span><span class="sxs-lookup"><span data-stu-id="66c54-123">Example</span></span>

##### <a name="request"></a><span data-ttu-id="66c54-124">Anforderung</span><span class="sxs-lookup"><span data-stu-id="66c54-124">Request</span></span>

<span data-ttu-id="66c54-125">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="66c54-125">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_permission"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/root/items/{item-id}/permissions/{perm-id}
```

##### <a name="response"></a><span data-ttu-id="66c54-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="66c54-126">Response</span></span>

<span data-ttu-id="66c54-127">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="66c54-127">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="66c54-128">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="66c54-128">Remarks</span></span>

* <span data-ttu-id="66c54-129">[Laufwerke](../resources/drive.md) mit dem**driveType** `personal` (OneDrive Personal) können keine Berechtigungen am Stamm-DriveItem erstellen oder ändern.</span><span class="sxs-lookup"><span data-stu-id="66c54-129">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission"
}-->
