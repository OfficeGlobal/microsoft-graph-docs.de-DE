<span data-ttu-id="33c3e-p103">Hierdurch wird der Typ der Vorschau festgelegt, die für die Aufgabe angezeigt wird. Mögliche Werte: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Bei Festlegung auf `automatic` wird die angezeigte Vorschau von der App ausgewählt, mit der die Aufgabe angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="33c3e-p103">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|Hierdurch wird der Typ der Vorschau festgelegt, die für die Aufgabe angezeigt wird. Mögliche Werte: `automatic`, `noPreview`, `checklist`, `description`, `reference`. Bei Festlegung auf `automatic` wird die angezeigte Vorschau von der App ausgewählt, mit der die Aufgabe angezeigt wird.|
|<span data-ttu-id="33c3e-135">references</span><span class="sxs-lookup"><span data-stu-id="33c3e-135">references</span></span>|[<span data-ttu-id="33c3e-136">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="33c3e-136">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="33c3e-137">Die Sammlung der Verweise für die Aufgabe.</span><span class="sxs-lookup"><span data-stu-id="33c3e-137">The collection of references on the task.</span></span>|

## <span data-ttu-id="33c3e-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="33c3e-138">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="33c3e-139">Keine</span><span class="sxs-lookup"><span data-stu-id="33c3e-139">None</span></span>


## <span data-ttu-id="33c3e-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="33c3e-140">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="33c3e-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="33c3e-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->