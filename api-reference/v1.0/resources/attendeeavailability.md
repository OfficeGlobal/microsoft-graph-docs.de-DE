---
title: Ressourcentyp „attendeeAvailability“
description: Die Verfügbarkeit eines Teilnehmers.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 63014553824b833e2e4cdfb03485fcb7962c01a0
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936248"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="d3c7f-103">Ressourcentyp „attendeeAvailability“</span><span class="sxs-lookup"><span data-stu-id="d3c7f-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="d3c7f-104">Die Verfügbarkeit eines Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="d3c7f-104">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3c7f-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d3c7f-105">JSON representation</span></span>

<span data-ttu-id="d3c7f-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d3c7f-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="d3c7f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d3c7f-107">Properties</span></span>
| <span data-ttu-id="d3c7f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d3c7f-108">Property</span></span>     | <span data-ttu-id="d3c7f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d3c7f-109">Type</span></span>   |<span data-ttu-id="d3c7f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3c7f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3c7f-111">attendee</span><span class="sxs-lookup"><span data-stu-id="d3c7f-111">attendee</span></span>|[<span data-ttu-id="d3c7f-112">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="d3c7f-112">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="d3c7f-113">Die e-Mail-Adresse und den Typ des Teilnehmers – unabhängig davon, ob es sich um eine Person oder eine Ressource handelt, und ob Sie erforderlich oder optional ist, wenn es sich um eine Person handelt</span><span class="sxs-lookup"><span data-stu-id="d3c7f-113">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="d3c7f-114">availability</span><span class="sxs-lookup"><span data-stu-id="d3c7f-114">availability</span></span>|<span data-ttu-id="d3c7f-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="d3c7f-115">freeBusyStatus</span></span>| <span data-ttu-id="d3c7f-116">Der Verfügbarkeitsstatus des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="d3c7f-116">The availability status of the attendee.</span></span> <span data-ttu-id="d3c7f-117">Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d3c7f-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
