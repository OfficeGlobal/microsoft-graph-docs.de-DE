<span data-ttu-id="aa192-p105">Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (*time-to-live (ttl)*) des DNS-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="aa192-p105">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span>| Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (*time-to-live (ttl)*) des DNS-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu. |

## <span data-ttu-id="aa192-140">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="aa192-140">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="aa192-141">Keine</span><span class="sxs-lookup"><span data-stu-id="aa192-141">None</span></span>

## <span data-ttu-id="aa192-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aa192-142">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="aa192-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aa192-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->