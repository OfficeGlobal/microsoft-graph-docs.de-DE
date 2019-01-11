---
title: plannerProgressTaskBoardTaskFormat-Ressourcentyp
description: Die **plannerProgressTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Fortschritt“ des Task Board verwendet werden (eine Ansicht, die nach dem Status des Felds „ProzentAbgeschlossen“ für das Aufgabenobjekt sortiert ist und Spalten für „Nicht gestartet“, „In Bearbeitung“ und „Abgeschlossen“ enthält). Jeder Aufgabe ist ein **plannerProgressTaskBoardTaskFormat**-Objekt zugeordnet.
localization_priority: Normal
ms.openlocfilehash: 2f3395e0b63d038b8c280e54a76afcc2ca864789
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845584"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="41fbc-104">plannerProgressTaskBoardTaskFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="41fbc-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="41fbc-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="41fbc-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41fbc-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="41fbc-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41fbc-p103">Die **plannerProgressTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Fortschritt“ des Task Board verwendet werden (eine Ansicht, die nach dem Status des Felds „ProzentAbgeschlossen“ für das Aufgabenobjekt sortiert ist und Spalten für „Nicht gestartet“, „In Bearbeitung“ und „Abgeschlossen“ enthält). Jeder [Aufgabe](plannertask.md) ist ein **plannerProgressTaskBoardTaskFormat**-Objekt zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="41fbc-p103">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete). Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="41fbc-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="41fbc-109">Methods</span></span>

| <span data-ttu-id="41fbc-110">Methode</span><span class="sxs-lookup"><span data-stu-id="41fbc-110">Method</span></span>           | <span data-ttu-id="41fbc-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="41fbc-111">Return Type</span></span>    |<span data-ttu-id="41fbc-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41fbc-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="41fbc-113">plannerProgressTaskBoardTaskFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="41fbc-113">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="41fbc-114">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="41fbc-114">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="41fbc-115">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerProgressTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="41fbc-115">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="41fbc-116">Update</span><span class="sxs-lookup"><span data-stu-id="41fbc-116">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="41fbc-117">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="41fbc-117">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="41fbc-118">Dient zum Aktualisieren des **plannerProgressTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="41fbc-118">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="41fbc-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="41fbc-119">Properties</span></span>
| <span data-ttu-id="41fbc-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="41fbc-120">Property</span></span>     | <span data-ttu-id="41fbc-121">Typ</span><span class="sxs-lookup"><span data-stu-id="41fbc-121">Type</span></span>   |<span data-ttu-id="41fbc-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="41fbc-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41fbc-123">id</span><span class="sxs-lookup"><span data-stu-id="41fbc-123">id</span></span>|<span data-ttu-id="41fbc-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="41fbc-124">String</span></span>| <span data-ttu-id="41fbc-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="41fbc-125">Read-only.</span></span> <span data-ttu-id="41fbc-126">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="41fbc-126">ID of the resource.</span></span> <span data-ttu-id="41fbc-127">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="41fbc-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="41fbc-128">[Format Validierung](tasks-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="41fbc-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="41fbc-129">orderHint</span><span class="sxs-lookup"><span data-stu-id="41fbc-129">orderHint</span></span>|<span data-ttu-id="41fbc-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="41fbc-130">String</span></span>|<span data-ttu-id="41fbc-p105">Hinweiswert, der verwendet wird, um die Aufgaben in der Ansicht „Fortschritt“ des Task Board anzuordnen. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="41fbc-p105">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="41fbc-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="41fbc-133">Relationships</span></span>
<span data-ttu-id="41fbc-134">Keine</span><span class="sxs-lookup"><span data-stu-id="41fbc-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="41fbc-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="41fbc-135">JSON representation</span></span>
<span data-ttu-id="41fbc-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="41fbc-136">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
