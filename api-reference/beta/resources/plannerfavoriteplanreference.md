---
title: Ressourcentyp plannerFavoritePlanReference
description: 'Die Ressource **PlannerFavoritePlanReference** Repesents Geben Sie einen Verweis auf eine PlannerPlan, die markiert wurde als Favoriten des Benutzers. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 77a931a882cc4b01725bd8ceb0ae6bcc721a9013
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518387"
---
# <a name="plannerfavoriteplanreference-resource-type"></a><span data-ttu-id="cb0f8-103">Ressourcentyp plannerFavoritePlanReference</span><span class="sxs-lookup"><span data-stu-id="cb0f8-103">plannerFavoritePlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb0f8-104">Die Ressource **PlannerFavoritePlanReference** Repesents Geben Sie einen Verweis auf eine [PlannerPlan](plannerplan.md) , die markiert wurde als Favoriten des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="cb0f8-104">The **plannerFavoritePlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has been marked as a favorite by the user.</span></span> <span data-ttu-id="cb0f8-105">Clients Beachten Sie, dass Einträge **PlannerFavoritePlanReference** **PlannerPlans** , die gelöscht werden, die der Benutzer zugreifen kann nicht mehr oder die mit einem anderen Titel aktualisiert wurden, verweisen können.</span><span class="sxs-lookup"><span data-stu-id="cb0f8-105">Clients should note that **plannerFavoritePlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>

<span data-ttu-id="cb0f8-106">Es wird empfohlen, dass Clients benachrichtigen Sie Benutzer bei Diskrepanzen und die Einträge auf dem aktuellen Stand halten.</span><span class="sxs-lookup"><span data-stu-id="cb0f8-106">We recommend that clients notify users when there are discrepancies and keep the entries up to date.</span></span>


## <a name="properties"></a><span data-ttu-id="cb0f8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cb0f8-107">Properties</span></span>
| <span data-ttu-id="cb0f8-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cb0f8-108">Property</span></span>     | <span data-ttu-id="cb0f8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="cb0f8-109">Type</span></span>   |<span data-ttu-id="cb0f8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb0f8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb0f8-111">orderHint</span><span class="sxs-lookup"><span data-stu-id="cb0f8-111">orderHint</span></span>|<span data-ttu-id="cb0f8-112">String</span><span class="sxs-lookup"><span data-stu-id="cb0f8-112">String</span></span>|<span data-ttu-id="cb0f8-p102">Hinweis, der zum Anordnen von Elementen dieses Typs in einer Listenansicht verwendet wird. Das Format ist unter [Verwenden von Anordnungshinweisen in Planner](planner-order-hint-format.md) definiert.</span><span class="sxs-lookup"><span data-stu-id="cb0f8-p102">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="cb0f8-115">planTitle</span><span class="sxs-lookup"><span data-stu-id="cb0f8-115">planTitle</span></span>|<span data-ttu-id="cb0f8-116">String</span><span class="sxs-lookup"><span data-stu-id="cb0f8-116">String</span></span>|<span data-ttu-id="cb0f8-117">Titel des Plans zur Zeit, dass der Benutzer als Favoriten markiert.</span><span class="sxs-lookup"><span data-stu-id="cb0f8-117">Title of the plan at the time the user marked it as a favorite.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="cb0f8-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cb0f8-118">JSON representation</span></span>

<span data-ttu-id="cb0f8-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cb0f8-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReference"
}-->

```json
{
  "orderHint": "String",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerfavoriteplanreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
