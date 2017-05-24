# <a name="planner-resource-type"></a>planner-Ressourcentyp

Die **planner**-Ressource ist der Einstiegspunkt für das Planner-Objektmodell. Sie gibt eine Singleton **planner**-Ressource zurück.  Sie enthält keine verwendbaren Eigenschaften.


### <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[plannerBucket erstellen](../api/planner_post_buckets.md) |[plannerBucket](plannerbucket.md)| Dient zum Erstellen eines neuen **plannerBucket** durch Veröffentlichung in der buckets-Sammlung.|
|[plannerPlan erstellen](../api/planner_post_plans.md) |[plannerPlan](plannerplan.md)| Dient zum Erstellen eines neuen **plannerPlan** durch Veröffentlichung in der plans-Sammlung.|
|[plannerTask erstellen](../api/planner_post_tasks.md) |[plannerTask](plannertask.md)| Dient zum Erstellen einer neuen **plannerTask** durch Veröffentlichung in der tasks-Sammlung.|

### <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Schreibgeschützt. Bezeichner der **planner**-Ressource.|

### <a name="relationships"></a>Beziehungen
| Beziehung | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|buckets|[plannerBucket](plannerbucket.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen einfaches zurück.|
|plans|[plannerPlan](plannerplan.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen Pläne zurück.|
|tasks|[plannerTask](plannertask.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Gibt eine Sammlung der angegebenen Aufgaben zurück.|

### <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.planner"
}-->

```json
{
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "planner resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->