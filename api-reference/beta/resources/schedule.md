---
title: Ressourcentyp planen
description: Eine Sammlung von schedulingGroups, Schichten, timeOffReasons und timesOff innerhalb eines Teams.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: de3662fcf3c5a8e50493e365f6a10a8641a451df
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657511"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="88d69-103">Ressourcentyp planen</span><span class="sxs-lookup"><span data-stu-id="88d69-103">schedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88d69-104">Eine Auflistung von [schedulinggroup](schedulinggroup.md) -Objekten, [Shift](shift.md) -Objekten, [timeOffReason](timeoffreason.md) -Objekten und [timeOff](timeoff.md) -Objekten innerhalb eines [Teams](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="88d69-104">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="88d69-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="88d69-105">Methods</span></span>

| <span data-ttu-id="88d69-106">Methode</span><span class="sxs-lookup"><span data-stu-id="88d69-106">Method</span></span>       | <span data-ttu-id="88d69-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="88d69-107">Return Type</span></span>  |<span data-ttu-id="88d69-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88d69-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="88d69-109">Erstellen oder Ersetzen eines Zeitplans</span><span class="sxs-lookup"><span data-stu-id="88d69-109">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="88d69-110">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="88d69-110">schedule</span></span>](schedule.md) | <span data-ttu-id="88d69-111">Erstellen oder ersetzen Sie `schedule`ein.</span><span class="sxs-lookup"><span data-stu-id="88d69-111">Create or replace a `schedule`.</span></span>|
|[<span data-ttu-id="88d69-112">Zeitplan abrufen</span><span class="sxs-lookup"><span data-stu-id="88d69-112">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="88d69-113">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="88d69-113">schedule</span></span>](schedule.md) | <span data-ttu-id="88d69-114">Get a `schedule`.</span><span class="sxs-lookup"><span data-stu-id="88d69-114">Get a `schedule`.</span></span>|
|[<span data-ttu-id="88d69-115">share</span><span class="sxs-lookup"><span data-stu-id="88d69-115">share</span></span>](../api/schedule-share.md) | <span data-ttu-id="88d69-116">None</span><span class="sxs-lookup"><span data-stu-id="88d69-116">None</span></span> | <span data-ttu-id="88d69-117">Teilen Sie `schedule` einen Zeitraum mit Schedule-Elementen.</span><span class="sxs-lookup"><span data-stu-id="88d69-117">Share a `schedule` time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="88d69-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="88d69-118">Properties</span></span>
|<span data-ttu-id="88d69-119">Name</span><span class="sxs-lookup"><span data-stu-id="88d69-119">Name</span></span>                   |<span data-ttu-id="88d69-120">Typ</span><span class="sxs-lookup"><span data-stu-id="88d69-120">Type</span></span>           |<span data-ttu-id="88d69-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88d69-121">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="88d69-122">id</span><span class="sxs-lookup"><span data-stu-id="88d69-122">id</span></span>                    |`string`  |<span data-ttu-id="88d69-123">ID des `schedule`.</span><span class="sxs-lookup"><span data-stu-id="88d69-123">ID of the `schedule`.</span></span>|
| <span data-ttu-id="88d69-124">aktiviert</span><span class="sxs-lookup"><span data-stu-id="88d69-124">enabled</span></span>               |`bool`    | <span data-ttu-id="88d69-125">Gibt an, ob der Zeitplan für das Team aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="88d69-125">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="88d69-126">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="88d69-126">Required.</span></span>|
| <span data-ttu-id="88d69-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="88d69-127">timeZone</span></span>              |`string`  | <span data-ttu-id="88d69-128">Gibt die Zeitzone des Zeit Plan Teams mit dem TZ-Datenbankformat an.</span><span class="sxs-lookup"><span data-stu-id="88d69-128">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="88d69-129">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="88d69-129">Required.</span></span>|
| <span data-ttu-id="88d69-130">provisionStatus</span><span class="sxs-lookup"><span data-stu-id="88d69-130">provisionStatus</span></span>       |`enum`    | <span data-ttu-id="88d69-131">Der Status der Terminplanung.</span><span class="sxs-lookup"><span data-stu-id="88d69-131">The status of the schedule provisioning.</span></span> |
| <span data-ttu-id="88d69-132">provisionStatusCode</span><span class="sxs-lookup"><span data-stu-id="88d69-132">provisionStatusCode</span></span>   |`string`  | <span data-ttu-id="88d69-133">Weitere Informationen dazu, warum die Planung fehlgeschlagen ist.</span><span class="sxs-lookup"><span data-stu-id="88d69-133">Additional information about why schedule provisioning failed.</span></span> |


## <a name="relationships"></a><span data-ttu-id="88d69-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="88d69-134">Relationships</span></span>
|<span data-ttu-id="88d69-135">Name</span><span class="sxs-lookup"><span data-stu-id="88d69-135">Name</span></span>                   |<span data-ttu-id="88d69-136">Typ</span><span class="sxs-lookup"><span data-stu-id="88d69-136">Type</span></span>           |<span data-ttu-id="88d69-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88d69-137">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="88d69-138">Verschiebungen</span><span class="sxs-lookup"><span data-stu-id="88d69-138">shifts</span></span>   |`collection(shift)`  | <span data-ttu-id="88d69-139">Die Verschiebungen im Zeitplan.</span><span class="sxs-lookup"><span data-stu-id="88d69-139">The shifts in the schedule.</span></span> |
| <span data-ttu-id="88d69-140">timesOff</span><span class="sxs-lookup"><span data-stu-id="88d69-140">timesOff</span></span>   |`collection(timeOff)`  | <span data-ttu-id="88d69-141">Die Instanzen von Zeiten, die im Zeitplan deaktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="88d69-141">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="88d69-142">timeOffReasons</span><span class="sxs-lookup"><span data-stu-id="88d69-142">timeOffReasons</span></span>   |`collection(timeOffReason)`  | <span data-ttu-id="88d69-143">Die Gründe für eine Zeitdauer im Zeitplan.</span><span class="sxs-lookup"><span data-stu-id="88d69-143">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="88d69-144">schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="88d69-144">schedulingGroups</span></span>   |`collection(schedulingGroup)`  | <span data-ttu-id="88d69-145">Die logische Gruppierung von Benutzern im Zeitplan (in der Regel nach Rolle).</span><span class="sxs-lookup"><span data-stu-id="88d69-145">The logical grouping of users in the schedule (usually by role).</span></span> |


## <a name="json-representation"></a><span data-ttu-id="88d69-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="88d69-146">JSON representation</span></span>

<span data-ttu-id="88d69-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="88d69-147">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedule"
}-->

```json
{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/schedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
