# <a name="filterdatetime-resource-type"></a>FilterDatetime-Ressourcentyp

Stellt dar, wie ein Datum beim Filtern nach Werten gefiltert wird.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|date|Zeichenfolge|Das Datum im ISO8601-Format zum Filtern von Daten.|
|specificity|Zeichenfolge|Wie spezifisch die Daten bestimmt werden sollen, um die Daten zu halten. Angenommen, das Datum ist der 02.04.2005 und die Spezifität wird auf „Monat“ festgelegt, hält der Filter-Vorgang alle Zeilen mit einem Datum im Monat April 2009. Die mögliche Werte sind: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->