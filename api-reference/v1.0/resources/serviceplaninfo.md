<span data-ttu-id="8dbdb-p103">Das Objekt, dem der Serviceplan zugewiesen werden kann. Mögliche Werte:</span><span class="sxs-lookup"><span data-stu-id="8dbdb-p103">The object the service plan can be assigned to. Possible values:</span></span>|Das Objekt, dem der Serviceplan zugewiesen werden kann. Mögliche Werte:<br/><span data-ttu-id="8dbdb-127">„User“ - Der Serviceplan kann einzelnen Benutzern zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="8dbdb-127">"User" - service plan can be assigned to individual users.</span></span><br/><span data-ttu-id="8dbdb-128">„Company“ - Der Serviceplan kann dem gesamten Mandanten zugewiesen werden.</span><span class="sxs-lookup"><span data-stu-id="8dbdb-128">"Company" - service plan can be assigned to the entire tenant.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="8dbdb-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8dbdb-129">JSON representation</span></span>

<span data-ttu-id="8dbdb-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8dbdb-130">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.servicePlanInfo"
}-->

```json
{
  "appliesTo": "string",
  "provisioningStatus": "string",
  "servicePlanId": "guid",
  "servicePlanName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePlanInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
