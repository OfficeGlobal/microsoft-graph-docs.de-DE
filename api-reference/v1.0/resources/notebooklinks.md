# <a name="notebooklinks-resource-type"></a>notebookLinks-Ressourcentyp

Links zum Öffnen eines OneNote-Notizbuchs.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|oneNoteClientUrl|[externalLink](externallink.md)|Öffnet das Notizbuch im systemeigenen OneNote-Client, sofern er installiert ist.|
|oneNoteWebUrl|[externalLink](externallink.md)|Öffnet das Notizbuch in OneNote Online.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->