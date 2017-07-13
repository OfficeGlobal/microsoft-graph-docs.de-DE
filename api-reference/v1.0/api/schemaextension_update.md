<span data-ttu-id="731e6-p107">Satz von Microsoft Graph-Typen (die Erweiterungen unterstützen können), auf die die Schemaerweiterung angewendet werden kann.  Nur additive Änderungen sind zulässig.</span><span class="sxs-lookup"><span data-stu-id="731e6-p107">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span>|Satz von Microsoft Graph-Typen (die Erweiterungen unterstützen können), auf die die Schemaerweiterung angewendet werden kann.  Nur additive Änderungen sind zulässig.|

## <span data-ttu-id="731e6-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="731e6-142">Response</span></span>
<a id="response" class="xliff"></a>

<span data-ttu-id="731e6-143">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="731e6-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <span data-ttu-id="731e6-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="731e6-144">Example</span></span>
<a id="example" class="xliff"></a>

##### <span data-ttu-id="731e6-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="731e6-145">Request</span></span>
<a id="request" class="xliff"></a>

<span data-ttu-id="731e6-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="731e6-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ],
}
```

##### <span data-ttu-id="731e6-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="731e6-147">Response</span></span>
<a id="response" class="xliff"></a>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <span data-ttu-id="731e6-148">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="731e6-148">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="731e6-149">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="731e6-149">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="731e6-150">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="731e6-150">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->