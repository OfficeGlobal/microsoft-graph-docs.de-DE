<a id="pivottable-resource-type" class="xliff"></a>
# Ressourcentyp pivotTable

Stellt eine Excel-PivotTable dar.

<a id="methods" class="xliff"></a>
## Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[workbookPivotTable abrufen](../api/workbookpivottable_get.md) | [workbookPivotTable](workbookpivottable.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des workbookPivotTable-Objekts.|
|[Aktualisieren](../api/workbookpivottable_refresh.md)|Keine|Aktualisiert die PivotTable. |
|[Refreshall](../api/workbookpivottable_refreshall.md)|Keine|Aktualisiert alle Tabellen im gegebenen Arbeitsblatt. Beachten Sie, dass diese Aktion nur für die PivotTable-Sammlung verfügbar ist.|

<a id="properties" class="xliff"></a>
## Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Die ID der PivotTable.   Schreibgeschützt.|
|name|String|Der Name der PivotTable.    |

<a id="relationships" class="xliff"></a>
## Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Arbeitsblatt|[Arbeitsblatt](worksheet.md)| Das Arbeitsblatt, das die aktuelle PivotTable enthält. Schreibgeschützt.   |

<a id="json-representation" class="xliff"></a>
## JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
