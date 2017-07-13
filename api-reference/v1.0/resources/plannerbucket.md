# plannerBucket-Ressourcentyp
<a id="plannerbucket-resource-type" class="xliff"></a>

Die **plannerBucket**-Ressource stellt einen Bucket (bzw. eine „benutzerdefinierte Spalte“) für Aufgaben in einem Plan in Office 365 dar. Sie ist in einem [plannerPlan](plannerPlan.md) enthalten und kann eine Sammlung von [plannerTasks](plannerTask.md) haben.



## Methoden
<a id="methods" class="xliff"></a>

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[plannerBucket abrufen](../api/plannerbucket_get.md) | [plannerBucket](plannerbucket.md) |Dient zum Lesen der Eigenschaften und Beziehungen des **plannerBucket**-Objekts.|
|[plannerTasks auflisten](../api/plannerbucket_list_tasks.md) |[plannerTask](plannertask.md)-Sammlung| Dient zum Abrufen einer **plannerTask**-Objektsammlung.|
|[Create](../api/planner_post_buckets.md) | [plannerBucket](plannerbucket.md)   | Dient zum Erstellen eines neuen **plannerBucket**-Objekts. |
|[Update](../api/plannerbucket_update.md) | [plannerBucket](plannerbucket.md)   |Dient zum Aktualisieren eines **plannerBucket**-Objekts. |
|[Delete](../api/plannerbucket_delete.md) | Keine |Dient zum Löschen eines **plannerBucket**-Objekts. |

## Eigenschaften
<a id="properties" class="xliff"></a>
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|String| Schreibgeschützt. ID des Buckets. Sie ist 28 Zeichen lang, und es wird zwischen Groß-und Kleinschreibung unterschieden. Für den Dienst wird eine [Formatüberprüfung](planner_identifiers_disclaimer.md) durchgeführt.|
|name|String|Name des Buckets.|
|orderHint|String|Hinweis, der zum Anordnen von Elementen dieses Typs in einer Listenansicht verwendet wird. Das Format ist wie [hier](planner_order_hint_format.md) beschrieben definiert.|
|planId|String|Plan-ID, zu der der Bucket gehört.|

## Beziehungen
<a id="relationships" class="xliff"></a>
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|tasks|[plannerTask](plannertask.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Die Sammlung von Aufgaben im Bucket.|

## JSON-Darstellung
<a id="json-representation" class="xliff"></a>
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->