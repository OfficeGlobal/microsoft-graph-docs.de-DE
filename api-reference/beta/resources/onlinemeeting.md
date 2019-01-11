---
title: Ressourcentyp onlineMeeting
description: Erfasst Informationen zu der Besprechung, einschließlich der Join-URL, die Teilnehmerliste und die Beschreibung an.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: b1a0b09c0e7c792b0a9662c08daecd212c027c89
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805159"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="8ed34-103">Ressourcentyp onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="8ed34-103">onlineMeeting resource type</span></span>

> <span data-ttu-id="8ed34-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8ed34-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ed34-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8ed34-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ed34-106">Erfasst Informationen zu der Besprechung, einschließlich der Join-URL, die Teilnehmerliste und die Beschreibung an.</span><span class="sxs-lookup"><span data-stu-id="8ed34-106">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="8ed34-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="8ed34-107">Methods</span></span>

| <span data-ttu-id="8ed34-108">Methode</span><span class="sxs-lookup"><span data-stu-id="8ed34-108">Method</span></span>         | <span data-ttu-id="8ed34-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8ed34-109">Return Type</span></span> | <span data-ttu-id="8ed34-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ed34-110">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="8ed34-111">Abrufen von onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="8ed34-111">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="8ed34-112">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="8ed34-112">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="8ed34-113">Lesen Sie Eigenschaften und Beziehungen OnlineMeeting-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8ed34-113">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8ed34-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8ed34-114">Properties</span></span>

| <span data-ttu-id="8ed34-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8ed34-115">Property</span></span>                  | <span data-ttu-id="8ed34-116">Typ</span><span class="sxs-lookup"><span data-stu-id="8ed34-116">Type</span></span>                                                   | <span data-ttu-id="8ed34-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ed34-117">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8ed34-118">accessLevel</span><span class="sxs-lookup"><span data-stu-id="8ed34-118">accessLevel</span></span>               | <span data-ttu-id="8ed34-119">String</span><span class="sxs-lookup"><span data-stu-id="8ed34-119">String</span></span>                                                 | <span data-ttu-id="8ed34-120">Die Zugriffsebene, die Zulassung der online-Besprechung steuert.</span><span class="sxs-lookup"><span data-stu-id="8ed34-120">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="8ed34-121">Mögliche Werte sind: `everyone`, `invited`, `locked`, `sameEnterprise` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="8ed34-121">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="8ed34-122">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="8ed34-122">audioConferencing</span></span>         | [<span data-ttu-id="8ed34-123">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="8ed34-123">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="8ed34-124">Stellt Access Telefoninformationen für einen OnlineMeeting.</span><span class="sxs-lookup"><span data-stu-id="8ed34-124">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="8ed34-125">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="8ed34-125">canceledDateTime</span></span>          | <span data-ttu-id="8ed34-126">DateTime</span><span class="sxs-lookup"><span data-stu-id="8ed34-126">DateTime</span></span>                                               | <span data-ttu-id="8ed34-127">Der Zeitpunkt, wann die Besprechung abgebrochen wurde.</span><span class="sxs-lookup"><span data-stu-id="8ed34-127">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="8ed34-128">chatInfo</span><span class="sxs-lookup"><span data-stu-id="8ed34-128">chatInfo</span></span>                  | [<span data-ttu-id="8ed34-129">chatInfo</span><span class="sxs-lookup"><span data-stu-id="8ed34-129">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="8ed34-130">Die Chat diese Besprechung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="8ed34-130">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="8ed34-131">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="8ed34-131">creationDateTime</span></span>          | <span data-ttu-id="8ed34-132">DateTime</span><span class="sxs-lookup"><span data-stu-id="8ed34-132">DateTime</span></span>                                               | <span data-ttu-id="8ed34-133">Die Uhrzeit der Erstellung die Besprechung.</span><span class="sxs-lookup"><span data-stu-id="8ed34-133">The time when the meeting was created.</span></span> <span data-ttu-id="8ed34-134">ReadOnly.</span><span class="sxs-lookup"><span data-stu-id="8ed34-134">Readonly.</span></span>
| <span data-ttu-id="8ed34-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="8ed34-135">endDateTime</span></span>               | <span data-ttu-id="8ed34-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="8ed34-136">DateTime</span></span>                                               | <span data-ttu-id="8ed34-137">Die Endzeit der Besprechung.</span><span class="sxs-lookup"><span data-stu-id="8ed34-137">End time of the meeting.</span></span> |
| <span data-ttu-id="8ed34-138">entryExitAnnouncement</span><span class="sxs-lookup"><span data-stu-id="8ed34-138">entryExitAnnouncement</span></span>     | <span data-ttu-id="8ed34-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ed34-139">Boolean</span></span>                                                | <span data-ttu-id="8ed34-140">Der Anwesenheitsstatus des Ankündigungen für die onlinebesprechung.</span><span class="sxs-lookup"><span data-stu-id="8ed34-140">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="8ed34-141">Wenn die Anwesenheit Ankündigungen aktiviert sind, wird die online-Besprechung den Namen der Verknüpfung Participantswho die Besprechung per Audio-ankündigen.</span><span class="sxs-lookup"><span data-stu-id="8ed34-141">When attendance announcements are enabled, the online meeting will announce the names of the participantswho join the meeting through audio.</span></span> |
| <span data-ttu-id="8ed34-142">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8ed34-142">expirationDateTime</span></span>        | <span data-ttu-id="8ed34-143">DateTime</span><span class="sxs-lookup"><span data-stu-id="8ed34-143">DateTime</span></span>                                               | <span data-ttu-id="8ed34-144">Absolute (Coordinated Universal Time, UTC) Datum und Uhrzeit nach dem kann die onlinebesprechung gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="8ed34-144">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="8ed34-145">Datum und Uhrzeit müssen zwischen ein Jahr vor und zehn Jahren nach dem das aktuelle Datum und die Uhrzeit auf dem Server sein.</span><span class="sxs-lookup"><span data-stu-id="8ed34-145">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="8ed34-146">id</span><span class="sxs-lookup"><span data-stu-id="8ed34-146">id</span></span>                        | <span data-ttu-id="8ed34-147">String</span><span class="sxs-lookup"><span data-stu-id="8ed34-147">String</span></span>                                                 | <span data-ttu-id="8ed34-148">Die ID der online-Besprechung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="8ed34-148">The ID associated with the online meeting.</span></span> <span data-ttu-id="8ed34-149">In einer HTTP GET-Anforderung verwendet wird, als ID zu.</span><span class="sxs-lookup"><span data-stu-id="8ed34-149">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="8ed34-150">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8ed34-150">Read-only.</span></span> <span data-ttu-id="8ed34-151">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="8ed34-151">Server generated.</span></span> |
| <span data-ttu-id="8ed34-152">isCancelled</span><span class="sxs-lookup"><span data-stu-id="8ed34-152">isCancelled</span></span>               | <span data-ttu-id="8ed34-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ed34-153">Boolean</span></span>                                                | <span data-ttu-id="8ed34-154">Gibt an, ob die Besprechung abgebrochen wurde.</span><span class="sxs-lookup"><span data-stu-id="8ed34-154">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="8ed34-155">joinUrl</span><span class="sxs-lookup"><span data-stu-id="8ed34-155">joinUrl</span></span>                   | <span data-ttu-id="8ed34-156">String</span><span class="sxs-lookup"><span data-stu-id="8ed34-156">String</span></span>                                                 | <span data-ttu-id="8ed34-157">Die URL, die verwendet wird, wenn die onlinebesprechung aus dem Internet verbunden ist.</span><span class="sxs-lookup"><span data-stu-id="8ed34-157">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="8ed34-158">meetingType</span><span class="sxs-lookup"><span data-stu-id="8ed34-158">meetingType</span></span>               | <span data-ttu-id="8ed34-159">String</span><span class="sxs-lookup"><span data-stu-id="8ed34-159">String</span></span>                                                 | <span data-ttu-id="8ed34-160">Mögliche Werte sind: `meetNow`, `scheduled`, `recurring`,`broadcast`</span><span class="sxs-lookup"><span data-stu-id="8ed34-160">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast`</span></span> |
| <span data-ttu-id="8ed34-161">participants</span><span class="sxs-lookup"><span data-stu-id="8ed34-161">participants</span></span>              | [<span data-ttu-id="8ed34-162">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="8ed34-162">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="8ed34-163">Die Teilnehmer der Besprechung online zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="8ed34-163">The participants associated with the online meeting.</span></span>  <span data-ttu-id="8ed34-164">Dazu gehören der Organisator und die Teilnehmer.</span><span class="sxs-lookup"><span data-stu-id="8ed34-164">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="8ed34-165">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8ed34-165">startDateTime</span></span>             | <span data-ttu-id="8ed34-166">DateTime</span><span class="sxs-lookup"><span data-stu-id="8ed34-166">DateTime</span></span>                                               | <span data-ttu-id="8ed34-167">Startzeit der Besprechung.</span><span class="sxs-lookup"><span data-stu-id="8ed34-167">Start time of the meeting.</span></span> |
| <span data-ttu-id="8ed34-168">Betreff</span><span class="sxs-lookup"><span data-stu-id="8ed34-168">subject</span></span>                   | <span data-ttu-id="8ed34-169">String</span><span class="sxs-lookup"><span data-stu-id="8ed34-169">String</span></span>                                                 | <span data-ttu-id="8ed34-170">Der Betreff der onlinebesprechung.</span><span class="sxs-lookup"><span data-stu-id="8ed34-170">The subject of the online meeting.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8ed34-171">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8ed34-171">Relationships</span></span>
<span data-ttu-id="8ed34-172">Keine</span><span class="sxs-lookup"><span data-stu-id="8ed34-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ed34-173">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8ed34-173">JSON representation</span></span>

<span data-ttu-id="8ed34-174">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8ed34-174">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
