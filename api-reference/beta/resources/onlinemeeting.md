---
title: Ressourcentyp onlineMeeting
description: Erfasst Informationen zu der Besprechung, einschließlich der Join-URL, die Teilnehmerliste und die Beschreibung an.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6bae6cf22e8790050f0b77ab903c5702354ea1f5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980398"
---
# <a name="onlinemeeting-resource-type"></a><span data-ttu-id="1f5d2-103">Ressourcentyp onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="1f5d2-103">onlineMeeting resource type</span></span>

> <span data-ttu-id="1f5d2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f5d2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f5d2-106">Erfasst Informationen zu der Besprechung, einschließlich der Join-URL, die Teilnehmerliste und die Beschreibung an.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-106">Captures information about the meeting, including the join URL, the attendees list, and the description.</span></span>

## <a name="methods"></a><span data-ttu-id="1f5d2-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="1f5d2-107">Methods</span></span>

| <span data-ttu-id="1f5d2-108">Methode</span><span class="sxs-lookup"><span data-stu-id="1f5d2-108">Method</span></span>         | <span data-ttu-id="1f5d2-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="1f5d2-109">Return Type</span></span> | <span data-ttu-id="1f5d2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f5d2-110">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="1f5d2-111">Abrufen von onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="1f5d2-111">Get onlineMeeting</span></span>](../api/onlinemeeting-get.md) | [<span data-ttu-id="1f5d2-112">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="1f5d2-112">onlineMeeting</span></span>](onlinemeeting.md) | <span data-ttu-id="1f5d2-113">Lesen Sie Eigenschaften und Beziehungen OnlineMeeting-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-113">Read properties and relationships of onlineMeeting object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1f5d2-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1f5d2-114">Properties</span></span>

| <span data-ttu-id="1f5d2-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1f5d2-115">Property</span></span>                  | <span data-ttu-id="1f5d2-116">Typ</span><span class="sxs-lookup"><span data-stu-id="1f5d2-116">Type</span></span>                                                   | <span data-ttu-id="1f5d2-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1f5d2-117">Description</span></span>                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1f5d2-118">accessLevel</span><span class="sxs-lookup"><span data-stu-id="1f5d2-118">accessLevel</span></span>               | <span data-ttu-id="1f5d2-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f5d2-119">String</span></span>                                                 | <span data-ttu-id="1f5d2-120">Die Zugriffsebene, die Zulassung der online-Besprechung steuert.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-120">The access level that controls admission to the online meeting.</span></span> <span data-ttu-id="1f5d2-121">Mögliche Werte sind: `everyone`, `invited`, `locked`, `sameEnterprise` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-121">Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`.</span></span> |
| <span data-ttu-id="1f5d2-122">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="1f5d2-122">audioConferencing</span></span>         | [<span data-ttu-id="1f5d2-123">audioConferencing</span><span class="sxs-lookup"><span data-stu-id="1f5d2-123">audioConferencing</span></span>](audioconferencing.md)              | <span data-ttu-id="1f5d2-124">Stellt Access Telefoninformationen für einen OnlineMeeting.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-124">Represents phone access information for an onlineMeeting.</span></span> |
| <span data-ttu-id="1f5d2-125">canceledDateTime</span><span class="sxs-lookup"><span data-stu-id="1f5d2-125">canceledDateTime</span></span>          | <span data-ttu-id="1f5d2-126">DateTime</span><span class="sxs-lookup"><span data-stu-id="1f5d2-126">DateTime</span></span>                                               | <span data-ttu-id="1f5d2-127">Der Zeitpunkt, wann die Besprechung abgebrochen wurde.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-127">The time when the meeting was canceled.</span></span> |
| <span data-ttu-id="1f5d2-128">chatInfo</span><span class="sxs-lookup"><span data-stu-id="1f5d2-128">chatInfo</span></span>                  | [<span data-ttu-id="1f5d2-129">chatInfo</span><span class="sxs-lookup"><span data-stu-id="1f5d2-129">chatInfo</span></span>](chatinfo.md)                                | <span data-ttu-id="1f5d2-130">Die Chat diese Besprechung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-130">The chat associated with this meeting.</span></span> |
| <span data-ttu-id="1f5d2-131">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="1f5d2-131">creationDateTime</span></span>          | <span data-ttu-id="1f5d2-132">DateTime</span><span class="sxs-lookup"><span data-stu-id="1f5d2-132">DateTime</span></span>                                               | <span data-ttu-id="1f5d2-133">Die Uhrzeit der Erstellung die Besprechung.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-133">The time when the meeting was created.</span></span> <span data-ttu-id="1f5d2-134">ReadOnly.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-134">Readonly.</span></span>
| <span data-ttu-id="1f5d2-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="1f5d2-135">endDateTime</span></span>               | <span data-ttu-id="1f5d2-136">DateTime</span><span class="sxs-lookup"><span data-stu-id="1f5d2-136">DateTime</span></span>                                               | <span data-ttu-id="1f5d2-137">Die Endzeit der Besprechung.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-137">End time of the meeting.</span></span> |
| <span data-ttu-id="1f5d2-138">entryExitAnnouncement</span><span class="sxs-lookup"><span data-stu-id="1f5d2-138">entryExitAnnouncement</span></span>     | <span data-ttu-id="1f5d2-139">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1f5d2-139">Boolean</span></span>                                                | <span data-ttu-id="1f5d2-140">Der Anwesenheitsstatus des Ankündigungen für die onlinebesprechung.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-140">The attendance announcements status for the online meeting.</span></span> <span data-ttu-id="1f5d2-141">Wenn die Anwesenheit Ankündigungen aktiviert sind, wird die online-Besprechung den Namen der Verknüpfung Participantswho die Besprechung per Audio-ankündigen.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-141">When attendance announcements are enabled, the online meeting will announce the names of the participantswho join the meeting through audio.</span></span> |
| <span data-ttu-id="1f5d2-142">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1f5d2-142">expirationDateTime</span></span>        | <span data-ttu-id="1f5d2-143">DateTime</span><span class="sxs-lookup"><span data-stu-id="1f5d2-143">DateTime</span></span>                                               | <span data-ttu-id="1f5d2-144">Absolute (Coordinated Universal Time, UTC) Datum und Uhrzeit nach dem kann die onlinebesprechung gelöscht werden.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-144">The absolute Coordinated Universal Time (UTC) date and time after which the online meeting can be deleted.</span></span> <span data-ttu-id="1f5d2-145">Datum und Uhrzeit müssen zwischen ein Jahr vor und zehn Jahren nach dem das aktuelle Datum und die Uhrzeit auf dem Server sein.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-145">The day and time must be between one year before, and ten years after, the current date and time on the server.</span></span> |
| <span data-ttu-id="1f5d2-146">id</span><span class="sxs-lookup"><span data-stu-id="1f5d2-146">id</span></span>                        | <span data-ttu-id="1f5d2-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f5d2-147">String</span></span>                                                 | <span data-ttu-id="1f5d2-148">Die ID der online-Besprechung zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-148">The ID associated with the online meeting.</span></span> <span data-ttu-id="1f5d2-149">In einer HTTP GET-Anforderung verwendet wird, als ID zu.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-149">Used in a GET HTTP request as the ID.</span></span> <span data-ttu-id="1f5d2-150">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-150">Read-only.</span></span> <span data-ttu-id="1f5d2-151">Server generiert wurde.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-151">Server generated.</span></span> |
| <span data-ttu-id="1f5d2-152">isCancelled</span><span class="sxs-lookup"><span data-stu-id="1f5d2-152">isCancelled</span></span>               | <span data-ttu-id="1f5d2-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f5d2-153">Boolean</span></span>                                                | <span data-ttu-id="1f5d2-154">Gibt an, ob die Besprechung abgebrochen wurde.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-154">Whether the meeting has been canceled.</span></span> |
| <span data-ttu-id="1f5d2-155">joinUrl</span><span class="sxs-lookup"><span data-stu-id="1f5d2-155">joinUrl</span></span>                   | <span data-ttu-id="1f5d2-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f5d2-156">String</span></span>                                                 | <span data-ttu-id="1f5d2-157">Die URL, die verwendet wird, wenn die onlinebesprechung aus dem Internet verbunden ist.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-157">The URL that is used when the online meeting is joined from the web.</span></span> |
| <span data-ttu-id="1f5d2-158">meetingType</span><span class="sxs-lookup"><span data-stu-id="1f5d2-158">meetingType</span></span>               | <span data-ttu-id="1f5d2-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f5d2-159">String</span></span>                                                 | <span data-ttu-id="1f5d2-160">Mögliche Werte sind: `meetNow`, `scheduled`, `recurring`,`broadcast`</span><span class="sxs-lookup"><span data-stu-id="1f5d2-160">Possible values are: `meetNow`, `scheduled`, `recurring`, `broadcast`</span></span> |
| <span data-ttu-id="1f5d2-161">participants</span><span class="sxs-lookup"><span data-stu-id="1f5d2-161">participants</span></span>              | [<span data-ttu-id="1f5d2-162">meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="1f5d2-162">meetingParticipants</span></span>](meetingparticipants.md)          | <span data-ttu-id="1f5d2-163">Die Teilnehmer der Besprechung online zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-163">The participants associated with the online meeting.</span></span>  <span data-ttu-id="1f5d2-164">Dazu gehören der Organisator und die Teilnehmer.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-164">This includes the organizer and the attendees.</span></span> |
| <span data-ttu-id="1f5d2-165">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1f5d2-165">startDateTime</span></span>             | <span data-ttu-id="1f5d2-166">DateTime</span><span class="sxs-lookup"><span data-stu-id="1f5d2-166">DateTime</span></span>                                               | <span data-ttu-id="1f5d2-167">Startzeit der Besprechung.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-167">Start time of the meeting.</span></span> |
| <span data-ttu-id="1f5d2-168">Betreff</span><span class="sxs-lookup"><span data-stu-id="1f5d2-168">subject</span></span>                   | <span data-ttu-id="1f5d2-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1f5d2-169">String</span></span>                                                 | <span data-ttu-id="1f5d2-170">Der Betreff der onlinebesprechung.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-170">The subject of the online meeting.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1f5d2-171">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1f5d2-171">Relationships</span></span>
<span data-ttu-id="1f5d2-172">Keine</span><span class="sxs-lookup"><span data-stu-id="1f5d2-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f5d2-173">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1f5d2-173">JSON representation</span></span>

<span data-ttu-id="1f5d2-174">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1f5d2-174">The following is a JSON representation of the resource.</span></span>

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
