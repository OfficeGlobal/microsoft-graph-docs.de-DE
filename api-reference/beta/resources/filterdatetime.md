# <a name="filterdatetime-resource-type"></a>FilterDatetime-Ressourcentyp

Stellt dar, wie ein Datum beim Filtern nach Werten gefiltert wird.

## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|date|string|Das Datum im ISO8601-Format zum Filtern von Daten.|
|specificity|string|Genauigkeit des Datums zum Beibehalten von Daten. Wenn z. B. das Datum 2005-04-02 ist und die Spezifität auf „Monat“ festgelegt ist, werden beim Filtervorgang alle Zeilen mit einem Datum im Monat April 2009 beibehalten. Mögliche Werte:`Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterDateTime"
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