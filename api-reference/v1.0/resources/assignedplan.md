---
title: assignedPlan-Ressourcentyp
description: Die **assignedPlans**-Eigenschaft der user-Entität und der oganization-Entität ist eine Sammlung von **assignedPlan**.
ms.openlocfilehash: 306c485b31189e7693075735ceda0812d3259251
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017012"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="56105-103">assignedPlan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="56105-103">assignedPlan resource type</span></span>

<span data-ttu-id="56105-104">Die **assignedPlans**-Eigenschaft der [user](user.md)-Entität und der [oganization](organization.md)-Entität ist eine Sammlung von **assignedPlan**.</span><span class="sxs-lookup"><span data-stu-id="56105-104">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="56105-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="56105-105">Properties</span></span>
| <span data-ttu-id="56105-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="56105-106">Property</span></span>     | <span data-ttu-id="56105-107">Typ</span><span class="sxs-lookup"><span data-stu-id="56105-107">Type</span></span>   |<span data-ttu-id="56105-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56105-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56105-109">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="56105-109">assignedDateTime</span></span>|<span data-ttu-id="56105-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56105-110">DateTimeOffset</span></span>|<span data-ttu-id="56105-p101">Datum und Uhrzeit der Zuweisung des Plans, z. B.: 2013-01-02T19:32:30Z. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="56105-p101">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="56105-114">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="56105-114">capabilityStatus</span></span>|<span data-ttu-id="56105-115">String</span><span class="sxs-lookup"><span data-stu-id="56105-115">String</span></span>|<span data-ttu-id="56105-116">Z. B. „Aktiviert“.</span><span class="sxs-lookup"><span data-stu-id="56105-116">For example, “Enabled”.</span></span>|
|<span data-ttu-id="56105-117">service</span><span class="sxs-lookup"><span data-stu-id="56105-117">service</span></span>|<span data-ttu-id="56105-118">String</span><span class="sxs-lookup"><span data-stu-id="56105-118">String</span></span>|<span data-ttu-id="56105-119">Der Name des Diensts. z. B. „Exchange“.</span><span class="sxs-lookup"><span data-stu-id="56105-119">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="56105-120">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="56105-120">servicePlanId</span></span>|<span data-ttu-id="56105-121">Guid</span><span class="sxs-lookup"><span data-stu-id="56105-121">Guid</span></span>|<span data-ttu-id="56105-122">Eine GUID, die den Serviceplan identifiziert.</span><span class="sxs-lookup"><span data-stu-id="56105-122">A GUID that identifies the service plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56105-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="56105-123">JSON representation</span></span>

<span data-ttu-id="56105-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="56105-124">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedPlan"
}-->

```json
{
  "assignedDateTime": "String (timestamp)",
  "capabilityStatus": "string",
  "service": "string",
  "servicePlanId": "guid"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
