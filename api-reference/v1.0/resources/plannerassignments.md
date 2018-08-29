# <a name="plannerassignments-resource-type"></a><span data-ttu-id="f4876-101">plannerAssignments-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f4876-101">plannerAssignments resource type</span></span>

<span data-ttu-id="f4876-p101">Die **plannerAssignments**-Ressource stellt Zuweisungen einer [plannerTask](plannertask.md)-Ressource dar. Es handelt sich um einen offenen Typ. Jeder Eigenschaftenname in diesem Typ ist die ID eines Benutzerobjekts, dem eine Aufgabe zugewiesen ist. Die Benutzer können Aufgaben zugewiesen werden, indem neue Eigenschaften mit dem Namen ihrer ID erstellt werden, wobei ein [plannerAssignment](plannerassignment.md)-Objekt mit der orderHint-Eigenschaft als Wert gefüllt wird. Die Zuweisung der zugewiesenen Personen zur Aufgabe kann aufgehoben werden, indem die Eigenschaft mit dem Namen ihrer ID auf „null“ festgelegt wird.</span><span class="sxs-lookup"><span data-stu-id="f4876-p101">The **plannerAssignments** resource represents assignments of a [plannerTask](plannertask.md) resource. This type is an open type. Each property name in this type is the ID of a user object a task is assigned to. The users can be assigned to tasks with creating new properties named with their ID, with a [plannerassignment](plannerassignment.md) object with orderHint property populated as the value. The assignees can be unassigned from the task by setting the propety named with their ID to null.</span></span>


## <a name="properties"></a><span data-ttu-id="f4876-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f4876-107">Properties</span></span>
<span data-ttu-id="f4876-p102">Eigenschaften mit offenem Typ können vom Client definiert werden. In diesem Fall muss der Client jedoch die IDs von zugewiesenen Benutzern als Eigenschaftennamen angeben. Die Eigenschaft muss auf ein **plannerAssignment**-Objekt festgelegt werden, um zugewiesene Personen zu erstellen oder zu ändern, und auf „null“, um sie zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="f4876-p102">Properties of an Open Type can be defined by the client. In this case though, the client must provide assigned user's IDs as property names. The property must be set to a **plannerAssignment** object to create or modify assignees, and to null to remove them.</span></span>

<span data-ttu-id="f4876-111">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="f4876-111">Example:</span></span>

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47", "4e98f8f1-bb03-4015-b8e0-19bb370949d8" ],
  "@odata.type": "microsoft.graph.plannerAssignments"
}-->
```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": null,
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": { 
      "@odata.type": "microsoft.graph.plannerAssignment",
      "orderHint": "String"
    }
}
```
<span data-ttu-id="f4876-p103">In diesem Beispiel wird der Benutzer mit der ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 aus der Liste der der Aufgabe zugewiesenen Personen entfernt; gleichzeitig wird die Anordnung der zugewiesenen Person mit der Benutzer-ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8 geändert. Wenn die Aufgabe nicht bereits dem Benutzer mit der ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8 zugewiesen ist, wird die Aufgabe durch Aktualisieren der Zuweisungen mit diesem Wert diesem Benutzer zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="f4876-p103">This example removes user with ID ca2a1df2-e36b-4987-9f6b-0ea462f4eb47 from the assignees list of the task, while changing the order of the assignee with user ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8. If the task isn't already assigned to user with ID 4e98f8f1-bb03-4015-b8e0-19bb370949d8, updating the assignments with this value will assign the task to this user.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignments resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->