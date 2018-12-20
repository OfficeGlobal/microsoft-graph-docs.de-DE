---
title: Ressourcentyp meetingParticipants
description: Teilnehmer an einer Besprechung.
author: VinodRavichandran
ms.openlocfilehash: 7e44863004dab5405251e2effaf2af8c2ae31f67
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380282"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="ec6c4-103">Ressourcentyp meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="ec6c4-103">meetingParticipants resource type</span></span>

> <span data-ttu-id="ec6c4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ec6c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec6c4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ec6c4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec6c4-106">Teilnehmer an einer Besprechung.</span><span class="sxs-lookup"><span data-stu-id="ec6c4-106">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="ec6c4-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ec6c4-107">Properties</span></span>

| <span data-ttu-id="ec6c4-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ec6c4-108">Property</span></span>       | <span data-ttu-id="ec6c4-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ec6c4-109">Type</span></span>    | <span data-ttu-id="ec6c4-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec6c4-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ec6c4-111">attendees</span><span class="sxs-lookup"><span data-stu-id="ec6c4-111">attendees</span></span> | <span data-ttu-id="ec6c4-112">[MeetingParticipantInfo](meetingparticipantinfo.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="ec6c4-112">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="ec6c4-113">organizer</span><span class="sxs-lookup"><span data-stu-id="ec6c4-113">organizer</span></span> | [<span data-ttu-id="ec6c4-114">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="ec6c4-114">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="ec6c4-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ec6c4-115">JSON representation</span></span>

<span data-ttu-id="ec6c4-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ec6c4-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipants"
}-->
```json
{
  "attendees": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingParticipants resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
