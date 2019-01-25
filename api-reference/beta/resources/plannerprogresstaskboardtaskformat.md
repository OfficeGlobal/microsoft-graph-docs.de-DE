---
title: plannerProgressTaskBoardTaskFormat-Ressourcentyp
description: Die **plannerProgressTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Fortschritt“ des Task Board verwendet werden (eine Ansicht, die nach dem Status des Felds „ProzentAbgeschlossen“ für das Aufgabenobjekt sortiert ist und Spalten für „Nicht gestartet“, „In Bearbeitung“ und „Abgeschlossen“ enthält). Jeder **Aufgabe** ist ein plannerProgressTaskBoardTaskFormat-Objekt zugeordnet.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 20a215b108ca1f1801702a532bda09eac67834c6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522070"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="5fbfe-104">plannerProgressTaskBoardTaskFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5fbfe-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fbfe-p102">Die **plannerProgressTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Fortschritt“ des Task Board verwendet werden (eine Ansicht, die nach dem Status des Felds „ProzentAbgeschlossen“ für das Aufgabenobjekt sortiert ist und Spalten für „Nicht gestartet“, „In Bearbeitung“ und „Abgeschlossen“ enthält). Jeder [Aufgabe](plannertask.md) ist ein **plannerProgressTaskBoardTaskFormat**-Objekt zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="5fbfe-p102">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete). Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="5fbfe-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="5fbfe-107">Methods</span></span>

| <span data-ttu-id="5fbfe-108">Methode</span><span class="sxs-lookup"><span data-stu-id="5fbfe-108">Method</span></span>           | <span data-ttu-id="5fbfe-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="5fbfe-109">Return Type</span></span>    |<span data-ttu-id="5fbfe-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5fbfe-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5fbfe-111">plannerProgressTaskBoardTaskFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="5fbfe-111">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="5fbfe-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="5fbfe-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="5fbfe-113">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerProgressTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5fbfe-113">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="5fbfe-114">Update</span><span class="sxs-lookup"><span data-stu-id="5fbfe-114">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="5fbfe-115">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="5fbfe-115">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="5fbfe-116">Dient zum Aktualisieren des **plannerProgressTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="5fbfe-116">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5fbfe-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5fbfe-117">Properties</span></span>
| <span data-ttu-id="5fbfe-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5fbfe-118">Property</span></span>     | <span data-ttu-id="5fbfe-119">Typ</span><span class="sxs-lookup"><span data-stu-id="5fbfe-119">Type</span></span>   |<span data-ttu-id="5fbfe-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5fbfe-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5fbfe-121">id</span><span class="sxs-lookup"><span data-stu-id="5fbfe-121">id</span></span>|<span data-ttu-id="5fbfe-122">String</span><span class="sxs-lookup"><span data-stu-id="5fbfe-122">String</span></span>| <span data-ttu-id="5fbfe-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="5fbfe-123">Read-only.</span></span> <span data-ttu-id="5fbfe-124">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5fbfe-124">ID of the resource.</span></span> <span data-ttu-id="5fbfe-125">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="5fbfe-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="5fbfe-126">[Format Validierung](tasks-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="5fbfe-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="5fbfe-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="5fbfe-127">orderHint</span></span>|<span data-ttu-id="5fbfe-128">String</span><span class="sxs-lookup"><span data-stu-id="5fbfe-128">String</span></span>|<span data-ttu-id="5fbfe-p104">Hinweiswert, der verwendet wird, um die Aufgaben in der Ansicht „Fortschritt“ des Task Board anzuordnen. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="5fbfe-p104">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="5fbfe-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5fbfe-131">Relationships</span></span>
<span data-ttu-id="5fbfe-132">Keine</span><span class="sxs-lookup"><span data-stu-id="5fbfe-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5fbfe-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5fbfe-133">JSON representation</span></span>
<span data-ttu-id="5fbfe-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5fbfe-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerprogresstaskboardtaskformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
