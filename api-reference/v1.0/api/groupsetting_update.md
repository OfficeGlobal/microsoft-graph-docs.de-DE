<span data-ttu-id="0813a-p102">Der aktualisierten Satz von Werten.  HINWEIS: Sie müssen den gesamten Sammlungssatz angeben. Sie können keinen einzelnen Wertesatz aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="0813a-p102">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> | Der aktualisierten Satz von Werten.  HINWEIS: Sie müssen den gesamten Sammlungssatz angeben. Sie können keinen einzelnen Wertesatz aktualisieren. |

## <a name="response"></a><span data-ttu-id="0813a-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="0813a-126">Response</span></span>

<span data-ttu-id="0813a-127">Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `204 OK` und ein aktualisiertes [groupSetting](../resources/groupsetting.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0813a-127">If successful, this method returns a `204 OK` response code and [directoryObject](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0813a-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0813a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0813a-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0813a-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a><span data-ttu-id="0813a-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="0813a-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->