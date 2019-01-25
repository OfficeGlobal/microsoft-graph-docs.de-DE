---
title: Ressourcentyp plannerRecentPlanReference
description: 'Die Ressource **PlannerRecentPlanReference** Repesents Geben Sie einen Verweis auf eine PlannerPlan, die kürzlich von einem Benutzer angezeigt wurde. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 55ccf34055d7d181dbbeecd5b6c30a3843f211d5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509161"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="53a36-103">Ressourcentyp plannerRecentPlanReference</span><span class="sxs-lookup"><span data-stu-id="53a36-103">plannerRecentPlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53a36-104">Die Ressource **PlannerRecentPlanReference** Repesents Geben Sie einen Verweis auf eine [PlannerPlan](plannerplan.md) , die kürzlich von einem Benutzer angezeigt wurde.</span><span class="sxs-lookup"><span data-stu-id="53a36-104">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="53a36-105">Die **PlannerRecentPlanReferences** für einen Benutzer werden explizit verwaltet von apps.</span><span class="sxs-lookup"><span data-stu-id="53a36-105">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="53a36-106">Alle Apps, die das letzte Pläne Feature implementiert sollte zu notieren, wenn der Benutzer zuletzt einen Plan und Update **PlannerRecentPlanReference** Einträge entsprechend angezeigt.</span><span class="sxs-lookup"><span data-stu-id="53a36-106">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="53a36-107">Apps Beachten Sie, dass Einträge **PlannerRecentPlanReference** **PlannerPlans** , die gelöscht werden, die der Benutzer zugreifen kann nicht mehr oder die mit einem anderen Titel aktualisiert wurden, verweisen können.</span><span class="sxs-lookup"><span data-stu-id="53a36-107">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="53a36-108">Es wird empfohlen, dass apps benachrichtigen Sie Benutzer bei Diskrepanzen und die Einträge auf dem aktuellen Stand halten.</span><span class="sxs-lookup"><span data-stu-id="53a36-108">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="53a36-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="53a36-109">Properties</span></span>
| <span data-ttu-id="53a36-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="53a36-110">Property</span></span>     | <span data-ttu-id="53a36-111">Typ</span><span class="sxs-lookup"><span data-stu-id="53a36-111">Type</span></span>   |<span data-ttu-id="53a36-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="53a36-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53a36-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="53a36-113">lastAccessedDateTime</span></span>|<span data-ttu-id="53a36-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53a36-114">DateTimeOffset</span></span>|<span data-ttu-id="53a36-115">Das Datum und die Zeit, die vom Benutzer zuletzt des Plans angezeigt wurde.</span><span class="sxs-lookup"><span data-stu-id="53a36-115">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="53a36-116">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="53a36-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="53a36-117">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="53a36-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="53a36-118">planTitle</span><span class="sxs-lookup"><span data-stu-id="53a36-118">planTitle</span></span>|<span data-ttu-id="53a36-119">String</span><span class="sxs-lookup"><span data-stu-id="53a36-119">String</span></span>|<span data-ttu-id="53a36-120">Der Titel des Plans zum Zeitpunkt der Benutzer es angezeigt.</span><span class="sxs-lookup"><span data-stu-id="53a36-120">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53a36-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="53a36-121">JSON representation</span></span>

<span data-ttu-id="53a36-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="53a36-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerRecentPlanReference"
}-->

```json
{
  "lastAccessedDateTime": "String (timestamp)",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerrecentplanreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
