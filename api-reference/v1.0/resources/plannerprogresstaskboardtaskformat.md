# plannerProgressTaskBoardTaskFormat-Ressourcentyp
<a id="plannerprogresstaskboardtaskformat-resource-type" class="xliff"></a>

Die **plannerProgressTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Fortschritt“ des Task Board verwendet werden (eine Ansicht, die nach dem Status des Felds „ProzentAbgeschlossen“ für das Aufgabenobjekt sortiert ist und Spalten für „Nicht gestartet“, „In Bearbeitung“ und „Abgeschlossen“ enthält). Jeder [Aufgabe](plannertask.md) ist ein **plannerProgressTaskBoardTaskFormat**-Objekt zugeordnet.


## Methoden
<a id="methods" class="xliff"></a>

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[plannerProgressTaskBoardTaskFormat abrufen](../api/plannerprogresstaskboardtaskformat_get.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) |Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerProgressTaskBoardTaskFormat**-Objekts.|
|[Update](../api/plannerprogresstaskboardtaskformat_update.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)    |Dient zum Aktualisieren des **plannerProgressTaskBoardTaskFormat**-Objekts. |

## Eigenschaften
<a id="properties" class="xliff"></a>
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Schreibgeschützt. ID der Ressource. Sie ist 28 Zeichen lang, und es wird zwischen Groß-und Kleinschreibung unterschieden. Für den Dienst wird eine [Formatüberprüfung](planner_identifiers_disclaimer.md) durchgeführt.|
|orderHint|String|Hinweiswert, der verwendet wird, um die Aufgaben in der Ansicht „Fortschritt“ des Task Board anzuordnen. Das Format ist wie [hier](planner_order_hint_format.md) beschrieben definiert.|

## Beziehungen
<a id="relationships" class="xliff"></a>
Keine


## JSON-Darstellung
<a id="json-representation" class="xliff"></a>
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->