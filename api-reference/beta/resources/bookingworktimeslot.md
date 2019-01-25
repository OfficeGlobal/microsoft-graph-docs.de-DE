---
title: Ressourcentyp bookingWorkTimeSlot
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a193843617d5acc7e18d8a06993a1629b80762be
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513788"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="2258f-104">Ressourcentyp bookingWorkTimeSlot</span><span class="sxs-lookup"><span data-stu-id="2258f-104">bookingWorkTimeSlot resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="2258f-105">Die Anfangs- und Endzeiten für die Arbeit.</span><span class="sxs-lookup"><span data-stu-id="2258f-105">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="2258f-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2258f-106">Properties</span></span>
| <span data-ttu-id="2258f-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2258f-107">Property</span></span>     | <span data-ttu-id="2258f-108">Typ</span><span class="sxs-lookup"><span data-stu-id="2258f-108">Type</span></span>   |<span data-ttu-id="2258f-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2258f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2258f-110">end</span><span class="sxs-lookup"><span data-stu-id="2258f-110">end</span></span>|<span data-ttu-id="2258f-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2258f-111">TimeOfDay</span></span>|<span data-ttu-id="2258f-112">Die Tageszeit arbeiten beginnt.</span><span class="sxs-lookup"><span data-stu-id="2258f-112">The time of the day that work starts.</span></span> <span data-ttu-id="2258f-113">Beispielsweise 08:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="2258f-113">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="2258f-114">start</span><span class="sxs-lookup"><span data-stu-id="2258f-114">start</span></span>|<span data-ttu-id="2258f-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2258f-115">TimeOfDay</span></span>|<span data-ttu-id="2258f-116">Die Tageszeit arbeiten wird beendet.</span><span class="sxs-lookup"><span data-stu-id="2258f-116">The time of the day that work stops.</span></span> <span data-ttu-id="2258f-117">Beispielsweise 17:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="2258f-117">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2258f-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2258f-118">JSON representation</span></span>

<span data-ttu-id="2258f-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2258f-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkTimeSlot"
}-->

```json
{
  "end": "String (timestamp)",
  "start": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingworktimeslot.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
