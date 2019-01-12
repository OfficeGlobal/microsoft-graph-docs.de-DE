---
title: Ressourcentyp bookingWorkTimeSlot
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 33dd856d678d2cf1ba9da2a747c0bd46f2fd4932
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968484"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="e5702-104">Ressourcentyp bookingWorkTimeSlot</span><span class="sxs-lookup"><span data-stu-id="e5702-104">bookingWorkTimeSlot resource type</span></span>

 > <span data-ttu-id="e5702-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e5702-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5702-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e5702-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="e5702-107">Die Anfangs- und Endzeiten für die Arbeit.</span><span class="sxs-lookup"><span data-stu-id="e5702-107">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="e5702-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e5702-108">Properties</span></span>
| <span data-ttu-id="e5702-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e5702-109">Property</span></span>     | <span data-ttu-id="e5702-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e5702-110">Type</span></span>   |<span data-ttu-id="e5702-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e5702-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5702-112">end</span><span class="sxs-lookup"><span data-stu-id="e5702-112">end</span></span>|<span data-ttu-id="e5702-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e5702-113">TimeOfDay</span></span>|<span data-ttu-id="e5702-114">Die Tageszeit arbeiten beginnt.</span><span class="sxs-lookup"><span data-stu-id="e5702-114">The time of the day that work starts.</span></span> <span data-ttu-id="e5702-115">Beispielsweise 08:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="e5702-115">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="e5702-116">start</span><span class="sxs-lookup"><span data-stu-id="e5702-116">start</span></span>|<span data-ttu-id="e5702-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e5702-117">TimeOfDay</span></span>|<span data-ttu-id="e5702-118">Die Tageszeit arbeiten wird beendet.</span><span class="sxs-lookup"><span data-stu-id="e5702-118">The time of the day that work stops.</span></span> <span data-ttu-id="e5702-119">Beispielsweise 17:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="e5702-119">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5702-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e5702-120">JSON representation</span></span>

<span data-ttu-id="e5702-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e5702-121">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "bookingWorkTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
