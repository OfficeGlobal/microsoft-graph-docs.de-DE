# <a name="recurrencepattern-resource-type"></a>recurrencePattern-Ressourcentyp

Die Häufigkeit eines Ereignisses.


## <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|dayOfMonth|Int32|Der Tag des Monats, andem das Ereignis stattfindet.|
|daysOfWeek|String collection|Eine Auflistung der Tage der Woche, an denen das Ereignis stattfindet. Mögliche Werte: `Sunday`, `Monday`, `Tuesday`, `Wednesday`, `Thursday`, `Friday`, `Saturday`.|
|firstDayOfWeek|String|Der Tag der Woche, an dem die Serie beginnt. Mögliche Werte: `Sunday`, `Monday`, `Tuesday`, `Wednesday`, `Thursday`, `Friday`, `Saturday`.|
|Index|String|Der Index der Woche, an dem die Serie stattfindet.: `First`, `Second`, `Third`, `Fourth`, `Last`.|
|Intervall|Int32|Die Anzahl von Einheiten eines bestimmten Serientyps zwischen Vorkommen.|
|Monat|Int32|Der Monat, in dem das Ereignis stattfindet.  Dies ist eine Zahl zwischen 1 und 12.|
|type|String|Typ des Serienmusters: `Daily`, `Weekly`, `AbsoluteMonthly`, `RelativeMonthly`, `AbsoluteYearly`, `RelativeYearly`.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencepattern"
}-->

```json
{
  "dayOfMonth": 1024,
  "daysOfWeek": ["String"],
  "firstDayOfWeek": "String",
  "index": "String",
  "interval": 1024,
  "month": 1024,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrencePattern resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->