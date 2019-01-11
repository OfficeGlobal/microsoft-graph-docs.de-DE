---
title: Ressourcentyp plannerFavoritePlanReference
description: 'Die Ressource **PlannerFavoritePlanReference** Repesents Geben Sie einen Verweis auf eine PlannerPlan, die markiert wurde als Favoriten des Benutzers. '
localization_priority: Normal
ms.openlocfilehash: b17846eaa1b9a9859d23735d18a191cae4872542
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871323"
---
# <a name="plannerfavoriteplanreference-resource-type"></a><span data-ttu-id="13e68-103">Ressourcentyp plannerFavoritePlanReference</span><span class="sxs-lookup"><span data-stu-id="13e68-103">plannerFavoritePlanReference resource type</span></span>

> <span data-ttu-id="13e68-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="13e68-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13e68-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="13e68-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13e68-106">Die Ressource **PlannerFavoritePlanReference** Repesents Geben Sie einen Verweis auf eine [PlannerPlan](plannerplan.md) , die markiert wurde als Favoriten des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="13e68-106">The **plannerFavoritePlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has been marked as a favorite by the user.</span></span> <span data-ttu-id="13e68-107">Clients Beachten Sie, dass Einträge **PlannerFavoritePlanReference** **PlannerPlans** , die gelöscht werden, die der Benutzer zugreifen kann nicht mehr oder die mit einem anderen Titel aktualisiert wurden, verweisen können.</span><span class="sxs-lookup"><span data-stu-id="13e68-107">Clients should note that **plannerFavoritePlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>

<span data-ttu-id="13e68-108">Es wird empfohlen, dass Clients benachrichtigen Sie Benutzer bei Diskrepanzen und die Einträge auf dem aktuellen Stand halten.</span><span class="sxs-lookup"><span data-stu-id="13e68-108">We recommend that clients notify users when there are discrepancies and keep the entries up to date.</span></span>


## <a name="properties"></a><span data-ttu-id="13e68-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="13e68-109">Properties</span></span>
| <span data-ttu-id="13e68-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13e68-110">Property</span></span>     | <span data-ttu-id="13e68-111">Typ</span><span class="sxs-lookup"><span data-stu-id="13e68-111">Type</span></span>   |<span data-ttu-id="13e68-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13e68-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13e68-113">orderHint</span><span class="sxs-lookup"><span data-stu-id="13e68-113">orderHint</span></span>|<span data-ttu-id="13e68-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13e68-114">String</span></span>|<span data-ttu-id="13e68-p103">Hinweis, der zum Anordnen von Elementen dieses Typs in einer Listenansicht verwendet wird. Das Format ist unter [Verwenden von Anordnungshinweisen in Planner](planner-order-hint-format.md) definiert.</span><span class="sxs-lookup"><span data-stu-id="13e68-p103">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="13e68-117">planTitle</span><span class="sxs-lookup"><span data-stu-id="13e68-117">planTitle</span></span>|<span data-ttu-id="13e68-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13e68-118">String</span></span>|<span data-ttu-id="13e68-119">Titel des Plans zur Zeit, dass der Benutzer als Favoriten markiert.</span><span class="sxs-lookup"><span data-stu-id="13e68-119">Title of the plan at the time the user marked it as a favorite.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="13e68-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="13e68-120">JSON representation</span></span>

<span data-ttu-id="13e68-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="13e68-121">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
