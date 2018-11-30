---
title: plannerProgressTaskBoardTaskFormat-Ressourcentyp
description: Die **plannerProgressTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Fortschritt“ des Task Board verwendet werden (eine Ansicht, die nach dem Status des Felds „ProzentAbgeschlossen“ für das Aufgabenobjekt sortiert ist und Spalten für „Nicht gestartet“, „In Bearbeitung“ und „Abgeschlossen“ enthält). Jeder Aufgabe ist ein **plannerProgressTaskBoardTaskFormat**-Objekt zugeordnet.
ms.openlocfilehash: 90ac4daa3d6b37f054c00df042de48d4c7706a96
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019505"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="42d2c-104">plannerProgressTaskBoardTaskFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="42d2c-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="42d2c-p102">Die **plannerProgressTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Fortschritt“ des Task Board verwendet werden (eine Ansicht, die nach dem Status des Felds „ProzentAbgeschlossen“ für das Aufgabenobjekt sortiert ist und Spalten für „Nicht gestartet“, „In Bearbeitung“ und „Abgeschlossen“ enthält). Jeder [Aufgabe](plannertask.md) ist ein **plannerProgressTaskBoardTaskFormat**-Objekt zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="42d2c-p102">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete). Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="42d2c-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="42d2c-107">Methods</span></span>

| <span data-ttu-id="42d2c-108">Methode</span><span class="sxs-lookup"><span data-stu-id="42d2c-108">Method</span></span>           | <span data-ttu-id="42d2c-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="42d2c-109">Return Type</span></span>    |<span data-ttu-id="42d2c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42d2c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="42d2c-111">plannerProgressTaskBoardTaskFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="42d2c-111">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="42d2c-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="42d2c-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="42d2c-113">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerProgressTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="42d2c-113">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="42d2c-114">Update</span><span class="sxs-lookup"><span data-stu-id="42d2c-114">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="42d2c-115">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="42d2c-115">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="42d2c-116">Dient zum Aktualisieren des **plannerProgressTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="42d2c-116">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="42d2c-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="42d2c-117">Properties</span></span>
| <span data-ttu-id="42d2c-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="42d2c-118">Property</span></span>     | <span data-ttu-id="42d2c-119">Typ</span><span class="sxs-lookup"><span data-stu-id="42d2c-119">Type</span></span>   |<span data-ttu-id="42d2c-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42d2c-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42d2c-121">id</span><span class="sxs-lookup"><span data-stu-id="42d2c-121">id</span></span>|<span data-ttu-id="42d2c-122">String</span><span class="sxs-lookup"><span data-stu-id="42d2c-122">String</span></span>| <span data-ttu-id="42d2c-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="42d2c-123">Read-only.</span></span> <span data-ttu-id="42d2c-124">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="42d2c-124">ID of the resource.</span></span> <span data-ttu-id="42d2c-125">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="42d2c-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="42d2c-126">[Format Validierung](planner-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="42d2c-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="42d2c-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="42d2c-127">orderHint</span></span>|<span data-ttu-id="42d2c-128">String</span><span class="sxs-lookup"><span data-stu-id="42d2c-128">String</span></span>|<span data-ttu-id="42d2c-p104">Hinweiswert, der verwendet wird, um die Aufgaben in der Ansicht „Fortschritt“ des Task Board anzuordnen. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="42d2c-p104">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="42d2c-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="42d2c-131">Relationships</span></span>
<span data-ttu-id="42d2c-132">Keine</span><span class="sxs-lookup"><span data-stu-id="42d2c-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="42d2c-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="42d2c-133">JSON representation</span></span>
<span data-ttu-id="42d2c-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="42d2c-134">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->