---
title: Ressourcentyp „attendeeAvailability“
description: Typ und Verfügbarkeit eines Teilnehmers
localization_priority: Normal
ms.openlocfilehash: 37b344f110557d6e04129a2b93592009635bddcf
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576283"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="2443d-103">Ressourcentyp „attendeeAvailability“</span><span class="sxs-lookup"><span data-stu-id="2443d-103">attendeeAvailability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2443d-104">Typ und Verfügbarkeit eines Teilnehmers</span><span class="sxs-lookup"><span data-stu-id="2443d-104">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2443d-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2443d-105">JSON representation</span></span>

<span data-ttu-id="2443d-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2443d-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="2443d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2443d-107">Properties</span></span>
| <span data-ttu-id="2443d-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2443d-108">Property</span></span>     | <span data-ttu-id="2443d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2443d-109">Type</span></span>   |<span data-ttu-id="2443d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2443d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2443d-111">attendee</span><span class="sxs-lookup"><span data-stu-id="2443d-111">attendee</span></span>|[<span data-ttu-id="2443d-112">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="2443d-112">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="2443d-113">Der Typ des Teilnehmers. Unterschieden wird zwischen Personen und Ressourcen. Bei Personen wird zusätzlich differenziert zwischen erforderlichen und optionalen Teilnehmern.</span><span class="sxs-lookup"><span data-stu-id="2443d-113">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="2443d-114">availability</span><span class="sxs-lookup"><span data-stu-id="2443d-114">availability</span></span>|<span data-ttu-id="2443d-115">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="2443d-115">freeBusyStatus</span></span>| <span data-ttu-id="2443d-116">Der Verfügbarkeitsstatus des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="2443d-116">The availability status of the attendee.</span></span> <span data-ttu-id="2443d-117">Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="2443d-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendeeavailability.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
