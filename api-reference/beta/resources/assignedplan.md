---
title: assignedPlan-Ressourcentyp
description: Die **assignedPlans**-Eigenschaft der user-Entität und der oganization-Entität ist eine Sammlung von **assignedPlan**.
ms.openlocfilehash: 0df1540819b569b62607bf0e56c1c8f53d2749da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058430"
---
# <a name="assignedplan-resource-type"></a><span data-ttu-id="ed30a-103">assignedPlan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ed30a-103">assignedPlan resource type</span></span>

> <span data-ttu-id="ed30a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ed30a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed30a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed30a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ed30a-106">Die **assignedPlans**-Eigenschaft der [user](user.md)-Entität und der [oganization](organization.md)-Entität ist eine Sammlung von **assignedPlan**.</span><span class="sxs-lookup"><span data-stu-id="ed30a-106">The **assignedPlans** property of both the [user](user.md) entity and the [organization](organization.md) entity is a collection of **assignedPlan**.</span></span>


## <a name="properties"></a><span data-ttu-id="ed30a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ed30a-107">Properties</span></span>
| <span data-ttu-id="ed30a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ed30a-108">Property</span></span>     | <span data-ttu-id="ed30a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ed30a-109">Type</span></span>   |<span data-ttu-id="ed30a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed30a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed30a-111">assignedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed30a-111">assignedDateTime</span></span>|<span data-ttu-id="ed30a-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed30a-112">DateTimeOffset</span></span>|<span data-ttu-id="ed30a-p102">Datum und Uhrzeit der Zuweisung des Plans, z. B.: 2013-01-02T19:32:30Z. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ed30a-p102">The date and time at which the plan was assigned; for example: 2013-01-02T19:32:30Z. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ed30a-116">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="ed30a-116">capabilityStatus</span></span>|<span data-ttu-id="ed30a-117">String</span><span class="sxs-lookup"><span data-stu-id="ed30a-117">String</span></span>|<span data-ttu-id="ed30a-118">Z. B. „Aktiviert“.</span><span class="sxs-lookup"><span data-stu-id="ed30a-118">For example, “Enabled”.</span></span>|
|<span data-ttu-id="ed30a-119">service</span><span class="sxs-lookup"><span data-stu-id="ed30a-119">service</span></span>|<span data-ttu-id="ed30a-120">String</span><span class="sxs-lookup"><span data-stu-id="ed30a-120">String</span></span>|<span data-ttu-id="ed30a-121">Der Name des Diensts. z. B. „Exchange“.</span><span class="sxs-lookup"><span data-stu-id="ed30a-121">The name of the service; for example, “Exchange”.</span></span>|
|<span data-ttu-id="ed30a-122">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="ed30a-122">servicePlanId</span></span>|<span data-ttu-id="ed30a-123">Guid</span><span class="sxs-lookup"><span data-stu-id="ed30a-123">Guid</span></span>|<span data-ttu-id="ed30a-124">Eine GUID, die den Serviceplan identifiziert.</span><span class="sxs-lookup"><span data-stu-id="ed30a-124">A GUID that identifies the service plan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed30a-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ed30a-125">JSON representation</span></span>

<span data-ttu-id="ed30a-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ed30a-126">Here is a JSON representation of the resource</span></span>

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
