# extensionSchemaProperty-Ressourcentyp
<a id="extensionschemaproperty-resource-type" class="xliff"></a>

Verwenden Sie die **extensionSchemaProperty**-Ressource, um den Namen und den Typ einer Eigenschaft im Rahmen einer [schemaExtension](schemaextension.md)-Definition zu definieren.


## Eigenschaften
<a id="properties" class="xliff"></a>
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|name|String| Der Name der stark typisierten Eigenschaft, die im Rahmen der Schemaerweiterung definiert wird.|
|type|String| Der Typ der Eigenschaft, die im Rahmen der Schemaerweiterung definiert wird.  Zulässige Werte sind *Binary, Boolean, DateTime, Integer* oder *String*.  Weitere Einzelheiten finden Sie in der Tabelle unten.|

#### Unterstützte Datentypen für Eigenschaften
<a id="supported-property-data-types" class="xliff"></a> 
Die folgenden Datentypen werden beim Definieren einer Eigenschaft in einer Schemaerweiterung unterstützt:

| Eigenschaftentyp | Bemerkungen |
|-------------|------------|
| Binär | Maximal 256 Bytes. |
| Boolescher Wert | Nicht unterstützt für Nachrichten, Ereignisse und Beiträge. |
| DateTime | Muss im ISO 8601-Format angegeben werden. Wird in UTC gespeichert. |
| Ganze Zahl | 32-Bit-Wert. Nicht unterstützt für Nachrichten, Ereignisse und Beiträge. |
| Zeichenfolge | Maximal 256 Zeichen. |

## JSON-Darstellung
<a id="json-representation" class="xliff"></a>
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extensionSchemaProperty"
}-->

```json
{
  "name": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extensionSchemaProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->