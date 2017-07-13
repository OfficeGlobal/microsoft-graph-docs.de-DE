<span data-ttu-id="a3d66-p104">Eindeutiger SKU-Anzeigename. Entspricht der skuPartNumber des zugehörigen [SubscribedSku](subscribedsku.md)-Objekts, z. B.: „AAD_Premium“. Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="a3d66-p104">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span>| Eindeutiger SKU-Anzeigename. Entspricht der skuPartNumber des zugehörigen [SubscribedSku](subscribedsku.md)-Objekts, z. B.: „AAD_Premium“. Schreibgeschützt |

## <span data-ttu-id="a3d66-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a3d66-132">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="a3d66-133">Keine</span><span class="sxs-lookup"><span data-stu-id="a3d66-133">None</span></span>

## <span data-ttu-id="a3d66-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a3d66-134">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="a3d66-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a3d66-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->