---
title: Ressourcentyp „attendeeAvailability“
description: Typ und Verfügbarkeit eines Teilnehmers
ms.openlocfilehash: 446dfb77d8f85021f41795038c3c1d597c6f1a6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016839"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="d5e15-103">Ressourcentyp „attendeeAvailability“</span><span class="sxs-lookup"><span data-stu-id="d5e15-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="d5e15-104">Typ und Verfügbarkeit eines Teilnehmers</span><span class="sxs-lookup"><span data-stu-id="d5e15-104">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5e15-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d5e15-105">JSON representation</span></span>

<span data-ttu-id="d5e15-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d5e15-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="d5e15-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d5e15-107">Properties</span></span>
| <span data-ttu-id="d5e15-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d5e15-108">Property</span></span>     | <span data-ttu-id="d5e15-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d5e15-109">Type</span></span>   |<span data-ttu-id="d5e15-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d5e15-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5e15-111">attendee</span><span class="sxs-lookup"><span data-stu-id="d5e15-111">attendee</span></span>|[<span data-ttu-id="d5e15-112">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="d5e15-112">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="d5e15-113">Der Typ des Teilnehmers. Unterschieden wird zwischen Personen und Ressourcen. Bei Personen wird zusätzlich differenziert zwischen erforderlichen und optionalen Teilnehmern.</span><span class="sxs-lookup"><span data-stu-id="d5e15-113">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="d5e15-114">availability</span><span class="sxs-lookup"><span data-stu-id="d5e15-114">availability</span></span>|<span data-ttu-id="d5e15-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="d5e15-115">freeBusyStatus</span></span>| <span data-ttu-id="d5e15-116">Der Verfügbarkeitsstatus des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="d5e15-116">The availability status of the attendee.</span></span> <span data-ttu-id="d5e15-117">Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d5e15-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
