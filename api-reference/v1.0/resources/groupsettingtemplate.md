<span data-ttu-id="08ab4-p102">Der eindeutige Bezeichner für die Vorlage. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="08ab4-p102">Unique identifier for the subscription. Read-only.</span></span>| Der eindeutige Bezeichner für die Vorlage. Schreibgeschützt.|
|<span data-ttu-id="08ab4-131">values</span><span class="sxs-lookup"><span data-stu-id="08ab4-131">values</span></span>|<span data-ttu-id="08ab4-132">[settingTemplateValue](settingtemplatevalue.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="08ab4-132">[settingTemplateValue](settingtemplatevalue.md) collection</span></span>| <span data-ttu-id="08ab4-133">Sammlung von settingTemplateValues, die den Satz der verfügbaren Einstellungen, Standardwerte und Typen auflistet, die diese Vorlage bilden.</span><span class="sxs-lookup"><span data-stu-id="08ab4-133">Collection of settingTemplateValues that list the set of available settings, defaults and types that make up this template.</span></span> |

## <a name="relationships"></a><span data-ttu-id="08ab4-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="08ab4-134">Relationships</span></span>

<span data-ttu-id="08ab4-135">Keine.</span><span class="sxs-lookup"><span data-stu-id="08ab4-135">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="08ab4-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="08ab4-136">JSON representation</span></span>

<span data-ttu-id="08ab4-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="08ab4-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->