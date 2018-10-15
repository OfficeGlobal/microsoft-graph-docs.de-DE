# <a name="plannerplan-resource-type"></a>plannerPlan-Ressourcentyp

Die **plannerPlan**-Ressource stellt einen Plan in Office 365 dar. Ein Plan kann im Besitz einer [Gruppe](group.md) sein und enthält eine Sammlung von [plannerTasks](plannerTask.md). Er kann auch über eine Sammlung von [plannerBuckets](plannerBucket.md) verfügen. Jedes Planobjekt verfügt über [details](plannerPlanDetails.md)-Objekt, das weitere Informationen über den Plan enthalten kann. Weitere Informationen zu den Beziehungen zwischen Gruppen, Plänen und Aufgaben finden Sie unter [Planner](planner_overview.md).

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[plannerPlan abrufen](../api/plannerplan_get.md) | [plannerPlan](plannerplan.md) |Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerPlan**-Objekts.|
|[Buckets auflisten](../api/plannerplan_list_buckets.md) |[plannerBucket](plannerbucket.md)-Sammlung| Dient zum Abrufen einer **plannerBucket**-Objektsammlung.|
|[Aufgaben auflisten](../api/plannerplan_list_tasks.md) |[plannerTask](plannertask.md)-Sammlung| Dient zum Abrufen einer **plannerTask**-Objektsammlung.|
|[Aktualisieren](../api/plannerplan_update.md) | [plannerPlan](plannerplan.md) |Dient zum Aktualisieren eines **plannerPlan**-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|createdDateTime|DateTimeOffset|Schreibgeschützt. Datum und Uhrzeit der Erstellung des Plans. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|id|Zeichenfolge| Schreibgeschützt. ID des Plans. Sie ist 28 Zeichen lang und berücksichtigt Groß-/Kleinschreibung. Die [Formatvalidierung](planner_identifiers_disclaimer.md) erfolgt für den Dienst.|
|owner|Zeichenfolge|ID der [Gruppe](group.md), die den Plan besitzt. Dieses Feld kann erst festgelegt werden, wenn eine gültige Gruppe vorhanden ist. Nachdem dieses festgelegt wurde, kann es nur noch vom Besitzer aktualisiert werden.|
|title|Zeichenfolge|Erforderlich.  Der Titel des Plans.|
|createdBy|[identitySet](identityset.md)|Schreibgeschützt. Der Benutzer, der den Plan erstellt hat.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|buckets|[plannerBucket](plannerbucket.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Sammlung von Buckets im Plan.|
|Details|[plannerPlanDetails](plannerplandetails.md)| Schreibgeschützt. Lässt Nullwerte zu. Weitere Details über den Plan.|
|tasks|[plannerTask](plannertask.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Sammlung von Aufgaben im Plan.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlan"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "owner": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->