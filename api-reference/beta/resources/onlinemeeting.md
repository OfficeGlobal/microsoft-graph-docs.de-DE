---
title: Ressourcentyp onlineMeeting
description: Erfasst Informationen zu der Besprechung, einschließlich der Join-URL, die Teilnehmerliste und die Beschreibung an.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d7009ceaf815986d50c8eb3b64d2541c32f01a88
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519598"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="437d3-103">Ressourcentyp onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="437d3-103">onlineMeeting resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="437d3-104">Erfasst Informationen zu der Besprechung, einschließlich der Join-URL, die Teilnehmerliste und die Beschreibung an.</span><span class="sxs-lookup"><span data-stu-id="437d3-104">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="437d3-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="437d3-105">Methods</span></span>

| <span data-ttu-id="437d3-106">Methode</span><span class="sxs-lookup"><span data-stu-id="437d3-106">Method</span></span>         | <span data-ttu-id="437d3-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="437d3-107">Return Type</span></span> | <span data-ttu-id="437d3-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="437d3-108">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="437d3-109">Abrufen von onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="437d3-109">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="437d3-110">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="437d3-110">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="437d3-111">Lesen Sie Eigenschaften und Beziehungen OnlineMeeting-Objekts.</span><span class="sxs-lookup"><span data-stu-id="437d3-111">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="437d3-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="437d3-112">Properties</span></span>

| <span data-ttu-id="437d3-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="437d3-113">Property</span></span>                  | <span data-ttu-id="437d3-114">Typ</span><span class="sxs-lookup"><span data-stu-id="437d3-114">Type</span></span>                                                   | <span data-ttu-id="437d3-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="437d3-115">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="437d3-116">AccessLevel</span><span class="sxs-lookup"><span data-stu-id="437d3-116">accessLevel</span></span>               | <span data-ttu-id="437d3-117">String</span><span class="sxs-lookup"><span data-stu-id="437d3-117">String</span></span>                                                 | <span data-ttu-id="437d3-118">Die Zugriffsebene, die Zulassung der online-Besprechung steuert.</span><span class="sxs-lookup"><span data-stu-id="437d3-118">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="437d3-119">Mögliche Werte sind: `everyone`, `invited`, `locked`, `sameEnterprise` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="437d3-119">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="437d3-120">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="437d3-120">audioConferencing</span></span>         | [<span data-ttu-id="437d3-121">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="437d3-121">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="437d3-122">Stellt Access Telefoninformationen für einen OnlineMeeting.</span><span class="sxs-lookup"><span data-stu-id="437d3-122">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="437d3-123">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="437d3-123">canceledDateTime</span></span>          | <span data-ttu-id="437d3-124">DateTime</span><span class="sxs-lookup"><span data-stu-id="437d3-124">DateTime</span></span>                                               | <span data-ttu-id="437d3-125">Der Zeitpunkt, wann die Besprechung abgebrochen wurde.</span><span class="sxs-lookup"><span data-stu-id="437d3-125">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="437d3-126">chatInfo</span><span class="sxs-lookup"><span data-stu-id="437d3-126">chatInfo</span></span>                  | [<span data-ttu-id="437d3-127">chatInfo</span><span class="sxs-lookup"><span data-stu-id="437d3-127">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="437d3-128">Die Chat diese Besprechung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="437d3-128">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="437d3-129">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="437d3-129">creationDateTime</span></span>          | <span data-ttu-id="437d3-130">DateTime</span><span class="sxs-lookup"><span data-stu-id="437d3-130">DateTime</span></span>                                               | <span data-ttu-id="437d3-131">Die Uhrzeit der Erstellung die Besprechung.</span><span class="sxs-lookup"><span data-stu-id="437d3-131">The time when the meeting was created.</span></span> <span data-ttu-id="437d3-132">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="437d3-132">Readonly.</span></span>
| <span data-ttu-id="437d3-133">endDateTime</span><span class="sxs-lookup"><span data-stu-id="437d3-133">endDateTime</span></span>               | <span data-ttu-id="437d3-134">DateTime</span><span class="sxs-lookup"><span data-stu-id="437d3-134">DateTime</span></span>                                               | <span data-ttu-id="437d3-135">Die Endzeit der Besprechung.</span><span class="sxs-lookup"><span data-stu-id="437d3-135">End time of the meeting.</span></span> |
| <span data-ttu-id="437d3-136">entryExitAnnouncement</span><span class="sxs-lookup"><span data-stu-id="437d3-136">entryExitAnnouncement</span></span>     | <span data-ttu-id="437d3-137">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="437d3-137">Boolean</span></span>                                                | <span data-ttu-id="437d3-138">Der Anwesenheitsstatus des Ankündigungen für die onlinebesprechung.</span><span class="sxs-lookup"><span data-stu-id="437d3-138">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="437d3-139">Wenn die Anwesenheit Ankündigungen aktiviert sind, wird die online-Besprechung den Namen der Verknüpfung Participantswho die Besprechung per Audio-ankündigen.</span><span class="sxs-lookup"><span data-stu-id="437d3-139">When attendance announcements are enabled, the online meeting will announce the names of the participantswho join the meeting through audio.</span></span> |
| <span data-ttu-id="437d3-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="437d3-140">expirationDateTime</span></span>        | <span data-ttu-id="437d3-141">DateTime</span><span class="sxs-lookup"><span data-stu-id="437d3-141">DateTime</span></span>                                               | <span data-ttu-id="437d3-142">Absolute (Coordinated Universal Time, UTC) Datum und Uhrzeit nach dem kann die onlinebesprechung gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="437d3-142">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="437d3-143">Datum und Uhrzeit müssen zwischen ein Jahr vor und zehn Jahren nach dem das aktuelle Datum und die Uhrzeit auf dem Server sein.</span><span class="sxs-lookup"><span data-stu-id="437d3-143">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="437d3-144">id</span><span class="sxs-lookup"><span data-stu-id="437d3-144">id</span></span>                        | <span data-ttu-id="437d3-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="437d3-145">String</span></span>                                                 | <span data-ttu-id="437d3-146">Die ID der online-Besprechung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="437d3-146">The ID associated with the online meeting.</span></span> <span data-ttu-id="437d3-147">In einer HTTP GET-Anforderung verwendet wird, als ID zu.</span><span class="sxs-lookup"><span data-stu-id="437d3-147">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="437d3-148">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="437d3-148">Read-only.</span></span> <span data-ttu-id="437d3-149">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="437d3-149">Server generated.</span></span> |
| <span data-ttu-id="437d3-150">isCancelled</span><span class="sxs-lookup"><span data-stu-id="437d3-150">isCancelled</span></span>               | <span data-ttu-id="437d3-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="437d3-151">Boolean</span></span>                                                | <span data-ttu-id="437d3-152">Gibt an, ob die Besprechung abgebrochen wurde.</span><span class="sxs-lookup"><span data-stu-id="437d3-152">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="437d3-153">joinUrl</span><span class="sxs-lookup"><span data-stu-id="437d3-153">joinUrl</span></span>                   | <span data-ttu-id="437d3-154">String</span><span class="sxs-lookup"><span data-stu-id="437d3-154">String</span></span>                                                 | <span data-ttu-id="437d3-155">Die URL, die verwendet wird, wenn die onlinebesprechung aus dem Internet verbunden ist.</span><span class="sxs-lookup"><span data-stu-id="437d3-155">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="437d3-156">meetingType</span><span class="sxs-lookup"><span data-stu-id="437d3-156">meetingType</span></span>               | <span data-ttu-id="437d3-157">String</span><span class="sxs-lookup"><span data-stu-id="437d3-157">String</span></span>                                                 | <span data-ttu-id="437d3-158">Mögliche Werte sind: `meetNow`, `scheduled` und `recurring`.</span><span class="sxs-lookup"><span data-stu-id="437d3-158">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast`</span></span> |
| <span data-ttu-id="437d3-159">participants</span><span class="sxs-lookup"><span data-stu-id="437d3-159">participants</span></span>              | [<span data-ttu-id="437d3-160">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="437d3-160">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="437d3-161">Die Teilnehmer der Besprechung online zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="437d3-161">The participants associated with the online meeting.</span></span>  <span data-ttu-id="437d3-162">Dazu gehören der Organisator und die Teilnehmer.</span><span class="sxs-lookup"><span data-stu-id="437d3-162">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="437d3-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="437d3-163">startDateTime</span></span>             | <span data-ttu-id="437d3-164">DateTime</span><span class="sxs-lookup"><span data-stu-id="437d3-164">DateTime</span></span>                                               | <span data-ttu-id="437d3-165">Startzeit der Besprechung.</span><span class="sxs-lookup"><span data-stu-id="437d3-165">Start time of the meeting.</span></span> |
| <span data-ttu-id="437d3-166">subject</span><span class="sxs-lookup"><span data-stu-id="437d3-166">subject</span></span>                   | <span data-ttu-id="437d3-167">String</span><span class="sxs-lookup"><span data-stu-id="437d3-167">String</span></span>                                                 | <span data-ttu-id="437d3-168">Der Betreff der onlinebesprechung.</span><span class="sxs-lookup"><span data-stu-id="437d3-168">The subject of the online meeting.</span></span> |

## <a name="relationships"></a><span data-ttu-id="437d3-169">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="437d3-169">Relationships</span></span>
<span data-ttu-id="437d3-170">Keine</span><span class="sxs-lookup"><span data-stu-id="437d3-170">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="437d3-171">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="437d3-171">JSON representation</span></span>

<span data-ttu-id="437d3-172">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="437d3-172">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "accessLevel": "everyone | invited | locked | sameEnterprise",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "entryExitAnnouncement": true,
  "expirationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCancelled": false,
  "joinUrl": "String",
  "meetingType": "meetNow | scheduled | recurring | broadcast",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onlinemeeting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
