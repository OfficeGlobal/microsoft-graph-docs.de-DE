# <a name="plannerbuckettaskboardtaskformat-resource-type"></a>plannerBucketTaskBoardTaskFormat-Ressourcentyp

Die **plannerBucketTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Buckets“ des Task Board verwendet werden (eine Ansicht, die nach den Aufgaben in den Buckets organisiert ist, denen sie zugewiesen sind). Jeder [Aufgabe](plannertask.md) ist ein **plannerBucketTaskBoardTaskFormat**-Objekt zugeordnet.


### <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[plannerBucketTaskBoardTaskFormat abrufen](../api/plannerbuckettaskboardtaskformat_get.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) |Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerBucketTaskBoardTaskFormat**-Objekts.|
|[Update](../api/plannerbuckettaskboardtaskformat_update.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)    |Dient zum Aktualisieren des **plannerBucketTaskBoardTaskFormat**-Objekts. |

### <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Schreibgeschützt. ID der Ressource. Sie ist 28 Zeichen lang, und es wird zwischen Groß-und Kleinschreibung unterschieden. Für den Dienst wird eine [Formatüberprüfung](planner_identifiers_disclaimer.md) durchgeführt.|
|orderHint|String|Hinweis, der zum Anordnen von Aufgaben in der Ansicht „Buckets“ des Task Board verwendet wird. Das Format ist wie [hier](planner_order_hint_format.md) beschrieben definiert.|

### <a name="relationships"></a>Beziehungen
Keine


### <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
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
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->