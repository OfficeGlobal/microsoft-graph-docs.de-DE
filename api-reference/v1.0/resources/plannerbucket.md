# <a name="plannerbucket-resource-type"></a>plannerBucket-Ressourcentyp

Die **plannerBucket**-Ressource stellt einen Bucket (bzw. eine „benutzerdefinierte Spalte“) für Aufgaben in einem Plan in Office 365 dar. Sie ist in einem [plannerPlan](plannerPlan.md) enthalten und kann eine Sammlung von [plannerTasks](plannerTask.md) haben.



## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[plannerBucket abrufen](../api/plannerbucket_get.md) | [plannerBucket](plannerbucket.md) |Dient zum Lesen der Eigenschaften und Beziehungen des **plannerBucket**-Objekts.|
|[plannerTasks auflisten](../api/plannerbucket_list_tasks.md) |[plannerTask](plannertask.md)-Sammlung| Dient zum Abrufen einer **plannerTask**-Objektsammlung.|
|[Erstellen](../api/planner_post_buckets.md) | [plannerBucket](plannerbucket.md)   | Dient zum Erstellen eines neuen **plannerBucket**-Objekts. |
|[Aktualisieren](../api/plannerbucket_update.md) | [plannerBucket](plannerbucket.md)   |Dient zum Aktualisieren eines **plannerBucket**-Objekts. |
|[Löschen](../api/plannerbucket_delete.md) | Keine |Dient zum Löschen eines **plannerBucket**-Objekts. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|ID|Zeichenfolge| Schreibgeschützt. ID des Buckets. Er ist 28 Zeichen lang und beachtet Groß-/Kleinschreibung. [Formatvalidierung](planner_identifiers_disclaimer.md) erfolgt für den Dienst.|
|Name|Zeichenfolge|Name des Buckets.|
|orderHint|Zeichenfolge|Hinweis, der zum Anordnen von Elementen dieses Typs in einer Listenansicht verwendet wird. Das Format ist wie [hier](planner_order_hint_format.md) beschrieben definiert.|
|planId|Zeichenfolge|Plan-ID, zu der der Bucket gehört.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Aufgaben|[plannerTask](plannertask.md)-Sammlung| Schreibgeschützt. Lässt Nullwerte zu. Die Sammlung von Aufgaben im Bucket.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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