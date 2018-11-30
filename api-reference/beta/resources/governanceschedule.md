---
title: Ressourcentyp governanceSchedule
description: 'Stellt den Zeitplan für einen GovernanceRoleAssignmentRequest dar. Der Zeitplan für eine Rolle Zuordnung Anforderung steuert beim Ausführen dieses Vorgangs Rolle Zuordnung für die rollenzuweisung beenden und wie häufig die Rolle Zuordnung Operation durchzuführen. '
ms.openlocfilehash: 6eff3977aa7806c975f968b8706f2e8c21e5d99e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063203"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="185dd-104">Ressourcentyp governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="185dd-104">governanceSchedule resource type</span></span>

> <span data-ttu-id="185dd-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="185dd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="185dd-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="185dd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="185dd-107">Stellt den Zeitplan für einen [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)dar.</span><span class="sxs-lookup"><span data-stu-id="185dd-107">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="185dd-108">Der Zeitplan für eine Rolle Zuordnung Anforderung steuert beim Ausführen dieses Vorgangs Rolle Zuordnung für die rollenzuweisung beenden und wie häufig die Rolle Zuordnung Operation durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="185dd-108">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="185dd-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="185dd-109">Properties</span></span>
| <span data-ttu-id="185dd-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="185dd-110">Property</span></span>     | <span data-ttu-id="185dd-111">Typ</span><span class="sxs-lookup"><span data-stu-id="185dd-111">Type</span></span>   |<span data-ttu-id="185dd-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="185dd-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="185dd-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="185dd-113">startDateTime</span></span>|<span data-ttu-id="185dd-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="185dd-114">DateTimeOffset</span></span>|<span data-ttu-id="185dd-115">Die Anfangszeit der rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="185dd-115">The start time of the role assignment.</span></span> <span data-ttu-id="185dd-116">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="185dd-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="185dd-117">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="185dd-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="185dd-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="185dd-118">endDateTime</span></span>|<span data-ttu-id="185dd-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="185dd-119">DateTimeOffset</span></span>|<span data-ttu-id="185dd-120">Die Endzeit der rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="185dd-120">The end time of the role assignment.</span></span> <span data-ttu-id="185dd-121">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="185dd-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="185dd-122">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="185dd-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="185dd-123">*Hinweis: Wenn der Wert ist `null`, es gibt eine permanente Zuordnung an.*</span><span class="sxs-lookup"><span data-stu-id="185dd-123">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="185dd-124">Typ</span><span class="sxs-lookup"><span data-stu-id="185dd-124">type</span></span>|<span data-ttu-id="185dd-125">String</span><span class="sxs-lookup"><span data-stu-id="185dd-125">String</span></span>|<span data-ttu-id="185dd-126">Die rollenzuweisung planen Typ.</span><span class="sxs-lookup"><span data-stu-id="185dd-126">The role assignment schedule type.</span></span> <span data-ttu-id="185dd-127">Nur `Once` wird jetzt unterstützt.</span><span class="sxs-lookup"><span data-stu-id="185dd-127">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="185dd-128">duration</span><span class="sxs-lookup"><span data-stu-id="185dd-128">duration</span></span>|<span data-ttu-id="185dd-129">Duration</span><span class="sxs-lookup"><span data-stu-id="185dd-129">Duration</span></span>|<span data-ttu-id="185dd-130">Die Dauer einer rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="185dd-130">The duration of a role assignment.</span></span> <span data-ttu-id="185dd-131">Es ist eine TimeSpan-Format.</span><span class="sxs-lookup"><span data-stu-id="185dd-131">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="185dd-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="185dd-132">JSON representation</span></span>

<span data-ttu-id="185dd-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="185dd-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSchedule"
}-->

```json
{
  "duration": "String (timespan)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
