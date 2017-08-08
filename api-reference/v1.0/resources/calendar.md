<span data-ttu-id="ec7de-p111">Die Sammlung erweiterter einwertiger Eigenschaften, die für den Kalender definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.</span><span class="sxs-lookup"><span data-stu-id="ec7de-p111">The collection of single-value extended properties defined for the calendar. Read-only. Nullable.</span></span>| Die Sammlung erweiterter einwertiger Eigenschaften, die für den Kalender definiert sind. Schreibgeschützt. Lässt NULL-Werte zu.|

## <a name="json-representation"></a><span data-ttu-id="ec7de-206">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ec7de-206">JSON representation</span></span>

<span data-ttu-id="ec7de-207">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ec7de-207">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendar"
}-->

```json
{
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "id": "string (identifier)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
