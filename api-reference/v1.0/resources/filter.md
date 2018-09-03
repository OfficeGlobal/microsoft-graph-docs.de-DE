# <a name="filter-resource-type"></a>Filter-Ressourcentyp

Verwaltet das Filtern der Spalte einer Tabelle.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Anwenden](../api/filter_apply.md)|Keine|Wendet die angegebenen Filterkriterien in der angegebenen Spalte an.|
|[Löschen](../api/filter_clear.md)|Keine|Deaktiviert den Filter für die angegebene Spalte.|

## <a name="properties"></a>Eigenschaften

| Name | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Kriterien|[WorkbookFilterCriteria](filtercriteria.md)|Der aktuell angewendete Filter in der angegebenen Spalte. Schreibgeschützt.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
  "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->