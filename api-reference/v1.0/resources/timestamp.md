# <a name="timestamp-resource-type"></a>Zeitstempel Ressourcentyp

Datums- und Zeitangaben für einen bestimmten Zeitpunkt

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|date|Datum|Der Datumsteil des Zeitstempels.|
|time|TimeOfDay|Der Uhrzeitteil des Zeitstempels.|
|timeZone|Zeichenfolge|Der Zeitzonenteil des Zeitstempels, der eine der 24 Zeitzonen der Welt bezeichnet.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->