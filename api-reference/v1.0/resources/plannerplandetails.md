# plannerPlanDetails-Ressourcentyp
<a id="plannerplandetails-resource-type" class="xliff"></a>


Die **plannerPlanDetails**-Ressource stellt die zusätzlichen Informationen zu einem Plan dar. Jedes [plan](plannerplan.md)-Objekt hat ein Detailobjekt.


## Methoden
<a id="methods" class="xliff"></a>

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[plannerPlanDetails abrufen](../api/plannerplandetails_get.md) | [plannerPlanDetails](plannerplandetails.md) |Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerPlanDetails**-Objekts.|
|[Update](../api/plannerplandetails_update.md) | [plannerPlanDetails](plannerplandetails.md)    |Dient zum Aktualisieren des **plannerPlanDetails**-Objekts. |


## Eigenschaften
<a id="properties" class="xliff"></a>
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|categoryDescriptions|[plannerCategoryDescriptions](plannercategorydescriptions.md)|Ein Objekt, das die Beschreibungen der sechs Kategorien angibt, die den Aufgaben im Plan zugeordnet werden können.|
|id|String| Schreibgeschützt. ID der Plandetails. Sie ist 28 Zeichen lang, und es wird zwischen Groß-und Kleinschreibung unterschieden. Für den Dienst wird eine [Formatüberprüfung](planner_identifiers_disclaimer.md) durchgeführt.|
|sharedWith|[plannerUserIds](planneruserids.md)|Der Satz von Benutzer-IDs, für die dieser Plan freigegeben ist. Wenn Sie Office 365 Gruppen nutzen, verwenden Sie die Gruppen-API zum Verwalten von Gruppenmitgliedschaften, um den Plan der [Gruppe](group.md) freizugeben. Sie können auch vorhandene Mitglieder der Gruppe zu dieser Sammlung hinzufügen, dies ist jedoch nicht erforderlich, damit sie auf den im Besitz der Gruppe befindlichen Plan zugreifen können. |

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
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}-->

```json
{
  "categoryDescriptions": {"@odata.type": "microsoft.graph.plannerCategoryDescriptions"},
  "id": "String (identifier)",
  "sharedWith": {"@odata.type": "microsoft.graph.plannerUserIds"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->