---
title: Ressourcentyp governanceSchedule
description: 'Stellt den Zeitplan für einen GovernanceRoleAssignmentRequest dar. Der Zeitplan für eine Rolle Zuordnung Anforderung steuert beim Ausführen dieses Vorgangs Rolle Zuordnung für die rollenzuweisung beenden und wie häufig die Rolle Zuordnung Operation durchzuführen. '
localization_priority: Normal
ms.openlocfilehash: 8bf36b786adbd8064ee0c00c0ce293408c6e2b7f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882313"
---
# <a name="governanceschedule-resource-type"></a><span data-ttu-id="a6669-104">Ressourcentyp governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="a6669-104">governanceSchedule resource type</span></span>

> <span data-ttu-id="a6669-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a6669-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6669-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a6669-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6669-107">Stellt den Zeitplan für einen [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)dar.</span><span class="sxs-lookup"><span data-stu-id="a6669-107">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="a6669-108">Der Zeitplan für eine Rolle Zuordnung Anforderung steuert beim Ausführen dieses Vorgangs Rolle Zuordnung für die rollenzuweisung beenden und wie häufig die Rolle Zuordnung Operation durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="a6669-108">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="a6669-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a6669-109">Properties</span></span>
| <span data-ttu-id="a6669-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a6669-110">Property</span></span>     | <span data-ttu-id="a6669-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a6669-111">Type</span></span>   |<span data-ttu-id="a6669-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a6669-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6669-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a6669-113">startDateTime</span></span>|<span data-ttu-id="a6669-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6669-114">DateTimeOffset</span></span>|<span data-ttu-id="a6669-115">Die Anfangszeit der rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="a6669-115">The start time of the role assignment.</span></span> <span data-ttu-id="a6669-116">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="a6669-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a6669-117">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a6669-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a6669-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a6669-118">endDateTime</span></span>|<span data-ttu-id="a6669-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6669-119">DateTimeOffset</span></span>|<span data-ttu-id="a6669-120">Die Endzeit der rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="a6669-120">The end time of the role assignment.</span></span> <span data-ttu-id="a6669-121">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="a6669-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a6669-122">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a6669-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="a6669-123">*Hinweis: Wenn der Wert ist `null`, es gibt eine permanente Zuordnung an.*</span><span class="sxs-lookup"><span data-stu-id="a6669-123">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="a6669-124">type</span><span class="sxs-lookup"><span data-stu-id="a6669-124">type</span></span>|<span data-ttu-id="a6669-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a6669-125">String</span></span>|<span data-ttu-id="a6669-126">Die rollenzuweisung planen Typ.</span><span class="sxs-lookup"><span data-stu-id="a6669-126">The role assignment schedule type.</span></span> <span data-ttu-id="a6669-127">Nur `Once` wird jetzt unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a6669-127">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="a6669-128">duration</span><span class="sxs-lookup"><span data-stu-id="a6669-128">duration</span></span>|<span data-ttu-id="a6669-129">Duration</span><span class="sxs-lookup"><span data-stu-id="a6669-129">Duration</span></span>|<span data-ttu-id="a6669-130">Die Dauer einer rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="a6669-130">The duration of a role assignment.</span></span> <span data-ttu-id="a6669-131">Es ist eine TimeSpan-Format.</span><span class="sxs-lookup"><span data-stu-id="a6669-131">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6669-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a6669-132">JSON representation</span></span>

<span data-ttu-id="a6669-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a6669-133">Here is a JSON representation of the resource.</span></span>

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
