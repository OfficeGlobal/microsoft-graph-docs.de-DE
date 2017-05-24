# <a name="planneruser-resource-type"></a>plannerUser-Ressourcentyp

Die **plannerUser**-Ressource bietet einem [Benutzer](user.md) Zugriff auf Planner-Ressourcen. Sie enthält keine verwendbaren Eigenschaften.


### <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Pläne auflisten](../api/planneruser_list_plans.md) |[plannerPlan](plannerplan.md)-Sammlung| Dient zum Abrufen einer **plannerPlan**-Objektsammlung.|
|[Aufgaben auflisten](../api/planneruser_list_tasks.md) |[plannerTask](plannertask.md)-Sammlung| Dient zum Abrufen einer **plannerTask**-Objektsammlung.|

### <a name="properties"></a>Eigenschaften
| Eigenschaft       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Schreibgeschützt. Bezeichner der plannerUser-Ressource.|

### <a name="relationships"></a>Beziehungen
| Beziehung | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|plans|[plannerPlan](plannerplan.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Gibt die dem Benutzer zugewiesenen [plannerTasks](plannertask.md) zurück.|
|tasks|[plannerTask](plannertask.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Gibt die für den Benutzer freigegebenen [plannerPlans](plannerplan.md) zurück.|

### <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUser"
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
  "description": "plannerUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->