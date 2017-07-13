<span data-ttu-id="76e63-p102">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="76e63-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| <span data-ttu-id="76e63-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="76e63-118">Property</span></span>     | <span data-ttu-id="76e63-119">Typ</span><span class="sxs-lookup"><span data-stu-id="76e63-119">Type</span></span>   |<span data-ttu-id="76e63-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="76e63-120">Description</span></span>|
|:---------------|:--------|:----------|

## <span data-ttu-id="76e63-121">Antwort</span><span class="sxs-lookup"><span data-stu-id="76e63-121">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="76e63-122">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte  [photo](../resources/photo.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="76e63-122">If successful, this method returns a `200 OK` response code and updated [photo](../resources/photo.md) object in the response body.</span></span>
## <span data-ttu-id="76e63-123">Beispiel</span><span class="sxs-lookup"><span data-stu-id="76e63-123">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="76e63-124">Anforderung</span><span class="sxs-lookup"><span data-stu-id="76e63-124">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="76e63-125">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="76e63-125">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_photo"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <span data-ttu-id="76e63-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="76e63-126">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="76e63-127">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="76e63-127">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
