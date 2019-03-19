---
title: timeOff-Ressourcentyp
description: Eine nicht-Arbeitseinheit im Zeitplan.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c15d65c6d0a5a9749654698a51996cb21c254a9d
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30676989"
---
# <a name="timeoff-resource-type"></a><span data-ttu-id="b433d-103">timeOff-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b433d-103">timeOff resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b433d-104">Eine nicht-Arbeitseinheit im Zeitplan.</span><span class="sxs-lookup"><span data-stu-id="b433d-104">A unit of non-work in the schedule.</span></span>

## <a name="methods"></a><span data-ttu-id="b433d-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="b433d-105">Methods</span></span>

| <span data-ttu-id="b433d-106">Methode</span><span class="sxs-lookup"><span data-stu-id="b433d-106">Method</span></span>       | <span data-ttu-id="b433d-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b433d-107">Return Type</span></span>  |<span data-ttu-id="b433d-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b433d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b433d-109">TimeOff erstellen</span><span class="sxs-lookup"><span data-stu-id="b433d-109">Create timeOff</span></span>](../api/schedule-post-timesoff.md) | [<span data-ttu-id="b433d-110">timeOff</span><span class="sxs-lookup"><span data-stu-id="b433d-110">timeOff</span></span>](timeOff.md) | <span data-ttu-id="b433d-111">Dient zum Erstellen eines neuen Objekts vom Typ `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="b433d-111">Create a new `timeOff` object.</span></span>|
|[<span data-ttu-id="b433d-112">AufListen von zeitOffs</span><span class="sxs-lookup"><span data-stu-id="b433d-112">List timeOffs</span></span>](../api/schedule-list-timesoff.md) | <span data-ttu-id="b433d-113">[timeOff](timeOff.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="b433d-113">[timeOff](timeOff.md) collection</span></span> | <span data-ttu-id="b433d-114">Rufen Sie die Liste `timeOff` der Objekte in diesem Zeitplan ab.</span><span class="sxs-lookup"><span data-stu-id="b433d-114">Get the list of `timeOff` objects in this schedule.</span></span>|
|[<span data-ttu-id="b433d-115">TimeOff abrufen</span><span class="sxs-lookup"><span data-stu-id="b433d-115">Get timeOff</span></span>](../api/timeoff-get.md) | [<span data-ttu-id="b433d-116">timeOff</span><span class="sxs-lookup"><span data-stu-id="b433d-116">timeOff</span></span>](timeOff.md) | <span data-ttu-id="b433d-117">Rufen Sie `timeOff` eine nach ID ab.</span><span class="sxs-lookup"><span data-stu-id="b433d-117">Get a `timeOff` by ID.</span></span>|
|[<span data-ttu-id="b433d-118">TimeOff ersetzen</span><span class="sxs-lookup"><span data-stu-id="b433d-118">Replace timeOff</span></span>](../api/timeoff-put.md) | [<span data-ttu-id="b433d-119">timeOff</span><span class="sxs-lookup"><span data-stu-id="b433d-119">timeOff</span></span>](timeOff.md) | <span data-ttu-id="b433d-120">Ersetzen Sie `timeOff`a.</span><span class="sxs-lookup"><span data-stu-id="b433d-120">Replace a `timeOff`.</span></span>|
|[<span data-ttu-id="b433d-121">TimeOff löschen</span><span class="sxs-lookup"><span data-stu-id="b433d-121">Delete timeOff</span></span>](../api/timeoff-delete.md) | <span data-ttu-id="b433d-122">Keine</span><span class="sxs-lookup"><span data-stu-id="b433d-122">None</span></span> | <span data-ttu-id="b433d-123">Löschen Sie `timeOff` eine aus dem Zeitplan.</span><span class="sxs-lookup"><span data-stu-id="b433d-123">Delete a `timeOff` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="b433d-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b433d-124">Properties</span></span>
|<span data-ttu-id="b433d-125">Name</span><span class="sxs-lookup"><span data-stu-id="b433d-125">Name</span></span>          |<span data-ttu-id="b433d-126">Typ</span><span class="sxs-lookup"><span data-stu-id="b433d-126">Type</span></span>           |<span data-ttu-id="b433d-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b433d-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b433d-128">id</span><span class="sxs-lookup"><span data-stu-id="b433d-128">id</span></span>            |`string`      |<span data-ttu-id="b433d-129">ID des `timeOff`.</span><span class="sxs-lookup"><span data-stu-id="b433d-129">ID of the `timeOff`.</span></span>|
| <span data-ttu-id="b433d-130">userId</span><span class="sxs-lookup"><span data-stu-id="b433d-130">userId</span></span>            |`string`      |<span data-ttu-id="b433d-131">Die ID des Benutzers, der dem `timeOff`zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="b433d-131">ID of the user assigned to the `timeOff`.</span></span> <span data-ttu-id="b433d-132">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b433d-132">Required.</span></span>|
| <span data-ttu-id="b433d-133">sharedTimeOff</span><span class="sxs-lookup"><span data-stu-id="b433d-133">sharedTimeOff</span></span>     |[<span data-ttu-id="b433d-134">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="b433d-134">timeOffItem</span></span>](timeoffitem.md)  |<span data-ttu-id="b433d-135">Die freigegebene `timeOff` Version dieses, die sowohl von Mitarbeitern als auch von Managern angezeigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="b433d-135">The shared version of this `timeOff` that is viewable by both employees and managers.</span></span> <span data-ttu-id="b433d-136">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b433d-136">Required.</span></span>|
| <span data-ttu-id="b433d-137">draftTimeOff</span><span class="sxs-lookup"><span data-stu-id="b433d-137">draftTimeOff</span></span>      |[<span data-ttu-id="b433d-138">timeOffItem</span><span class="sxs-lookup"><span data-stu-id="b433d-138">timeOffItem</span></span>](timeoffitem.md)        |<span data-ttu-id="b433d-139">Die Entwurfsversion dieses `timeOff` , die von Managern angezeigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="b433d-139">The draft version of this `timeOff` that is viewable by managers.</span></span> <span data-ttu-id="b433d-140">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b433d-140">Required.</span></span>|
| <span data-ttu-id="b433d-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b433d-141">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="b433d-142">Der Zeitstempel, an dem `timeOff` dieser zuerst erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="b433d-142">The time stamp at which this `timeOff` was first created.</span></span> <span data-ttu-id="b433d-143">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="b433d-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b433d-144">Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="b433d-144">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="b433d-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b433d-145">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="b433d-146">Der Zeitstempel, an dem `timeOff` dieser zuletzt aktualisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="b433d-146">The time stamp at which this `timeOff` was last updated.</span></span> <span data-ttu-id="b433d-147">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="b433d-147">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b433d-148">Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="b433d-148">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="b433d-149">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b433d-149">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="b433d-150">Die Identität, die zuletzt aktualisiert `timeOff`hat.</span><span class="sxs-lookup"><span data-stu-id="b433d-150">The identity that last updated this `timeOff`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b433d-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b433d-151">JSON representation</span></span>

<span data-ttu-id="b433d-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b433d-152">Here is a JSON representation of the resource.</span></span>

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
