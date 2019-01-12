---
title: Ressourcentyp plannerRecentPlanReference
description: 'Die Ressource **PlannerRecentPlanReference** Repesents Geben Sie einen Verweis auf eine PlannerPlan, die kürzlich von einem Benutzer angezeigt wurde. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: bafaf6d20dc8f64ffe49eb4e2f998607708a2773
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943529"
---
# <a name="plannerrecentplanreference-resource-type"></a><span data-ttu-id="d3196-103">Ressourcentyp plannerRecentPlanReference</span><span class="sxs-lookup"><span data-stu-id="d3196-103">plannerRecentPlanReference resource type</span></span>

> <span data-ttu-id="d3196-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d3196-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3196-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d3196-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d3196-106">Die Ressource **PlannerRecentPlanReference** Repesents Geben Sie einen Verweis auf eine [PlannerPlan](plannerplan.md) , die kürzlich von einem Benutzer angezeigt wurde.</span><span class="sxs-lookup"><span data-stu-id="d3196-106">The **plannerRecentPlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has recently been viewed by a user.</span></span> <span data-ttu-id="d3196-107">Die **PlannerRecentPlanReferences** für einen Benutzer werden explizit verwaltet von apps.</span><span class="sxs-lookup"><span data-stu-id="d3196-107">The **plannerRecentPlanReferences** for a user are explicitly maintained by apps.</span></span> <span data-ttu-id="d3196-108">Alle Apps, die das letzte Pläne Feature implementiert sollte zu notieren, wenn der Benutzer zuletzt einen Plan und Update **PlannerRecentPlanReference** Einträge entsprechend angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d3196-108">Any app that implements the recent plans feature should record when the user last viewed a plan, and update **plannerRecentPlanReference** entries accordingly.</span></span>
<span data-ttu-id="d3196-109">Apps Beachten Sie, dass Einträge **PlannerRecentPlanReference** **PlannerPlans** , die gelöscht werden, die der Benutzer zugreifen kann nicht mehr oder die mit einem anderen Titel aktualisiert wurden, verweisen können.</span><span class="sxs-lookup"><span data-stu-id="d3196-109">Apps should note that **plannerRecentPlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>
<span data-ttu-id="d3196-110">Es wird empfohlen, dass apps benachrichtigen Sie Benutzer bei Diskrepanzen und die Einträge auf dem aktuellen Stand halten.</span><span class="sxs-lookup"><span data-stu-id="d3196-110">We recommend that apps notify users when there are discrepancies and keep the entries up to date.</span></span>

## <a name="properties"></a><span data-ttu-id="d3196-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d3196-111">Properties</span></span>
| <span data-ttu-id="d3196-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d3196-112">Property</span></span>     | <span data-ttu-id="d3196-113">Typ</span><span class="sxs-lookup"><span data-stu-id="d3196-113">Type</span></span>   |<span data-ttu-id="d3196-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3196-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3196-115">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3196-115">lastAccessedDateTime</span></span>|<span data-ttu-id="d3196-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3196-116">DateTimeOffset</span></span>|<span data-ttu-id="d3196-117">Das Datum und die Zeit, die vom Benutzer zuletzt des Plans angezeigt wurde.</span><span class="sxs-lookup"><span data-stu-id="d3196-117">The date and time the plan was last viewed by the user.</span></span> <span data-ttu-id="d3196-118">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="d3196-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d3196-119">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d3196-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d3196-120">planTitle</span><span class="sxs-lookup"><span data-stu-id="d3196-120">planTitle</span></span>|<span data-ttu-id="d3196-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d3196-121">String</span></span>|<span data-ttu-id="d3196-122">Der Titel des Plans zum Zeitpunkt der Benutzer es angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d3196-122">The title of the plan at the time the user viewed it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3196-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d3196-123">JSON representation</span></span>

<span data-ttu-id="d3196-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d3196-124">The following is a JSON representation of the resource.</span></span>

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
