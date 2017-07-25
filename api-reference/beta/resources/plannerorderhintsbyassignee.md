# plannerOrderHintsByAssignee-Ressourcentyp
<a id="plannerorderhintsbyassignee-resource-type" class="xliff"></a>

Die **plannerOrderHintsByAssignee**-Ressource enthält [Anordnungshinweise](planner_order_hint_format.md) für zugewiesene Personen in einer [plannerTask](plannerTask.md)-Ressource, um die Anordnung der Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board anzugeben. Es handelt sich um einen offenen Typ. Die Eigenschaften sind die IDs der Benutzer, die der Aufgabe zugewiesen sind, und die Werte sind Anordnungshinweise.

## Eigenschaften
<a id="properties" class="xliff"></a>
Eigenschaften mit offenem Typ können vom Client definiert werden. In diesem Fall muss der Client IDs von Benutzern, die der Aufgabe zugewiesen sind, als Eigenschaftennamen und einen gültigen [Anordnungshinweis](planner_order_hint_format.md) als Wert angeben. Von diesem Typ können keine Eigenschaften entfernt werden. Der Dienst entfernt automatisch Werte, wenn die Zuweisungen in der enthaltenden [plannerTask](plannerTask.md)-Ressource aktualisiert werden.

Beispiel:

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": "String",
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->