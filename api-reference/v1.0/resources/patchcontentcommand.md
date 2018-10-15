# <a name="patchcontentcommand-resource-type"></a>patchContentCommand-Ressourcentyp

Die an einer OneNote-Seite vorzunehmenden Änderungen in einer PATCH-Anforderung.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource, die im Text der Anforderung [PATCH pages/{id}`](../api/page_update.md) gesendet wird. 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Aktion|onenotePatchActionType|Die auf das Zielelement anzuwendende Aktion. Die möglichen Werte sind: `replace`, `append`, `delete`, `insert`, oder`prepend`.|
|Inhalt|Zeichenfolge|Eine Zeichenfolge aus wohlgeformtem HTML-Code, die der Seite hinzugefügt werden soll, sowie alle Bild- oder Dateibinärdaten. Wenn der Inhalt Binärdaten enthält, muss die Anforderung unter Verwendung des Inhaltstyps `multipart/form-data` mit der Komponente „Commands“ gesendet werden |
|Position|onenotePatchInsertPosition|Die Position, an der der angegebene Inhalt hinzugefügt werden soll, relativ zum Zielelement. Die möglichen Werte sind: `after` (Standard) oder `before`.|
|Ziel|Zeichenfolge|Das zu aktualisierende Element. Muss die `#<data-id>` oder die generierte `<id>` des Elements oder das Schlüsselwort `body` oder `title` sein.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
