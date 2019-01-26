---
title: Ressourcentyp governanceSchedule
description: 'Stellt den Zeitplan für einen GovernanceRoleAssignmentRequest dar. Der Zeitplan für eine Rolle Zuordnung Anforderung steuert beim Ausführen dieses Vorgangs Rolle Zuordnung für die rollenzuweisung beenden und wie häufig die Rolle Zuordnung Operation durchzuführen. '
localization_priority: Normal
ms.openlocfilehash: 11ac010829309c9b701e20da8ad40ebf905e02ba
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575251"
---
# <a name="microsoftgraphgovernanceschedule-resource-type"></a><span data-ttu-id="72118-104">Ressourcentyp microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="72118-104">microsoft.graph.governanceSchedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72118-105">Stellt den Zeitplan für einen [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)dar.</span><span class="sxs-lookup"><span data-stu-id="72118-105">Represents the schedule for a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span> <span data-ttu-id="72118-106">Der Zeitplan für eine Rolle Zuordnung Anforderung steuert beim Ausführen dieses Vorgangs Rolle Zuordnung für die rollenzuweisung beenden und wie häufig die Rolle Zuordnung Operation durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="72118-106">For a role assignment request, the schedule controls when to perform the role assignment operation, when to stop the role assignment, and how frequently to do the role assignment operation.</span></span> 



## <a name="properties"></a><span data-ttu-id="72118-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="72118-107">Properties</span></span>
| <span data-ttu-id="72118-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="72118-108">Property</span></span>     | <span data-ttu-id="72118-109">Typ</span><span class="sxs-lookup"><span data-stu-id="72118-109">Type</span></span>   |<span data-ttu-id="72118-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="72118-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72118-111">startDateTime</span><span class="sxs-lookup"><span data-stu-id="72118-111">startDateTime</span></span>|<span data-ttu-id="72118-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72118-112">DateTimeOffset</span></span>|<span data-ttu-id="72118-113">Die Anfangszeit der rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="72118-113">The start time of the role assignment.</span></span> <span data-ttu-id="72118-114">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="72118-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="72118-115">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="72118-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="72118-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="72118-116">endDateTime</span></span>|<span data-ttu-id="72118-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72118-117">DateTimeOffset</span></span>|<span data-ttu-id="72118-118">Die Endzeit der rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="72118-118">The end time of the role assignment.</span></span> <span data-ttu-id="72118-119">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="72118-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="72118-120">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="72118-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="72118-121">*Hinweis: Wenn der Wert ist `null`, es gibt eine permanente Zuordnung an.*</span><span class="sxs-lookup"><span data-stu-id="72118-121">*Note: if the value is `null`, it indicates a permanent assignment.*</span></span>|
|<span data-ttu-id="72118-122">type</span><span class="sxs-lookup"><span data-stu-id="72118-122">type</span></span>|<span data-ttu-id="72118-123">String</span><span class="sxs-lookup"><span data-stu-id="72118-123">String</span></span>|<span data-ttu-id="72118-124">Die rollenzuweisung planen Typ.</span><span class="sxs-lookup"><span data-stu-id="72118-124">The role assignment schedule type.</span></span> <span data-ttu-id="72118-125">Nur `Once` wird jetzt unterstützt.</span><span class="sxs-lookup"><span data-stu-id="72118-125">Only `Once` is supported for now.</span></span>
|<span data-ttu-id="72118-126">duration</span><span class="sxs-lookup"><span data-stu-id="72118-126">duration</span></span>|<span data-ttu-id="72118-127">Dauer</span><span class="sxs-lookup"><span data-stu-id="72118-127">Duration</span></span>|<span data-ttu-id="72118-128">Die Dauer einer rollenzuweisung.</span><span class="sxs-lookup"><span data-stu-id="72118-128">The duration of a role assignment.</span></span> <span data-ttu-id="72118-129">Es ist eine TimeSpan-Format.</span><span class="sxs-lookup"><span data-stu-id="72118-129">It is in format of a TimeSpan.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="72118-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="72118-130">JSON representation</span></span>

<span data-ttu-id="72118-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="72118-131">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "governanceSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceschedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
