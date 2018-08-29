# <a name="plannerorderhintsbyassignee-resource-type"></a><span data-ttu-id="5c511-101">plannerOrderHintsByAssignee-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5c511-101">plannerOrderHintsByAssignee resource type</span></span>

<span data-ttu-id="5c511-p101">Die **plannerOrderHintsByAssignee**-Ressource enthält [Anordnungshinweise](planner_order_hint_format.md) für zugewiesene Personen in einer [plannerTask](plannerTask.md)-Ressource, um die Anordnung der Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board anzugeben. Es handelt sich um einen offenen Typ. Die Eigenschaften sind die IDs der Benutzer, die der Aufgabe zugewiesen sind, und die Werte sind Anordnungshinweise.</span><span class="sxs-lookup"><span data-stu-id="5c511-p101">The **plannerOrderHintsByAssignee** is a resource that contains [ordering hints](planner_order_hint_format.md) for assignees in a [plannerTask](plannerTask.md) resource, to indicate the order of the task in Assigned To view of the Task Board. This type is an open type. The properties are the ids of users assigned to the task, and the values are order hints.</span></span>

## <a name="properties"></a><span data-ttu-id="5c511-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5c511-105">Properties</span></span>
<span data-ttu-id="5c511-p102">Eigenschaften mit offenem Typ können vom Client definiert werden. In diesem Fall muss der Client IDs von Benutzern, die der Aufgabe zugewiesen sind, als Eigenschaftennamen und einen gültigen [Anordnungshinweis](planner_order_hint_format.md) als Wert angeben. Von diesem Typ können keine Eigenschaften entfernt werden. Der Dienst entfernt automatisch Werte, wenn die Zuweisungen in der enthaltenden [plannerTask](plannerTask.md)-Ressource aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="5c511-p102">Properties of an Open Type can be defined by the client. In this case, the client must provide ids of users assigned to the task as property names, and a valid [order hint](planner_order_hint_format.md) as the value. Properties cannot be removed from this type. The service will automatically remove values as the assignments on the containing [plannerTask](plannerTask.md) are updated.</span></span>

<span data-ttu-id="5c511-110">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="5c511-110">Example:</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47", "4e98f8f1-bb03-4015-b8e0-19bb370949d8" ],
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