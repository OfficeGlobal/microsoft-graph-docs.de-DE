<span data-ttu-id="6bd18-p104">Wird verwendet, um die relative Reihenfolge der Elemente in der Checkliste festzulegen. Das Format ist wie [hier](planner_order_hint_format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="6bd18-p104">Used to set the relative order of items in the checklist. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|Wird verwendet, um die relative Reihenfolge der Elemente in der Checkliste festzulegen. Das Format ist wie [hier](planner_order_hint_format.md) beschrieben definiert.|
|<span data-ttu-id="6bd18-125">title</span><span class="sxs-lookup"><span data-stu-id="6bd18-125">title</span></span>|<span data-ttu-id="6bd18-126">String</span><span class="sxs-lookup"><span data-stu-id="6bd18-126">String</span></span>|<span data-ttu-id="6bd18-127">Titel des Checklistenelements.</span><span class="sxs-lookup"><span data-stu-id="6bd18-127">Title of the checklist item</span></span>|

## <span data-ttu-id="6bd18-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6bd18-128">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="6bd18-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6bd18-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->