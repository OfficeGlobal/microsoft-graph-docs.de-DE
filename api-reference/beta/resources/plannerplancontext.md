---
title: Ressourcentyp plannerPlanContext
description: Die Ressource **PlannerPlanContext** stellt die Beziehung zwischen einem PlannerPlan zu einer Benutzeroberfläche außerhalb Planner dar. Pläne in Planner können in anderen Erfahrungen, beispielsweise Microsoft-Teams, zum Nachverfolgen von Arbeit im Zusammenhang mit dieser Erfahrungen verfügbar gemacht werden.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: e118e32ea74332f0d8d0f958f7c55cd9980acb8f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962891"
---
# <a name="plannerplancontext-resource-type"></a><span data-ttu-id="7cdfa-104">Ressourcentyp plannerPlanContext</span><span class="sxs-lookup"><span data-stu-id="7cdfa-104">plannerPlanContext resource type</span></span>

> <span data-ttu-id="7cdfa-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7cdfa-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7cdfa-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7cdfa-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7cdfa-107">Die Ressource **PlannerPlanContext** stellt die Beziehung zwischen einem [PlannerPlan](plannerplan.md) zu einer Benutzeroberfläche außerhalb Planner dar.</span><span class="sxs-lookup"><span data-stu-id="7cdfa-107">The **plannerPlanContext** resource represents the relationship of a [plannerPlan](plannerplan.md) to a user experience outside of Planner.</span></span> <span data-ttu-id="7cdfa-108">Pläne in Planner können in anderen Erfahrungen, beispielsweise Microsoft-Teams, zum Nachverfolgen von Arbeit im Zusammenhang mit dieser Erfahrungen verfügbar gemacht werden.</span><span class="sxs-lookup"><span data-stu-id="7cdfa-108">Plans in Planner can be surfaced in other experiences, such as Microsoft Teams, to track work in the context of that experience.</span></span>
<span data-ttu-id="7cdfa-109">Die Erfahrung, die der Eintrag **PlannerPlanContext** reresents kann auf Basis der **OwnerAppId** -Eigenschaft identifiziert werden:</span><span class="sxs-lookup"><span data-stu-id="7cdfa-109">The experience the **plannerPlanContext** entry reresents can be identified based on the **ownerAppId** property:</span></span>
 - <span data-ttu-id="7cdfa-110">5e3ce6c0-2b1f-4285-8d4b-75ee78787346: der Kontext Eintrag gehört zum Microsoft-Teams.</span><span class="sxs-lookup"><span data-stu-id="7cdfa-110">5e3ce6c0-2b1f-4285-8d4b-75ee78787346 : The context entry belongs to Microsoft Teams.</span></span>
 - <span data-ttu-id="7cdfa-111">00000003-0000-0ff1-CE00-000000000000: der Eintrag Kontext zu SharePoint gehört.</span><span class="sxs-lookup"><span data-stu-id="7cdfa-111">00000003-0000-0ff1-ce00-000000000000 : The context entry belongs to SharePoint.</span></span>

## <a name="properties"></a><span data-ttu-id="7cdfa-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7cdfa-112">Properties</span></span>
| <span data-ttu-id="7cdfa-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7cdfa-113">Property</span></span>     | <span data-ttu-id="7cdfa-114">Typ</span><span class="sxs-lookup"><span data-stu-id="7cdfa-114">Type</span></span>   |<span data-ttu-id="7cdfa-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7cdfa-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7cdfa-116">associationType</span><span class="sxs-lookup"><span data-stu-id="7cdfa-116">associationType</span></span>|<span data-ttu-id="7cdfa-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7cdfa-117">String</span></span>|<span data-ttu-id="7cdfa-118">Lässt Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="7cdfa-118">Nullable.</span></span> <span data-ttu-id="7cdfa-119">Eine app-benutzerdefinierten Typ der Zuordnung zwischen der [PlannerPlan](plannerplan.md) und die app.</span><span class="sxs-lookup"><span data-stu-id="7cdfa-119">An app-defined type of association between the [plannerPlan](plannerplan.md) and the app.</span></span> <span data-ttu-id="7cdfa-120">Diese Informationen können die app verschiedene Arten von Beziehungen an den gleichen [PlannerPlan](plannerplan.md)verfolgen.</span><span class="sxs-lookup"><span data-stu-id="7cdfa-120">The app can use this information to track different kinds of relationships to the same [plannerPlan](plannerplan.md).</span></span>|
|<span data-ttu-id="7cdfa-121">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7cdfa-121">createdDateTime</span></span>|<span data-ttu-id="7cdfa-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cdfa-122">DateTimeOffset</span></span>|<span data-ttu-id="7cdfa-123">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7cdfa-123">Read-only.</span></span> <span data-ttu-id="7cdfa-124">Datum und Uhrzeit der Erstellung der **PlannerPlanContext** .</span><span class="sxs-lookup"><span data-stu-id="7cdfa-124">The date and time when the **plannerPlanContext** was created.</span></span> <span data-ttu-id="7cdfa-125">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="7cdfa-125">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7cdfa-126">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="7cdfa-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7cdfa-127">displayNameSegments</span><span class="sxs-lookup"><span data-stu-id="7cdfa-127">displayNameSegments</span></span>|<span data-ttu-id="7cdfa-128">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="7cdfa-128">String collection</span></span>|<span data-ttu-id="7cdfa-129">Der Name der externen Erfahrung-Segmente.</span><span class="sxs-lookup"><span data-stu-id="7cdfa-129">The segments of the name of the external experience.</span></span> <span data-ttu-id="7cdfa-130">Segmente sind eine hierarchische Struktur, die anderen apps auf die Beziehung anzeigen kann.</span><span class="sxs-lookup"><span data-stu-id="7cdfa-130">Segments represent a hierarchical structure that allows other apps to display the relationship.</span></span>|
|<span data-ttu-id="7cdfa-131">ownerAppId</span><span class="sxs-lookup"><span data-stu-id="7cdfa-131">ownerAppId</span></span>|<span data-ttu-id="7cdfa-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7cdfa-132">String</span></span>|<span data-ttu-id="7cdfa-133">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7cdfa-133">Read-only.</span></span> <span data-ttu-id="7cdfa-134">Die ID der app, die die **PlannerPlanContext**erstellt.</span><span class="sxs-lookup"><span data-stu-id="7cdfa-134">ID of the app that created the **plannerPlanContext**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7cdfa-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7cdfa-135">JSON representation</span></span>

<span data-ttu-id="7cdfa-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7cdfa-136">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
