<span data-ttu-id="9cc54-p101">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="9cc54-p101">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| <span data-ttu-id="9cc54-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9cc54-120">Property</span></span>     | <span data-ttu-id="9cc54-121">Typ</span><span class="sxs-lookup"><span data-stu-id="9cc54-121">Type</span></span>   | <span data-ttu-id="9cc54-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9cc54-122">Description</span></span>                   |
|:-------------|:-------|:------------------------------|
| <span data-ttu-id="9cc54-123">**roles**</span><span class="sxs-lookup"><span data-stu-id="9cc54-123">**roles**</span></span>    | <span data-ttu-id="9cc54-124">String</span><span class="sxs-lookup"><span data-stu-id="9cc54-124">String</span></span> | <span data-ttu-id="9cc54-125">Ein Array von Berechtigungstypen.</span><span class="sxs-lookup"><span data-stu-id="9cc54-125">An array of permission types.</span></span> |


## <span data-ttu-id="9cc54-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="9cc54-126">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="9cc54-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [permission](../resources/permission.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9cc54-127">If successful, this method returns a `200 OK` response code and updated [permission](../resources/permission.md) object in the response body.</span></span>

## <span data-ttu-id="9cc54-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9cc54-128">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="9cc54-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9cc54-129">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="9cc54-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9cc54-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_permission"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/permissions/{perm-id}
Content-type: application/json

{
  "roles": [ "read" ]
}
```
##### <span data-ttu-id="9cc54-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="9cc54-131">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="9cc54-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9cc54-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "read" ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update permission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Update permission"
}-->
