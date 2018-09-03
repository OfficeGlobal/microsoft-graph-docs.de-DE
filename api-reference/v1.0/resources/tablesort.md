# <a name="tablesort-resource-type"></a>TableSort-Ressourcentyp

Verwaltet Sortiervorgänge für Table-Objekte.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Get TableSort](../api/tablesort_get.md) | [WorkbookTableSort](tablesort.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des tableSort-Objekts.|
|[Anwenden](../api/tablesort_apply.md)|Keine|Führt einen Sortiervorgang aus.|
|[Löschen](../api/tablesort_clear.md)|Keine|Löscht die Sortierung, die derzeit in der Tabelle enthalten ist. Dies ändert nicht die Sortierung der Tabelle, löscht jedoch den Zustand der Kopfzeilen-Schaltflächen.|
|[Reapply](../api/tablesort_reapply.md)|Keine|Wendet die aktuellen Sortierparameter erneut auf die Tabelle an.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|fields|[WorkbookSortField](sortfield.md)-Sammlung|Stellt die aktuellen Bedingungen dar, die zuletzt zum Sortieren der Tabelle verwendet wurden. Schreibgeschützt.|
|matchCase|boolescher Wert|Stellt dar, ob die Groß-/Kleinschreibung den letzten Sortiervorgang der Tabelle beeinflusst hat. Schreibgeschützt.|
|method|Zeichenfolge|Stellt die Sortiermethode für chinesische Zeichen dar, die zuletzt verwendet wurde, um die Tabelle zu sortieren. Die möglichen Werte sind: `PinYin`, `StrokeCount`. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->