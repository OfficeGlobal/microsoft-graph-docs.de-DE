<span data-ttu-id="92cd2-p107">Die Sammlung erweiterter einwertiger Eigenschaften, die für das mailFolder-Element definiert sind. Schreibgeschützt. Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="92cd2-p107">The collection of single-value extended properties defined for the mailFolder. Read-only. Nullable.</span></span>| Die Sammlung erweiterter einwertiger Eigenschaften, die für das mailFolder-Element definiert sind. Schreibgeschützt. Lässt Nullwerte zu.|


## <span data-ttu-id="92cd2-200">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="92cd2-200">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>

<span data-ttu-id="92cd2-201">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="92cd2-201">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailFolder"
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,

  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}

```

## <span data-ttu-id="92cd2-202">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="92cd2-202">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="92cd2-203">Verwenden einer Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten</span><span class="sxs-lookup"><span data-stu-id="92cd2-203">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="92cd2-204">Inkrementelle Änderungen an Nachrichten in einem Ordner abrufen</span><span class="sxs-lookup"><span data-stu-id="92cd2-204">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
