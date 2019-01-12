---
title: plannerBucketTaskBoardTaskFormat-Ressourcentyp
description: Die **plannerBucketTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Buckets“ des Task Board verwendet werden (eine Ansicht, die nach den Aufgaben in den Buckets organisiert ist, denen sie zugewiesen sind). Jeder Aufgabe ist ein **plannerBucketTaskBoardTaskFormat**-Objekt zugeordnet.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: ea557bad20aa0fd10a73e71902b959913e8fff12
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986194"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="97071-104">plannerBucketTaskBoardTaskFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="97071-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

> <span data-ttu-id="97071-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="97071-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97071-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="97071-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97071-p103">Die **plannerBucketTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Buckets“ des Task Board verwendet werden (eine Ansicht, die nach den Aufgaben in den Buckets organisiert ist, denen sie zugewiesen sind). Jeder [Aufgabe](plannertask.md) ist ein **plannerBucketTaskBoardTaskFormat**-Objekt zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="97071-p103">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="97071-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="97071-109">Methods</span></span>

| <span data-ttu-id="97071-110">Methode</span><span class="sxs-lookup"><span data-stu-id="97071-110">Method</span></span>           | <span data-ttu-id="97071-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="97071-111">Return Type</span></span>    |<span data-ttu-id="97071-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97071-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="97071-113">plannerBucketTaskBoardTaskFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="97071-113">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="97071-114">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="97071-114">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="97071-115">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerBucketTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="97071-115">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="97071-116">Update</span><span class="sxs-lookup"><span data-stu-id="97071-116">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="97071-117">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="97071-117">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="97071-118">Dient zum Aktualisieren des **plannerBucketTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="97071-118">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="97071-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="97071-119">Properties</span></span>
| <span data-ttu-id="97071-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="97071-120">Property</span></span>     | <span data-ttu-id="97071-121">Typ</span><span class="sxs-lookup"><span data-stu-id="97071-121">Type</span></span>   |<span data-ttu-id="97071-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97071-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97071-123">id</span><span class="sxs-lookup"><span data-stu-id="97071-123">id</span></span>|<span data-ttu-id="97071-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97071-124">String</span></span>| <span data-ttu-id="97071-125">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="97071-125">Read-only.</span></span> <span data-ttu-id="97071-126">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="97071-126">ID of the resource.</span></span> <span data-ttu-id="97071-127">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="97071-127">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="97071-128">[Format Validierung](tasks-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="97071-128">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="97071-129">orderHint</span><span class="sxs-lookup"><span data-stu-id="97071-129">orderHint</span></span>|<span data-ttu-id="97071-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="97071-130">String</span></span>|<span data-ttu-id="97071-p105">Hinweis, der zum Anordnen von Aufgaben in der Ansicht „Buckets“ des Task Board verwendet wird. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="97071-p105">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="97071-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="97071-133">Relationships</span></span>
<span data-ttu-id="97071-134">Keine</span><span class="sxs-lookup"><span data-stu-id="97071-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="97071-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="97071-135">JSON representation</span></span>
<span data-ttu-id="97071-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="97071-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
