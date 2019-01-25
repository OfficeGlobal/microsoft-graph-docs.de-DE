---
title: plannerBucketTaskBoardTaskFormat-Ressourcentyp
description: Die **plannerBucketTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Buckets“ des Task Board verwendet werden (eine Ansicht, die nach den Aufgaben in den Buckets organisiert ist, denen sie zugewiesen sind). Jeder **Aufgabe** ist ein plannerBucketTaskBoardTaskFormat-Objekt zugeordnet.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: eca8865e54d68fb7b403364b065e642ad61e9276
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526949"
---
# <a name="plannerbuckettaskboardtaskformat-resource-type"></a><span data-ttu-id="bd289-104">plannerBucketTaskBoardTaskFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bd289-104">plannerBucketTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd289-p102">Die **plannerBucketTaskBoardTaskFormat**-Ressource stellt die Informationen dar, die zum korrekten Rendern einer Aufgabe in der Ansicht „Buckets“ des Task Board verwendet werden (eine Ansicht, die nach den Aufgaben in den Buckets organisiert ist, denen sie zugewiesen sind). Jeder [Aufgabe](plannertask.md) ist ein **plannerBucketTaskBoardTaskFormat**-Objekt zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="bd289-p102">The **plannerBucketTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Buckets view of the Task Board (a view organized by tasks within the buckets they are assigned to). Each [task](plannertask.md) will have one **plannerBucketTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="bd289-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="bd289-107">Methods</span></span>

| <span data-ttu-id="bd289-108">Methode</span><span class="sxs-lookup"><span data-stu-id="bd289-108">Method</span></span>           | <span data-ttu-id="bd289-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bd289-109">Return Type</span></span>    |<span data-ttu-id="bd289-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd289-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bd289-111">plannerBucketTaskBoardTaskFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="bd289-111">Get plannerBucketTaskBoardTaskFormat</span></span>](../api/plannerbuckettaskboardtaskformat-get.md) | [<span data-ttu-id="bd289-112">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="bd289-112">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md) |<span data-ttu-id="bd289-113">Dient zum Lesen der Eigenschaften und Beziehungen eines **plannerBucketTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bd289-113">Read properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="bd289-114">Update</span><span class="sxs-lookup"><span data-stu-id="bd289-114">Update</span></span>](../api/plannerbuckettaskboardtaskformat-update.md) | [<span data-ttu-id="bd289-115">plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="bd289-115">plannerBucketTaskBoardTaskFormat</span></span>](plannerbuckettaskboardtaskformat.md)  |<span data-ttu-id="bd289-116">Dient zum Aktualisieren des **plannerBucketTaskBoardTaskFormat**-Objekts.</span><span class="sxs-lookup"><span data-stu-id="bd289-116">Update **plannerBucketTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bd289-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bd289-117">Properties</span></span>
| <span data-ttu-id="bd289-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd289-118">Property</span></span>     | <span data-ttu-id="bd289-119">Typ</span><span class="sxs-lookup"><span data-stu-id="bd289-119">Type</span></span>   |<span data-ttu-id="bd289-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd289-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd289-121">id</span><span class="sxs-lookup"><span data-stu-id="bd289-121">id</span></span>|<span data-ttu-id="bd289-122">String</span><span class="sxs-lookup"><span data-stu-id="bd289-122">String</span></span>| <span data-ttu-id="bd289-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="bd289-123">Read-only.</span></span> <span data-ttu-id="bd289-124">Die ID der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bd289-124">ID of the resource.</span></span> <span data-ttu-id="bd289-125">Es ist eine 28 Zeichen lang und Groß-/Kleinschreibung beachtet.</span><span class="sxs-lookup"><span data-stu-id="bd289-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="bd289-126">[Format Validierung](tasks-identifiers-disclaimer.md) erfolgt für den Dienst.</span><span class="sxs-lookup"><span data-stu-id="bd289-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="bd289-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="bd289-127">orderHint</span></span>|<span data-ttu-id="bd289-128">String</span><span class="sxs-lookup"><span data-stu-id="bd289-128">String</span></span>|<span data-ttu-id="bd289-p104">Hinweis, der zum Anordnen von Aufgaben in der Ansicht „Buckets“ des Task Board verwendet wird. Das Format ist wie [hier](planner-order-hint-format.md) beschrieben definiert.</span><span class="sxs-lookup"><span data-stu-id="bd289-p104">Hint used to order tasks in the Bucket view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd289-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bd289-131">Relationships</span></span>
<span data-ttu-id="bd289-132">Keine</span><span class="sxs-lookup"><span data-stu-id="bd289-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bd289-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bd289-133">JSON representation</span></span>
<span data-ttu-id="bd289-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bd289-134">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerbuckettaskboardtaskformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
