<span data-ttu-id="87c81-p123">Ein Zeichenfolgenwert kann zum Klassifizieren der Benutzertypen in Ihrem Verzeichnis verwendet werden, z. B. „Member“ und „Guest“. Unterstützt $filter.</span><span class="sxs-lookup"><span data-stu-id="87c81-p123">A string value that can be used to classify user types in your directory, such as “Member” and “Guest”. Supports $filter.</span></span>|Ein Zeichenfolgenwert kann zum Klassifizieren der Benutzertypen in Ihrem Verzeichnis verwendet werden, z. B. „Member“ und „Guest“. Unterstützt $filter.          |

## <span data-ttu-id="87c81-261">Antwort</span><span class="sxs-lookup"><span data-stu-id="87c81-261">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="87c81-262">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87c81-262">If successful, this method returns a `204 No Content` response code.</span></span>
## <span data-ttu-id="87c81-263">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87c81-263">Example</span></span>
<a id="example" class="xliff"></a>
##### <span data-ttu-id="87c81-264">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87c81-264">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="87c81-265">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87c81-265">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_user"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me
Content-type: application/json
Content-length: 491

{
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "disabledPlans": [ "bea13e0c-3828-4daa-a392-28af7ff61a0f" ],
      "skuId": "skuId-value"
    }
  ],
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "companyName": "companyName-value"
}
```
##### <span data-ttu-id="87c81-266">Antwort</span><span class="sxs-lookup"><span data-stu-id="87c81-266">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="87c81-267">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="87c81-267">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
