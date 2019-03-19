---
title: Schicht-Ressourcentyp
description: Eine Schicht ist eine Einheit der geplanten Arbeit im Zeitplan.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cd80cd36bd32ea9efba9e565aabd2da963c51ec8
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30676968"
---
# <a name="shift-resource-type"></a><span data-ttu-id="de646-103">Schicht-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="de646-103">shift resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de646-104">Eine Einheit der geplanten Arbeit in einem [Zeitplan](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="de646-104">A unit of scheduled work in a [schedule](schedule.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="de646-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="de646-105">Methods</span></span>

| <span data-ttu-id="de646-106">Methode</span><span class="sxs-lookup"><span data-stu-id="de646-106">Method</span></span>       | <span data-ttu-id="de646-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="de646-107">Return Type</span></span>  |<span data-ttu-id="de646-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de646-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="de646-109">Schicht erstellen</span><span class="sxs-lookup"><span data-stu-id="de646-109">Create shift</span></span>](../api/schedule-post-shifts.md) | [<span data-ttu-id="de646-110">UMSCHALT</span><span class="sxs-lookup"><span data-stu-id="de646-110">shift</span></span>](shift.md) | <span data-ttu-id="de646-111">Erstellen Sie eine `shift`neue.</span><span class="sxs-lookup"><span data-stu-id="de646-111">Create a new `shift`.</span></span>|
|[<span data-ttu-id="de646-112">Listen Verschiebungen</span><span class="sxs-lookup"><span data-stu-id="de646-112">List shifts</span></span>](../api/schedule-list-shifts.md) | <span data-ttu-id="de646-113">[Shift](shift.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="de646-113">[shift](shift.md) collection</span></span> | <span data-ttu-id="de646-114">Rufen Sie die Liste `shifts` der in diesem Zeitplan ab.</span><span class="sxs-lookup"><span data-stu-id="de646-114">Get the list of `shifts` in this schedule.</span></span>|
|[<span data-ttu-id="de646-115">Shift abrufen</span><span class="sxs-lookup"><span data-stu-id="de646-115">Get shift</span></span>](../api/shift-get.md) | [<span data-ttu-id="de646-116">UMSCHALT</span><span class="sxs-lookup"><span data-stu-id="de646-116">shift</span></span>](shift.md) | <span data-ttu-id="de646-117">Rufen Sie `shift` eine nach ID ab.</span><span class="sxs-lookup"><span data-stu-id="de646-117">Get a `shift` by ID.</span></span>|
|[<span data-ttu-id="de646-118">UMSCHALT ersetzen</span><span class="sxs-lookup"><span data-stu-id="de646-118">Replace shift</span></span>](../api/shift-put.md) | [<span data-ttu-id="de646-119">UMSCHALT</span><span class="sxs-lookup"><span data-stu-id="de646-119">shift</span></span>](shift.md) | <span data-ttu-id="de646-120">Ersetzen Sie `shift`a.</span><span class="sxs-lookup"><span data-stu-id="de646-120">Replace a `shift`.</span></span>|
|[<span data-ttu-id="de646-121">Schicht löschen</span><span class="sxs-lookup"><span data-stu-id="de646-121">Delete shift</span></span>](../api/shift-delete.md) | <span data-ttu-id="de646-122">Keine</span><span class="sxs-lookup"><span data-stu-id="de646-122">None</span></span> | <span data-ttu-id="de646-123">Löschen Sie `shift` eine aus dem Zeitplan.</span><span class="sxs-lookup"><span data-stu-id="de646-123">Delete a `shift` from the schedule.</span></span>|

## <a name="properties"></a><span data-ttu-id="de646-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="de646-124">Properties</span></span>
|<span data-ttu-id="de646-125">Name</span><span class="sxs-lookup"><span data-stu-id="de646-125">Name</span></span>          |<span data-ttu-id="de646-126">Typ</span><span class="sxs-lookup"><span data-stu-id="de646-126">Type</span></span>           |<span data-ttu-id="de646-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de646-127">Description</span></span>                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="de646-128">id</span><span class="sxs-lookup"><span data-stu-id="de646-128">id</span></span>            |`string`      |<span data-ttu-id="de646-129">ID des `shift`.</span><span class="sxs-lookup"><span data-stu-id="de646-129">ID of the `shift`.</span></span>|
| <span data-ttu-id="de646-130">userId</span><span class="sxs-lookup"><span data-stu-id="de646-130">userId</span></span>            |`string`      |<span data-ttu-id="de646-131">Die ID des Benutzers, der dem `shift`zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="de646-131">ID of the user assigned to the `shift`.</span></span> <span data-ttu-id="de646-132">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="de646-132">Required.</span></span> |
| <span data-ttu-id="de646-133">schedulingGroupId</span><span class="sxs-lookup"><span data-stu-id="de646-133">schedulingGroupId</span></span>         |`string`      |<span data-ttu-id="de646-134">Die ID der Planungsgruppe, `shift` in der Sie enthalten ist.</span><span class="sxs-lookup"><span data-stu-id="de646-134">ID of the scheduling group the `shift` is part of.</span></span> <span data-ttu-id="de646-135">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="de646-135">Required.</span></span> |
| <span data-ttu-id="de646-136">sharedShift</span><span class="sxs-lookup"><span data-stu-id="de646-136">sharedShift</span></span>   |[<span data-ttu-id="de646-137">shiftItem</span><span class="sxs-lookup"><span data-stu-id="de646-137">shiftItem</span></span>](shiftitem.md)  |<span data-ttu-id="de646-138">Die freigegebene `shift` Version dieses, die sowohl von Mitarbeitern als auch von Managern angezeigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="de646-138">The shared version of this `shift` that is viewable by both employees and managers.</span></span> <span data-ttu-id="de646-139">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="de646-139">Required.</span></span> |
| <span data-ttu-id="de646-140">draftShift</span><span class="sxs-lookup"><span data-stu-id="de646-140">draftShift</span></span>        |[<span data-ttu-id="de646-141">shiftItem</span><span class="sxs-lookup"><span data-stu-id="de646-141">shiftItem</span></span>](shiftitem.md)        |<span data-ttu-id="de646-142">Die Entwurfsversion dieses `shift` , die von Managern angezeigt werden kann.</span><span class="sxs-lookup"><span data-stu-id="de646-142">The draft version of this `shift` that is viewable by managers.</span></span> <span data-ttu-id="de646-143">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="de646-143">Required.</span></span> |
| <span data-ttu-id="de646-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de646-144">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="de646-145">Der Zeitstempel, für `shift` den dies zuerst erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="de646-145">The timestamp on which this `shift` was first created.</span></span> <span data-ttu-id="de646-146">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="de646-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="de646-147">Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="de646-147">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="de646-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de646-148">lastModifiedDateTime</span></span>      |`DateTimeOffset`        |<span data-ttu-id="de646-149">Der Zeitstempel, an `shift` dem dieser zuletzt aktualisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="de646-149">The timestamp on which this `shift` was last updated.</span></span> <span data-ttu-id="de646-150">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="de646-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="de646-151">Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="de646-151">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="de646-152">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="de646-152">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="de646-153">Die Identität, die zuletzt aktualisiert `shift`hat.</span><span class="sxs-lookup"><span data-stu-id="de646-153">The identity that last updated this `shift`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de646-154">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="de646-154">JSON representation</span></span>

<span data-ttu-id="de646-155">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="de646-155">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shift"
}-->

```json
{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/shift.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->