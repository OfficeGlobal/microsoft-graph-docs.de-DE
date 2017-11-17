<span data-ttu-id="e2299-p104">Hinweiswert, der verwendet wird, um die Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board anzuordnen, wenn die Aufgabe keinem Benutzer zugewiesen ist oder wenn das orderHintsByAssignee-Wörterbuch keinen Anordnungshinweis für den Benutzer enthält, dem die Aufgabe zugewiesen ist. Das Format ist wie [hier](planner_order_hint_format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="e2299-p104">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner_order_hint_format.md).</span></span>|Hinweiswert, der verwendet wird, um die Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board anzuordnen, wenn die Aufgabe keinem Benutzer zugewiesen ist oder wenn das orderHintsByAssignee-Wörterbuch keinen Anordnungshinweis für den Benutzer enthält, dem die Aufgabe zugewiesen ist. Das Format ist wie [hier](planner_order_hint_format.md) beschrieben definiert.|

## <span data-ttu-id="e2299-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e2299-133">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="e2299-134">Keine</span><span class="sxs-lookup"><span data-stu-id="e2299-134">None</span></span>


## <span data-ttu-id="e2299-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e2299-135">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="e2299-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e2299-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->