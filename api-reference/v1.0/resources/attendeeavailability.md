---
title: Ressourcentyp „attendeeAvailability“
description: Typ und Verfügbarkeit eines Teilnehmers
localization_priority: Normal
ms.openlocfilehash: a6dee994fc5eb3786fc1a432adcb9333bdb56ec8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834748"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="dafb6-103">Ressourcentyp „attendeeAvailability“</span><span class="sxs-lookup"><span data-stu-id="dafb6-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="dafb6-104">Typ und Verfügbarkeit eines Teilnehmers</span><span class="sxs-lookup"><span data-stu-id="dafb6-104">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dafb6-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dafb6-105">JSON representation</span></span>

<span data-ttu-id="dafb6-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dafb6-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="dafb6-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dafb6-107">Properties</span></span>
| <span data-ttu-id="dafb6-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dafb6-108">Property</span></span>     | <span data-ttu-id="dafb6-109">Typ</span><span class="sxs-lookup"><span data-stu-id="dafb6-109">Type</span></span>   |<span data-ttu-id="dafb6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dafb6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dafb6-111">attendee</span><span class="sxs-lookup"><span data-stu-id="dafb6-111">attendee</span></span>|[<span data-ttu-id="dafb6-112">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="dafb6-112">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="dafb6-113">Der Typ des Teilnehmers. Unterschieden wird zwischen Personen und Ressourcen. Bei Personen wird zusätzlich differenziert zwischen erforderlichen und optionalen Teilnehmern.</span><span class="sxs-lookup"><span data-stu-id="dafb6-113">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="dafb6-114">availability</span><span class="sxs-lookup"><span data-stu-id="dafb6-114">availability</span></span>|<span data-ttu-id="dafb6-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="dafb6-115">freeBusyStatus</span></span>| <span data-ttu-id="dafb6-116">Der Verfügbarkeitsstatus des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="dafb6-116">The availability status of the attendee.</span></span> <span data-ttu-id="dafb6-117">Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="dafb6-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
