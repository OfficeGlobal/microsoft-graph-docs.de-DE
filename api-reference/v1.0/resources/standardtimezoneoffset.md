# <a name="standardtimezoneoffset-resource-type"></a>standardTimeZoneOffset-Ressourcentyp

Gibt an, wann eine Zeitzone von Sommerzeit in Standardzeit wechselt.

Wenn eine Zeitzone beispielsweise mit den folgenden Eigenschaften angegeben wird:

- **dayOccurrence** ist 3
- **dayOfWeek** ist „Sonntag“
- **month** ist 10
- **time** 02:00:00 _ ist **year** ist 0. Dies bedeutet, dass der Übergang von Sommerzeit zu Standardzeit jedes Jahr um 2 Uhr am dritten Sonntag im Oktober stattfindet.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| dayOccurrence | Edm.Int32 | Stellt das n-te Vorkommen des Wochentags dar, an dem der Übergang von Sommerzeit zu Standardzeit erfolgt. |
| dayOfWeek | dayOfWeek | Stellt den Wochentag dar, an dem der Übergang von Sommerzeit zu Standardzeit erfolgt. |
| month | Edm.Int32 | Stellt den Monat dar, an dem der Übergang von Sommerzeit zu Standardzeit erfolgt. |
| time | Edm.TimeOfDay | Stellt die Uhrzeit dar, zu der der Übergang von Sommerzeit zu Standardzeit erfolgt. |
| year | Edm.Int32 | Stellt dar, wie häufig der Wechsel von Sommerzeit zu Standardzeit in einem Jahr erfolgt. Der Wert 0 bedeutet z. B. jedes Jahr.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.standardTimeZoneOffset"
}-->

```json
{
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->