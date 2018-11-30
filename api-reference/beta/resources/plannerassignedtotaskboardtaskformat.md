---
title: plannerAssignedToTaskBoardTaskFormat-Ressourcentyp
description: Die **plannerAssignedToTaskBoardTaskFormat** Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board verwendet werden (eine Ansicht, die nach Benutzern organisiert ist, denen Aufgaben zugewiesen sind). Jeder Aufgabe ist ein **plannerAssignedToTaskBoardTaskFormat**-Objekt zugeordnet.
ms.openlocfilehash: 8fc96d6fa7d4f05f6bc81f7030ebe766bf769e40
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062290"
---
# <a name="plannerassignedtotaskboardtaskformat-resource-type"></a><span data-ttu-id="7efdd-104">plannerAssignedToTaskBoardTaskFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7efdd-104">plannerAssignedToTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="7efdd-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7efdd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7efdd-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7efdd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7efdd-p103">Die **plannerAssignedToTaskBoardTaskFormat** Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board verwendet werden (eine Ansicht, die nach Benutzern organisiert ist, denen Aufgaben zugewiesen sind). Jeder [Aufgabe](plannertask.md) ist ein **plannerAssignedToTaskBoardTaskFormat**-Objekt zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="7efdd-p103">The **plannerAssignedToTaskBoardTaskFormat** resource represents the information used to render a task correctly in the AssignedTo view of the Task Board (a view organized by users to whom tasks are assigned to). Each [task](plannertask.md) will have one **plannerAssignedToTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="7efdd-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="7efdd-109">Methods</span></span>

| <span data-ttu-id="7efdd-110">Methode</span><span class="sxs-lookup"><span data-stu-id="7efdd-110">Method</span></span>           | <span data-ttu-id="7efdd-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="7efdd-111">Return Type</span></span>    |<span data-ttu-id="7efdd-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7efdd-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7efdd-113">plannerAssignedToTaskBoardTaskFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="7efdd-113">Get plannerAssignedToTaskBoardTaskFormat</span></span>](../api/plannerassignedtotaskboardtaskformat-get.md) | [<span data-ttu-id="7efdd-114">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="7efdd-114">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md) |<span data-ttu-id="7efdd-115">Dient zum Lesen der Eigenschaften und Beziehungen eines **PlannerAssignedToTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7efdd-115">Read properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="7efdd-116">Update</span><span class="sxs-lookup"><span data-stu-id="7efdd-116">Update</span></span>](../api/plannerassignedtotaskboardtaskformat-update.md) | [<span data-ttu-id="7efdd-117">plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="7efdd-117">plannerAssignedToTaskBoardTaskFormat</span></span>](plannerassignedtotaskboardtaskformat.md)  |<span data-ttu-id="7efdd-118">Dient zum Aktualisieren eines **plannerAssignedToTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="7efdd-118">Update **plannerAssignedToTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7efdd-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7efdd-119">Properties</span></span>
| <span data-ttu-id="7efdd-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7efdd-120">Property</span></span>     | <span data-ttu-id="7efdd-121">Typ</span><span class="sxs-lookup"><span data-stu-id="7efdd-121">Type</span></span>   |<span data-ttu-id="7efdd-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7efdd-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7efdd-123">id</span><span class="sxs-lookup"><span data-stu-id="7efdd-123">id</span></span>|<span data-ttu-id="7efdd-124">String</span><span class="sxs-lookup"><span data-stu-id="7efdd-124">String</span></span>| <span data-ttu-id="7efdd-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7efdd-125">Read-only.</span></span> <span data-ttu-id="7efdd-126">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7efdd-126">ID of the resource.</span></span> <span data-ttu-id="7efdd-127">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="7efdd-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="7efdd-128">[Format Validierung](tasks-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="7efdd-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="7efdd-129">orderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="7efdd-129">orderHintsByAssignee</span></span>|[<span data-ttu-id="7efdd-130">plannerOrderHintsByAssignee</span><span class="sxs-lookup"><span data-stu-id="7efdd-130">plannerOrderHintsByAssignee</span></span>](plannerorderhintsbyassignee.md)|<span data-ttu-id="7efdd-p105">Wörterbuch von Hinweisen, die verwendet werden, um Aufgaben in der Ansicht „ZugewiesenAn“ des Task Board anzuordnen. Der Schlüssel für jeden Eintrag ist einer der Benutzer, denen die Aufgabe zugewiesen ist, und der Wert ist der Anordnungshinweis. Das Format der einzelnen Werte ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="7efdd-p105">Dictionary of hints used to order tasks on the AssignedTo view of the Task Board. The key of each entry is one of the users the task is assigned to and the value is the order hint. The format of each value is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="7efdd-134">unassignedOrderHint</span><span class="sxs-lookup"><span data-stu-id="7efdd-134">unassignedOrderHint</span></span>|<span data-ttu-id="7efdd-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7efdd-135">String</span></span>|<span data-ttu-id="7efdd-p106">Hinweiswert, der verwendet wird, um die Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board anzuordnen, wenn die Aufgabe keinem Benutzer zugewiesen ist oder wenn das orderHintsByAssignee-Wörterbuch keinen Anordnungshinweis für den Benutzer enthält, dem die Aufgabe zugewiesen ist. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="7efdd-p106">Hint value used to order the task on the AssignedTo view of the Task Board when the task is not assigned to anyone, or if the orderHintsByAssignee dictionary does not provide an order hint for the user the task is assigned to. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="7efdd-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7efdd-138">Relationships</span></span>
<span data-ttu-id="7efdd-139">Keine</span><span class="sxs-lookup"><span data-stu-id="7efdd-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7efdd-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7efdd-140">JSON representation</span></span>
<span data-ttu-id="7efdd-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7efdd-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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