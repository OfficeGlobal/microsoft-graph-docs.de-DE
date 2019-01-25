---
title: Ressourcentyp bookingWorkHours
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9a51fb9d4f97dde2e3b50d9a19481eeab31483d1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527535"
---
# <a name="bookingworkhours-resource-type"></a><span data-ttu-id="d9cec-104">Ressourcentyp bookingWorkHours</span><span class="sxs-lookup"><span data-stu-id="d9cec-104">bookingWorkHours resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="d9cec-105">Repräsentiert den Satz der Arbeitsstunden an einem Tag der Woche, für eine [BookingBusiness](bookingbusiness.md) oder [BookingStaffMember](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="d9cec-105">Represents the set of working hours in a single day of the week, for a [bookingBusiness](bookingbusiness.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d9cec-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d9cec-106">Properties</span></span>
| <span data-ttu-id="d9cec-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d9cec-107">Property</span></span>     | <span data-ttu-id="d9cec-108">Typ</span><span class="sxs-lookup"><span data-stu-id="d9cec-108">Type</span></span>   |<span data-ttu-id="d9cec-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d9cec-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9cec-110">Tag</span><span class="sxs-lookup"><span data-stu-id="d9cec-110">day</span></span>|<span data-ttu-id="d9cec-111">String</span><span class="sxs-lookup"><span data-stu-id="d9cec-111">String</span></span>| <span data-ttu-id="d9cec-112">Von dieser Instanz dargestellten Wochentag.</span><span class="sxs-lookup"><span data-stu-id="d9cec-112">The day of the week represented by this instance.</span></span> <span data-ttu-id="d9cec-113">Mögliche Werte sind: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday` und `saturday`.</span><span class="sxs-lookup"><span data-stu-id="d9cec-113">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="d9cec-114">timeslots</span><span class="sxs-lookup"><span data-stu-id="d9cec-114">timeSlots</span></span>|<span data-ttu-id="d9cec-115">[BookingWorkTimeSlot](bookingworktimeslot.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d9cec-115">[bookingWorkTimeSlot](bookingworktimeslot.md) collection</span></span>|<span data-ttu-id="d9cec-116">Eine Liste der Anfangs-/Zeiten während eines Tages.</span><span class="sxs-lookup"><span data-stu-id="d9cec-116">A list of start/end times during a day.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d9cec-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d9cec-117">JSON representation</span></span>

<span data-ttu-id="d9cec-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d9cec-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkHours"
}-->

```json
{
  "day": "String",
  "timeSlots": [{"@odata.type": "microsoft.graph.bookingWorkTimeSlot"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingworkhours.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
