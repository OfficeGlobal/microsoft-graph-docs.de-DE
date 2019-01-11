---
title: Ressourcentyp bookingWorkTimeSlot
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 69a802e4addd3c0cb821a630707a62724ea984a2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839557"
---
# <a name="bookingworktimeslot-resource-type"></a><span data-ttu-id="12327-104">Ressourcentyp bookingWorkTimeSlot</span><span class="sxs-lookup"><span data-stu-id="12327-104">bookingWorkTimeSlot resource type</span></span>

 > <span data-ttu-id="12327-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="12327-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12327-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="12327-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="12327-107">Die Anfangs- und Endzeiten für die Arbeit.</span><span class="sxs-lookup"><span data-stu-id="12327-107">The start and end times for work.</span></span>


## <a name="properties"></a><span data-ttu-id="12327-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="12327-108">Properties</span></span>
| <span data-ttu-id="12327-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="12327-109">Property</span></span>     | <span data-ttu-id="12327-110">Typ</span><span class="sxs-lookup"><span data-stu-id="12327-110">Type</span></span>   |<span data-ttu-id="12327-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12327-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12327-112">end</span><span class="sxs-lookup"><span data-stu-id="12327-112">end</span></span>|<span data-ttu-id="12327-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="12327-113">TimeOfDay</span></span>|<span data-ttu-id="12327-114">Die Tageszeit arbeiten beginnt.</span><span class="sxs-lookup"><span data-stu-id="12327-114">The time of the day that work starts.</span></span> <span data-ttu-id="12327-115">Beispielsweise 08:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="12327-115">For example, 08:00:00.0000000.</span></span>|
|<span data-ttu-id="12327-116">start</span><span class="sxs-lookup"><span data-stu-id="12327-116">start</span></span>|<span data-ttu-id="12327-117">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="12327-117">TimeOfDay</span></span>|<span data-ttu-id="12327-118">Die Tageszeit arbeiten wird beendet.</span><span class="sxs-lookup"><span data-stu-id="12327-118">The time of the day that work stops.</span></span> <span data-ttu-id="12327-119">Beispielsweise 17:00:00.0000000.</span><span class="sxs-lookup"><span data-stu-id="12327-119">For example, 17:00:00.0000000.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12327-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="12327-120">JSON representation</span></span>

<span data-ttu-id="12327-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="12327-121">The following is a JSON representation of the resource.</span></span>

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
