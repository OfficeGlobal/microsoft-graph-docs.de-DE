---
title: Ressourcentyp plannerRecentPlanReference
description: 'Die Ressource **PlannerRecentPlanReference** Repesents Geben Sie einen Verweis auf eine PlannerPlan, die kürzlich von einem Benutzer angezeigt wurde. '
ms.openlocfilehash: ac774ffbf7ebdfe45211cf50c2ce065921de30f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058864"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="e72b6-103">Ressourcentyp plannerRecentPlanReference</span><span class="sxs-lookup"><span data-stu-id="e72b6-103">plannerRecentPlanReference resource type</span></span>

> <span data-ttu-id="e72b6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e72b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e72b6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e72b6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e72b6-106">Die Ressource **PlannerRecentPlanReference** Repesents Geben Sie einen Verweis auf eine [PlannerPlan](plannerplan.md) , die kürzlich von einem Benutzer angezeigt wurde.</span><span class="sxs-lookup"><span data-stu-id="e72b6-106">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="e72b6-107">Die **PlannerRecentPlanReferences** für einen Benutzer werden explizit verwaltet von apps.</span><span class="sxs-lookup"><span data-stu-id="e72b6-107">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="e72b6-108">Alle Apps, die das letzte Pläne Feature implementiert sollte zu notieren, wenn der Benutzer zuletzt einen Plan und Update **PlannerRecentPlanReference** Einträge entsprechend angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e72b6-108">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="e72b6-109">Apps Beachten Sie, dass Einträge **PlannerRecentPlanReference** **PlannerPlans** , die gelöscht werden, die der Benutzer zugreifen kann nicht mehr oder die mit einem anderen Titel aktualisiert wurden, verweisen können.</span><span class="sxs-lookup"><span data-stu-id="e72b6-109">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="e72b6-110">Es wird empfohlen, dass apps benachrichtigen Sie Benutzer bei Diskrepanzen und die Einträge auf dem aktuellen Stand halten.</span><span class="sxs-lookup"><span data-stu-id="e72b6-110">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="e72b6-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e72b6-111">Properties</span></span>
| <span data-ttu-id="e72b6-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e72b6-112">Property</span></span>     | <span data-ttu-id="e72b6-113">Typ</span><span class="sxs-lookup"><span data-stu-id="e72b6-113">Type</span></span>   |<span data-ttu-id="e72b6-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e72b6-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e72b6-115">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="e72b6-115">lastAccessedDateTime</span></span>|<span data-ttu-id="e72b6-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e72b6-116">DateTimeOffset</span></span>|<span data-ttu-id="e72b6-117">Das Datum und die Zeit, die vom Benutzer zuletzt des Plans angezeigt wurde.</span><span class="sxs-lookup"><span data-stu-id="e72b6-117">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="e72b6-118">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="e72b6-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e72b6-119">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e72b6-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e72b6-120">planTitle</span><span class="sxs-lookup"><span data-stu-id="e72b6-120">planTitle</span></span>|<span data-ttu-id="e72b6-121">String</span><span class="sxs-lookup"><span data-stu-id="e72b6-121">String</span></span>|<span data-ttu-id="e72b6-122">Der Titel des Plans zum Zeitpunkt der Benutzer es angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e72b6-122">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e72b6-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e72b6-123">JSON representation</span></span>

<span data-ttu-id="e72b6-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e72b6-124">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerRecentPlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
