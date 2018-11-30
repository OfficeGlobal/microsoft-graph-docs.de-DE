---
title: plannerAssignedToTaskBoardTaskFormat-Ressourcentyp
description: Die **plannerAssignedToTaskBoardTaskFormat** Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board verwendet werden (eine Ansicht, die nach Benutzern organisiert ist, denen Aufgaben zugewiesen sind). Jeder Aufgabe ist ein **plannerAssignedToTaskBoardTaskFormat**-Objekt zugeordnet.
ms.openlocfilehash: 35aaf5d93e4190fead1234131864e7fab11b96b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018577"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="e46c3-104">plannerAssignedToTaskBoardTaskFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e46c3-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="e46c3-p102">Die **plannerAssignedToTaskBoardTaskFormat** Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board verwendet werden (eine Ansicht, die nach Benutzern organisiert ist, denen Aufgaben zugewiesen sind). Jeder [Aufgabe](plannertask.md) ist ein **plannerAssignedToTaskBoardTaskFormat**-Objekt zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="e46c3-p102">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to). Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="e46c3-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="e46c3-107">Methods</span></span>

| <span data-ttu-id="e46c3-108">Methode</span><span class="sxs-lookup"><span data-stu-id="e46c3-108">Method</span></span>           | <span data-ttu-id="e46c3-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="e46c3-109">Return Type</span></span>    |<span data-ttu-id="e46c3-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e46c3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e46c3-111">plannerAssignedToTaskBoardTaskFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="e46c3-111">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="e46c3-112">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e46c3-112">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="e46c3-113">Dient zum Lesen der Eigenschaften und Beziehungen eines **PlannerAssignedToTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e46c3-113">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="e46c3-114">Update</span><span class="sxs-lookup"><span data-stu-id="e46c3-114">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="e46c3-115">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="e46c3-115">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="e46c3-116">Dient zum Aktualisieren eines **plannerAssignedToTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="e46c3-116">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e46c3-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e46c3-117">Properties</span></span>
| <span data-ttu-id="e46c3-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e46c3-118">Property</span></span>     | <span data-ttu-id="e46c3-119">Typ</span><span class="sxs-lookup"><span data-stu-id="e46c3-119">Type</span></span>   |<span data-ttu-id="e46c3-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e46c3-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e46c3-121">id</span><span class="sxs-lookup"><span data-stu-id="e46c3-121">id</span></span>|<span data-ttu-id="e46c3-122">String</span><span class="sxs-lookup"><span data-stu-id="e46c3-122">String</span></span>| <span data-ttu-id="e46c3-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e46c3-123">Read-only.</span></span> <span data-ttu-id="e46c3-124">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e46c3-124">ID of the resource.</span></span> <span data-ttu-id="e46c3-125">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="e46c3-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="e46c3-126">[Format Validierung](planner-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="e46c3-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="e46c3-127">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="e46c3-127">orderHintsByAssignee</span></span>|[<span data-ttu-id="e46c3-128">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="e46c3-128">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="e46c3-p104">Wörterbuch von Hinweisen, die verwendet werden, um Aufgaben in der Ansicht „ZugewiesenAn“ des Task Board anzuordnen. Der Schlüssel für jeden Eintrag ist einer der Benutzer, denen die Aufgabe zugewiesen ist, und der Wert ist der Anordnungshinweis. Das Format der einzelnen Werte ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="e46c3-p104">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="e46c3-132">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="e46c3-132">unassignedOrderHint</span></span>|<span data-ttu-id="e46c3-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e46c3-133">String</span></span>|<span data-ttu-id="e46c3-p105">Hinweiswert, der verwendet wird, um die Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board anzuordnen, wenn die Aufgabe keinem Benutzer zugewiesen ist oder wenn das orderHintsByAssignee-Wörterbuch keinen Anordnungshinweis für den Benutzer enthält, dem die Aufgabe zugewiesen ist. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="e46c3-p105">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="e46c3-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e46c3-136">Relationships</span></span>
<span data-ttu-id="e46c3-137">Keine</span><span class="sxs-lookup"><span data-stu-id="e46c3-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e46c3-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e46c3-138">JSON representation</span></span>
<span data-ttu-id="e46c3-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e46c3-139">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHintsByAssignee": {"@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"},
  "unassignedOrderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAssignedToTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->