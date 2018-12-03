---
title: plannerBucketTaskBoardTaskFormat-Ressourcentyp
description: Die **plannerBucketTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Buckets“ des Task Board verwendet werden (eine Ansicht, die nach den Aufgaben in den Buckets organisiert ist, denen sie zugewiesen sind). Jeder Aufgabe ist ein **plannerBucketTaskBoardTaskFormat**-Objekt zugeordnet.
ms.openlocfilehash: 7fb15bf59b2c7ffc0a515baff7b3f0dda8be179f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016418"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="61d3f-104">plannerBucketTaskBoardTaskFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="61d3f-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="61d3f-p102">Die **plannerBucketTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Buckets“ des Task Board verwendet werden (eine Ansicht, die nach den Aufgaben in den Buckets organisiert ist, denen sie zugewiesen sind). Jeder [Aufgabe](plannertask.md) ist ein **plannerBucketTaskBoardTaskFormat**-Objekt zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="61d3f-p102">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="61d3f-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="61d3f-107">Methods</span></span>

| <span data-ttu-id="61d3f-108">Methode</span><span class="sxs-lookup"><span data-stu-id="61d3f-108">Method</span></span>           | <span data-ttu-id="61d3f-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="61d3f-109">Return Type</span></span>    |<span data-ttu-id="61d3f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61d3f-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="61d3f-111">plannerBucketTaskBoardTaskFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="61d3f-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="61d3f-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="61d3f-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="61d3f-113">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerBucketTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="61d3f-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="61d3f-114">Update</span><span class="sxs-lookup"><span data-stu-id="61d3f-114">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="61d3f-115">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="61d3f-115">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="61d3f-116">Dient zum Aktualisieren des **plannerBucketTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="61d3f-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="61d3f-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="61d3f-117">Properties</span></span>
| <span data-ttu-id="61d3f-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61d3f-118">Property</span></span>     | <span data-ttu-id="61d3f-119">Typ</span><span class="sxs-lookup"><span data-stu-id="61d3f-119">Type</span></span>   |<span data-ttu-id="61d3f-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61d3f-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61d3f-121">id</span><span class="sxs-lookup"><span data-stu-id="61d3f-121">id</span></span>|<span data-ttu-id="61d3f-122">String</span><span class="sxs-lookup"><span data-stu-id="61d3f-122">String</span></span>| <span data-ttu-id="61d3f-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="61d3f-123">Read-only.</span></span> <span data-ttu-id="61d3f-124">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="61d3f-124">ID of the resource.</span></span> <span data-ttu-id="61d3f-125">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="61d3f-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="61d3f-126">[Format Validierung](planner-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="61d3f-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="61d3f-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="61d3f-127">orderHint</span></span>|<span data-ttu-id="61d3f-128">String</span><span class="sxs-lookup"><span data-stu-id="61d3f-128">String</span></span>|<span data-ttu-id="61d3f-p104">Hinweis, der zum Anordnen von Aufgaben in der Ansicht „Buckets“ des Task Board verwendet wird. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="61d3f-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="61d3f-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="61d3f-131">Relationships</span></span>
<span data-ttu-id="61d3f-132">Keine</span><span class="sxs-lookup"><span data-stu-id="61d3f-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="61d3f-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="61d3f-133">JSON representation</span></span>
<span data-ttu-id="61d3f-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="61d3f-134">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
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
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->