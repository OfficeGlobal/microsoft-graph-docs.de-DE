---
title: Ressourcentyp bookingWorkHours
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: af606cf8ea867c040c20db3b4082761b3de69052
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958474"
---
# <a name="bookingworkhours-resource-type"></a><span data-ttu-id="f46a2-104">Ressourcentyp bookingWorkHours</span><span class="sxs-lookup"><span data-stu-id="f46a2-104">bookingWorkHours resource type</span></span>

 > <span data-ttu-id="f46a2-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f46a2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f46a2-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f46a2-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="f46a2-107">Repräsentiert den Satz der Arbeitsstunden an einem Tag der Woche, für eine [BookingBusiness](bookingbusiness.md) oder [BookingStaffMember](bookingstaffmember.md).</span><span class="sxs-lookup"><span data-stu-id="f46a2-107">Represents the set of working hours in a single day of the week, for a [bookingBusiness](bookingbusiness.md) or [bookingStaffMember](bookingstaffmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f46a2-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f46a2-108">Properties</span></span>
| <span data-ttu-id="f46a2-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f46a2-109">Property</span></span>     | <span data-ttu-id="f46a2-110">Typ</span><span class="sxs-lookup"><span data-stu-id="f46a2-110">Type</span></span>   |<span data-ttu-id="f46a2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f46a2-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f46a2-112">Tag</span><span class="sxs-lookup"><span data-stu-id="f46a2-112">day</span></span>|<span data-ttu-id="f46a2-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f46a2-113">String</span></span>| <span data-ttu-id="f46a2-114">Von dieser Instanz dargestellten Wochentag.</span><span class="sxs-lookup"><span data-stu-id="f46a2-114">The day of the week represented by this instance.</span></span> <span data-ttu-id="f46a2-115">Mögliche Werte sind: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday` und `saturday`.</span><span class="sxs-lookup"><span data-stu-id="f46a2-115">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="f46a2-116">Zeitabschnitte an</span><span class="sxs-lookup"><span data-stu-id="f46a2-116">timeSlots</span></span>|<span data-ttu-id="f46a2-117">[BookingWorkTimeSlot](bookingworktimeslot.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f46a2-117">[bookingWorkTimeSlot](bookingworktimeslot.md) collection</span></span>|<span data-ttu-id="f46a2-118">Eine Liste der Anfangs-/Zeiten während eines Tages.</span><span class="sxs-lookup"><span data-stu-id="f46a2-118">A list of start/end times during a day.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f46a2-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f46a2-119">JSON representation</span></span>

<span data-ttu-id="f46a2-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f46a2-120">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingWorkHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
