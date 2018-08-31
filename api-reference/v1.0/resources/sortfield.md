# <a name="sortfield-resource-type"></a>SortField-Ressourcentyp

Stellt eine Bedingung in einem Sortiervorgang dar.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|aufsteigend|boolesch|Stellt dar, ob die Sortierung in aufsteigender Reihenfolge ausgeführt wird.|
|Farbe|Zeichenfolge|Stellt die Farbe dar, die das Ziel der Bedingung ist, wenn die Sortierung für die Schrift- oder Zellenfarbe gilt.|
|dataOption|Zeichenfolge|Stellt weitere Sortieroptionen für dieses Feld dar. Mögliche Werte sind: `Normal`, `TextAsNumber`.|
|Schlüssel|int|Stellt die Spalte (oder Zeile, je nach Sortierausrichtung) dar, für die die Bedingung gilt. Wird als Offset von der ersten Spalte (oder Zeile) dargestellt.|
|sortOn|Zeichenfolge|Stellt den Typ der Sortierung dieser Bedingung dar. Mögliche Werte sind: `Value`, `CellColor`, `FontColor`, `Icon`.|
|Symbol|[WorkbookIcon](icon.md)|Stellt das Symbol dar, welches das Ziel der Bedingung ist, wenn die Sortierung für das Symbol der Zelle gilt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->