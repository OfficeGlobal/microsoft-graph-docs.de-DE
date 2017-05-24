# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a>plannerAssignedToTaskBoardTaskFormat-Ressourcentyp

Die **plannerAssignedToTaskBoardTaskFormat** Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board verwendet werden (eine Ansicht, die nach Benutzern organisiert ist, denen Aufgaben zugewiesen sind). Jeder [Aufgabe](plannertask.md) ist ein **plannerAssignedToTaskBoardTaskFormat**-Objekt zugeordnet.


### <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[plannerAssignedToTaskBoardTaskFormat abrufen](../api/plannerassignedtotaskboardtaskformat_get.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) |Dient zum Lesen der Eigenschaften und Beziehungen eines **PlannerAssignedToTaskBoardTaskFormat**-Objekts.|
|[Update](../api/plannerassignedtotaskboardtaskformat_update.md) | [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)    |Dient zum Aktualisieren eines **plannerAssignedToTaskBoardTaskFormat**-Objekts. |

### <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Schreibgeschützt. ID der Ressource. Sie ist 28 Zeichen lang, und es wird zwischen Groß-und Kleinschreibung unterschieden. Für den Dienst wird eine [Formatüberprüfung](planner_identifiers_disclaimer.md) durchgeführt.|
|orderHintsByAssignee|[plannerOrderHintsByAssignee](plannerorderhintsbyassignee.md)|Wörterbuch von Hinweisen, die verwendet werden, um Aufgaben in der Ansicht „ZugewiesenAn“ des Task Board anzuordnen. Der Schlüssel für jeden Eintrag ist einer der Benutzer, denen die Aufgabe zugewiesen ist, und der Wert ist der Anordnungshinweis. Das Format der einzelnen Werte ist wie [hier](planner_order_hint_format.md) beschrieben definiert.|
|unassignedOrderHint|String|Hinweiswert, der verwendet wird, um die Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board anzuordnen, wenn die Aufgabe keinem Benutzer zugewiesen ist oder wenn das orderHintsByAssignee-Wörterbuch keinen Anordnungshinweis für den Benutzer enthält, dem die Aufgabe zugewiesen ist. Das Format ist wie [hier](planner_order_hint_format.md) beschrieben definiert.|

### <a name="relationships"></a>Beziehungen
Keine


### <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->