# <a name="plannerprogresstaskboardtaskformat-resource-type"></a>plannerProgressTaskBoardTaskFormat-Ressourcentyp

Die **plannerProgressTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Fortschritt“ des Task Board verwendet werden (eine Ansicht, die nach dem Status des Felds „ProzentAbgeschlossen“ für das Aufgabenobjekt sortiert ist und Spalten für „Nicht gestartet“, „In Bearbeitung“ und „Abgeschlossen“ enthält). Jeder [Aufgabe](plannertask.md) ist ein **plannerProgressTaskBoardTaskFormat**-Objekt zugeordnet.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[plannerProgressTaskBoardTaskFormat abrufen](../api/plannerprogresstaskboardtaskformat_get.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md) |Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerProgressTaskBoardTaskFormat**-Objekts.|
|[Aktualisieren](../api/plannerprogresstaskboardtaskformat_update.md) | [plannerProgressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)    |Dient zum Aktualisieren des **plannerProgressTaskBoardTaskFormat**-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|Zeichenfolge| Schreibgeschützt. Die ID der Ressource. Sie ist 28 Zeichen lang und berücksichtigt Groß-/Kleinschreibung. [Formatvalidierung](planner_identifiers_disclaimer.md) erfolgt für den Dienst.|
|orderHint|Zeichenfolge|Hinweiswert, der verwendet wird, um die Aufgaben in der Ansicht „Fortschritt“ des Task Board anzuordnen. Das Format ist wie [hier](planner_order_hint_format.md) beschrieben definiert.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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