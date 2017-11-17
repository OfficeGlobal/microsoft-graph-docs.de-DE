<span data-ttu-id="a614a-p105">Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (*time-to-live (ttl)*) des SRV-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="a614a-p105">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span>| Wert, der beim Konfigurieren der Eigenschaft für die Gültigkeitsdauer (*time-to-live (ttl)*) des SRV-Eintrags auf dem DNS-Host verwendet werden soll. Lässt keine Nullwerte zu. |
|<span data-ttu-id="a614a-149">weight</span><span class="sxs-lookup"><span data-stu-id="a614a-149">weight</span></span>|<span data-ttu-id="a614a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a614a-150">Int32</span></span>| <span data-ttu-id="a614a-151">Wert, der beim Konfigurieren der *weight*-Eigenschaft des SRV-Eintrags auf dem DNS-Host verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="a614a-151">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <span data-ttu-id="a614a-152">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a614a-152">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="a614a-153">Keine</span><span class="sxs-lookup"><span data-stu-id="a614a-153">None</span></span>


## <span data-ttu-id="a614a-154">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a614a-154">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="a614a-155">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a614a-155">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->