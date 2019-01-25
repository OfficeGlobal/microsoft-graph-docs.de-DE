---
title: Ressourcentyp plannerPlanContext
description: Die Ressource **PlannerPlanContext** stellt die Beziehung zwischen einem PlannerPlan zu einer Benutzeroberfläche außerhalb Planner dar. Pläne in Planner können in anderen Erfahrungen, beispielsweise Microsoft-Teams, zum Nachverfolgen von Arbeit im Zusammenhang mit dieser Erfahrungen verfügbar gemacht werden.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 76260b51bc6f77acf6fac22e80bd676edd8b8e11
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509238"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="e3367-104">Ressourcentyp plannerPlanContext</span><span class="sxs-lookup"><span data-stu-id="e3367-104">plannerPlanContext resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3367-105">Die Ressource **PlannerPlanContext** stellt die Beziehung zwischen einem [PlannerPlan](plannerplan.md) zu einer Benutzeroberfläche außerhalb Planner dar.</span><span class="sxs-lookup"><span data-stu-id="e3367-105">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="e3367-106">Pläne in Planner können in anderen Erfahrungen, beispielsweise Microsoft-Teams, zum Nachverfolgen von Arbeit im Zusammenhang mit dieser Erfahrungen verfügbar gemacht werden.</span><span class="sxs-lookup"><span data-stu-id="e3367-106">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span>
<span data-ttu-id="e3367-107">Die Erfahrung, die der Eintrag **PlannerPlanContext** reresents kann auf Basis der **OwnerAppId** -Eigenschaft identifiziert werden:</span><span class="sxs-lookup"><span data-stu-id="e3367-107">The experience the **plannerPlanContext** entry reresents can be identified based on the **ownerAppId** property:</span></span>
 - <span data-ttu-id="e3367-108">5e3ce6c0-2b1f-4285-8d4b-75ee78787346: der Kontext Eintrag gehört zum Microsoft-Teams.</span><span class="sxs-lookup"><span data-stu-id="e3367-108">5e3ce6c0-2b1f-4285-8d4b-75ee78787346 : The context entry belongs to Microsoft Teams.</span></span>
 - <span data-ttu-id="e3367-109">00000003-0000-0ff1-CE00-000000000000: der Eintrag Kontext zu SharePoint gehört.</span><span class="sxs-lookup"><span data-stu-id="e3367-109">00000003-0000-0ff1-ce00-000000000000 : The context entry belongs to SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="e3367-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e3367-110">Properties</span></span>
| <span data-ttu-id="e3367-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e3367-111">Property</span></span>     | <span data-ttu-id="e3367-112">Typ</span><span class="sxs-lookup"><span data-stu-id="e3367-112">Type</span></span>   |<span data-ttu-id="e3367-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3367-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3367-114">associationType</span><span class="sxs-lookup"><span data-stu-id="e3367-114">associationType</span></span>|<span data-ttu-id="e3367-115">String</span><span class="sxs-lookup"><span data-stu-id="e3367-115">String</span></span>|<span data-ttu-id="e3367-116">Nullwerte zulassend.</span><span class="sxs-lookup"><span data-stu-id="e3367-116">Nullable.</span></span> <span data-ttu-id="e3367-117">Eine app-benutzerdefinierten Typ der Zuordnung zwischen der [PlannerPlan](plannerplan.md) und die app.</span><span class="sxs-lookup"><span data-stu-id="e3367-117">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="e3367-118">Diese Informationen können die app verschiedene Arten von Beziehungen an den gleichen [PlannerPlan](plannerplan.md)verfolgen.</span><span class="sxs-lookup"><span data-stu-id="e3367-118">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="e3367-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3367-119">createdDateTime</span></span>|<span data-ttu-id="e3367-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3367-120">DateTimeOffset</span></span>|<span data-ttu-id="e3367-121">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e3367-121">Read-only.</span></span> <span data-ttu-id="e3367-122">Datum und Uhrzeit der Erstellung der **PlannerPlanContext** .</span><span class="sxs-lookup"><span data-stu-id="e3367-122">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="e3367-123">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="e3367-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e3367-124">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e3367-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e3367-125">displayNameSegments</span><span class="sxs-lookup"><span data-stu-id="e3367-125">displayNameSegments</span></span>|<span data-ttu-id="e3367-126">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="e3367-126">String collection</span></span>|<span data-ttu-id="e3367-127">Der Name der externen Erfahrung-Segmente.</span><span class="sxs-lookup"><span data-stu-id="e3367-127">The segments of the name of the external experience.</span></span> <span data-ttu-id="e3367-128">Segmente sind eine hierarchische Struktur, die anderen apps auf die Beziehung anzeigen kann.</span><span class="sxs-lookup"><span data-stu-id="e3367-128">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="e3367-129">ownerAppId</span><span class="sxs-lookup"><span data-stu-id="e3367-129">ownerAppId</span></span>|<span data-ttu-id="e3367-130">String</span><span class="sxs-lookup"><span data-stu-id="e3367-130">String</span></span>|<span data-ttu-id="e3367-131">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="e3367-131">Read-only.</span></span> <span data-ttu-id="e3367-132">Die ID der app, die die **PlannerPlanContext**erstellt.</span><span class="sxs-lookup"><span data-stu-id="e3367-132">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3367-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e3367-133">JSON representation</span></span>

<span data-ttu-id="e3367-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e3367-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContext"
}-->

```json
{
  "associationType": "Board",
  "createdDateTime": "2015-10-14T00:57:28.4698344Z",
  "displayNameSegments": [
    "Finance Team",
    "Budget Plans"
  ],
  "ownerAppId": "5e3ce6c0-2b1f-4285-8d4b-75ee78787346"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontext.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
