---
title: Ressourcentyp meetingParticipants
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 4f91c9198018e903eccff7e8fe07d6668d9fd2c9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065714"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="b21b4-103">Ressourcentyp meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="b21b4-103">meetingParticipants resource type</span></span>

> <span data-ttu-id="b21b4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b21b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b21b4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b21b4-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="b21b4-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b21b4-106">Properties</span></span>

| <span data-ttu-id="b21b4-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b21b4-107">Property</span></span>       | <span data-ttu-id="b21b4-108">Typ</span><span class="sxs-lookup"><span data-stu-id="b21b4-108">Type</span></span>    | <span data-ttu-id="b21b4-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b21b4-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b21b4-110">attendees</span><span class="sxs-lookup"><span data-stu-id="b21b4-110">attendees</span></span> | <span data-ttu-id="b21b4-111">[MeetingParticipantInfo](meetingparticipantinfo.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b21b4-111">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="b21b4-112">organizer</span><span class="sxs-lookup"><span data-stu-id="b21b4-112">organizer</span></span> | [<span data-ttu-id="b21b4-113">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="b21b4-113">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="b21b4-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b21b4-114">JSON representation</span></span>

<span data-ttu-id="b21b4-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b21b4-115">The following is a JSON representation of the resource.</span></span>

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
