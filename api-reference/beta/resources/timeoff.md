---
title: timeOff-Ressourcentyp
description: Eine nicht-Arbeitseinheit im Zeitplan.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 933c940e25c772cede7918dabf62b52ee58f18d2
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657798"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="b681d-103">timeOff-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b681d-103">timeOff resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b681d-104">Eine nicht-Arbeitseinheit im Zeitplan.</span><span class="sxs-lookup"><span data-stu-id="b681d-104">A unit of non-work in the schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="b681d-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="b681d-105">Methods</span></span>

| <span data-ttu-id="b681d-106">Methode</span><span class="sxs-lookup"><span data-stu-id="b681d-106">Method</span></span>       | <span data-ttu-id="b681d-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b681d-107">Return Type</span></span>  |<span data-ttu-id="b681d-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b681d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b681d-109">TimeOff erstellen</span><span class="sxs-lookup"><span data-stu-id="b681d-109">Create timeOff</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="b681d-110">timeOff</span><span class="sxs-lookup"><span data-stu-id="b681d-110">timeOff</span></span>](timeOff.md) | <span data-ttu-id="b681d-111">Dient zum Erstellen eines neuen Objekts vom Typ `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="b681d-111">Create a new `timeOff` object.</span></span>|
|[<span data-ttu-id="b681d-112">AufListen von zeitOffs</span><span class="sxs-lookup"><span data-stu-id="b681d-112">List timeOffs</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="b681d-113">[timeOff](timeOff.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="b681d-113">[timeOff](timeOff.md) collection</span></span> | <span data-ttu-id="b681d-114">Rufen Sie die Liste `timeOff` der Objekte in diesem Zeitplan ab.</span><span class="sxs-lookup"><span data-stu-id="b681d-114">Get the list of `timeOff` objects in this schedule.</span></span>|
|[<span data-ttu-id="b681d-115">TimeOff abrufen</span><span class="sxs-lookup"><span data-stu-id="b681d-115">Get timeOff</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="b681d-116">timeOff</span><span class="sxs-lookup"><span data-stu-id="b681d-116">timeOff</span></span>](timeOff.md) | <span data-ttu-id="b681d-117">Rufen Sie `timeOff` eine nach ID ab.</span><span class="sxs-lookup"><span data-stu-id="b681d-117">Get a `timeOff` by ID.</span></span>|
|[<span data-ttu-id="b681d-118">TimeOff ersetzen</span><span class="sxs-lookup"><span data-stu-id="b681d-118">Replace timeOff</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="b681d-119">timeOff</span><span class="sxs-lookup"><span data-stu-id="b681d-119">timeOff</span></span>](timeOff.md) | <span data-ttu-id="b681d-120">Ersetzen Sie `timeOff`a.</span><span class="sxs-lookup"><span data-stu-id="b681d-120">Replace a `timeOff`.</span></span>|
|[<span data-ttu-id="b681d-121">TimeOff löschen</span><span class="sxs-lookup"><span data-stu-id="b681d-121">Delete timeOff</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="b681d-122">None</span><span class="sxs-lookup"><span data-stu-id="b681d-122">None</span></span> | <span data-ttu-id="b681d-123">Löschen Sie `timeOff` eine aus dem Zeitplan.</span><span class="sxs-lookup"><span data-stu-id="b681d-123">Delete a `timeOff` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="b681d-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b681d-124">Properties</span></span>
|<span data-ttu-id="b681d-125">Name</span><span class="sxs-lookup"><span data-stu-id="b681d-125">Name</span></span>          |<span data-ttu-id="b681d-126">Typ</span><span class="sxs-lookup"><span data-stu-id="b681d-126">Type</span></span>           |<span data-ttu-id="b681d-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b681d-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b681d-128">id</span><span class="sxs-lookup"><span data-stu-id="b681d-128">id</span></span>            |`string`      |<span data-ttu-id="b681d-129">ID des `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="b681d-129">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="b681d-130">userId</span><span class="sxs-lookup"><span data-stu-id="b681d-130">userId</span></span>            |`string`      |<span data-ttu-id="b681d-131">Die ID des Benutzers, der dem `timeOff`zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="b681d-131">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="b681d-132">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b681d-132">Required.</span></span>|
| <span data-ttu-id="b681d-133">sharedTimeOff</span><span class="sxs-lookup"><span data-stu-id="b681d-133">sharedTimeOff</span></span>     |`[timeOffItem](timeoffitem.md)`  |<span data-ttu-id="b681d-134">Die freigegebene `timeOff` Version dieses, die sowohl von Mitarbeitern als auch von Managern angezeigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="b681d-134">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="b681d-135">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b681d-135">Required.</span></span>|
| <span data-ttu-id="b681d-136">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="b681d-136">draftTimeOff</span></span>      |`[timeOffItem](timeoffitem.md)`        |<span data-ttu-id="b681d-137">Die Entwurfsversion dieses `timeOff` , die von Managern angezeigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="b681d-137">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="b681d-138">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b681d-138">Required.</span></span>|
| <span data-ttu-id="b681d-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b681d-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="b681d-140">Der Zeitstempel, an dem `timeOff` dieser zuerst erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="b681d-140">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="b681d-141">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="b681d-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b681d-142">Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="b681d-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="b681d-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b681d-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="b681d-144">Der Zeitstempel, an dem `timeOff` dieser zuletzt aktualisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="b681d-144">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="b681d-145">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="b681d-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b681d-146">Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="b681d-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="b681d-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b681d-147">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="b681d-148">Die Identität, die zuletzt aktualisiert `timeOff`hat.</span><span class="sxs-lookup"><span data-stu-id="b681d-148">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b681d-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b681d-149">JSON representation</span></span>

<span data-ttu-id="b681d-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b681d-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff"
}-->

```json
{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOff resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoff.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
