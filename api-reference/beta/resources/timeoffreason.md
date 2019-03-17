---
title: timeOffReason-Ressourcentyp
description: Ein gültiger Grund, die Zeitdauer im Zeitplan zu übernehmen.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 72597fa1678110a40b9dd1a0ea6e6235625144ab
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657532"
---
# <a name="timeoffreason-resource-type"></a><span data-ttu-id="f5c48-103">timeOffReason-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f5c48-103">timeOffReason resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5c48-104">Ein gültiger Grund für eine [timeOff](timeoff.md) -Instanz in einem [Zeitplan](schedule.md).</span><span class="sxs-lookup"><span data-stu-id="f5c48-104">A valid reason to for a [timeOff](timeoff.md) instance in a [schedule](schedule.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f5c48-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="f5c48-105">Methods</span></span>

| <span data-ttu-id="f5c48-106">Methode</span><span class="sxs-lookup"><span data-stu-id="f5c48-106">Method</span></span>       | <span data-ttu-id="f5c48-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f5c48-107">Return Type</span></span>  |<span data-ttu-id="f5c48-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5c48-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f5c48-109">TimeOffReason erstellen</span><span class="sxs-lookup"><span data-stu-id="f5c48-109">Create timeOffReason</span></span>](../api/schedule-post-timeoffreasons.md) | [<span data-ttu-id="f5c48-110">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="f5c48-110">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="f5c48-111">Erstellen Sie eine `timeOffReason`neue.</span><span class="sxs-lookup"><span data-stu-id="f5c48-111">Create a new `timeOffReason`.</span></span>|
|[<span data-ttu-id="f5c48-112">TimeOffReason aufListen</span><span class="sxs-lookup"><span data-stu-id="f5c48-112">List timeOffReason</span></span>](../api/schedule-list-timeoffreasons.md) | <span data-ttu-id="f5c48-113">[timeOffReason](timeoffreason.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="f5c48-113">[timeOffReason](timeoffreason.md) collection</span></span> | <span data-ttu-id="f5c48-114">Abrufen der Liste der `timeOffReasons` in einem Zeitplan.</span><span class="sxs-lookup"><span data-stu-id="f5c48-114">Get the list of `timeOffReasons` in a schedule.</span></span>|
|[<span data-ttu-id="f5c48-115">TimeOffReason abrufen</span><span class="sxs-lookup"><span data-stu-id="f5c48-115">Get timeOffReason</span></span>](../api/timeoffreason-get.md) | [<span data-ttu-id="f5c48-116">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="f5c48-116">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="f5c48-117">Rufen Sie `timeOffReason` eine nach ID ab.</span><span class="sxs-lookup"><span data-stu-id="f5c48-117">Get a `timeOffReason` by ID.</span></span>|
|[<span data-ttu-id="f5c48-118">TimeOffReason ersetzen</span><span class="sxs-lookup"><span data-stu-id="f5c48-118">Replace timeOffReason</span></span>](../api/timeoffreason-put.md) | [<span data-ttu-id="f5c48-119">timeOffReason</span><span class="sxs-lookup"><span data-stu-id="f5c48-119">timeOffReason</span></span>](timeoffreason.md) | <span data-ttu-id="f5c48-120">Ersetzen Sie `timeOffReason`a.</span><span class="sxs-lookup"><span data-stu-id="f5c48-120">Replace a `timeOffReason`.</span></span>|
|[<span data-ttu-id="f5c48-121">TimeOffReason löschen</span><span class="sxs-lookup"><span data-stu-id="f5c48-121">Delete timeOffReason</span></span>](../api/timeoffreason-delete.md) | <span data-ttu-id="f5c48-122">None</span><span class="sxs-lookup"><span data-stu-id="f5c48-122">None</span></span> | <span data-ttu-id="f5c48-123">Als `timeOffReason` inaktiv markieren.</span><span class="sxs-lookup"><span data-stu-id="f5c48-123">Mark `timeOffReason` as inactive.</span></span>|

## <a name="properties"></a><span data-ttu-id="f5c48-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f5c48-124">Properties</span></span>
|<span data-ttu-id="f5c48-125">Name</span><span class="sxs-lookup"><span data-stu-id="f5c48-125">Name</span></span>          |<span data-ttu-id="f5c48-126">Typ</span><span class="sxs-lookup"><span data-stu-id="f5c48-126">Type</span></span>           |<span data-ttu-id="f5c48-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f5c48-127">Description</span></span>                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| <span data-ttu-id="f5c48-128">id</span><span class="sxs-lookup"><span data-stu-id="f5c48-128">id</span></span>            |`string`      |<span data-ttu-id="f5c48-129">ID des `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="f5c48-129">ID of the `timeOffReason`.</span></span>|
| <span data-ttu-id="f5c48-130">displayName</span><span class="sxs-lookup"><span data-stu-id="f5c48-130">displayName</span></span>               | `string`                  | <span data-ttu-id="f5c48-131">Der Name des `timeOffReason`.</span><span class="sxs-lookup"><span data-stu-id="f5c48-131">The name of the `timeOffReason`.</span></span> <span data-ttu-id="f5c48-132">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f5c48-132">Required.</span></span> |
| <span data-ttu-id="f5c48-133">icontype</span><span class="sxs-lookup"><span data-stu-id="f5c48-133">iconType</span></span> | `enum`   | <span data-ttu-id="f5c48-134">Unterstützte Symboltypen: None; Auto Kalender ausgeführt Ebene FirstAid Arzt notWorking; Takt juryDuty; weltweit Tasse Telefon Wetter Schirm Piggybank Hund Kuchen trafficCone; PIN sonnigen.</span><span class="sxs-lookup"><span data-stu-id="f5c48-134">Supported icon types: none; car; calendar; running; plane; firstAid; doctor; notWorking; clock; juryDuty; globe; cup; phone; weather; umbrella; piggyBank; dog; cake; trafficCone; pin; sunny.</span></span> <span data-ttu-id="f5c48-135">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f5c48-135">Required.</span></span> |
| <span data-ttu-id="f5c48-136">isActive</span><span class="sxs-lookup"><span data-stu-id="f5c48-136">isActive</span></span>          |`bool`      | <span data-ttu-id="f5c48-137">Gibt an, `timeOffReason` ob die verwendet werden kann, wenn neue Entitäten erstellt oder vorhandene aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="f5c48-137">Indicates whether the `timeOffReason` can be used when creating new entities or updating existing ones.</span></span> <span data-ttu-id="f5c48-138">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f5c48-138">Required.</span></span> |
| <span data-ttu-id="f5c48-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f5c48-139">createdDateTime</span></span>       |`DateTimeOffset`        |<span data-ttu-id="f5c48-140">Der Zeitstempel, an dem `timeOffReason` dieser zuerst erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="f5c48-140">The time stamp on which this `timeOffReason` was first created.</span></span> <span data-ttu-id="f5c48-141">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="f5c48-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f5c48-142">Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="f5c48-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="f5c48-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5c48-143">lastModifiedDateTime</span></span>      |`DateTimeOffset`         |<span data-ttu-id="f5c48-144">Der Zeitstempel, an dem `timeOffReason` dieser zuletzt aktualisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="f5c48-144">The time stamp on which this `timeOffReason` was last updated.</span></span> <span data-ttu-id="f5c48-145">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="f5c48-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f5c48-146">Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="f5c48-146">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="f5c48-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f5c48-147">lastModifiedBy</span></span>        |`microsoft.graph.identitySet`        |<span data-ttu-id="f5c48-148">Die Identität, die zuletzt aktualisiert `timeOffReason`hat.</span><span class="sxs-lookup"><span data-stu-id="f5c48-148">The identity that last updated this `timeOffReason`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5c48-149">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f5c48-149">JSON representation</span></span>

<span data-ttu-id="f5c48-150">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f5c48-150">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason"
}-->

```json
{
  "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true,
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffReason resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoffreason.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
