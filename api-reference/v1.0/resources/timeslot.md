---
title: Ressourcentyp „timeSlot“
description: Ein Zeitfenster
ms.openlocfilehash: 43ce20e006f2a6946877a4ffd2bf730d45d6d1c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018026"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="ed3ba-103">Ressourcentyp „timeSlot“</span><span class="sxs-lookup"><span data-stu-id="ed3ba-103">timeSlot resource type</span></span>

<span data-ttu-id="ed3ba-104">Ein Zeitfenster</span><span class="sxs-lookup"><span data-stu-id="ed3ba-104">A time period.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed3ba-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ed3ba-105">JSON representation</span></span>

<span data-ttu-id="ed3ba-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ed3ba-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeSlot"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a><span data-ttu-id="ed3ba-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ed3ba-107">Properties</span></span>
| <span data-ttu-id="ed3ba-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ed3ba-108">Property</span></span>     | <span data-ttu-id="ed3ba-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ed3ba-109">Type</span></span>   |<span data-ttu-id="ed3ba-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed3ba-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed3ba-111">end</span><span class="sxs-lookup"><span data-stu-id="ed3ba-111">end</span></span>|[<span data-ttu-id="ed3ba-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ed3ba-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="ed3ba-113">Die Startzeit des betreffenden Zeitfensters</span><span class="sxs-lookup"><span data-stu-id="ed3ba-113">The time a period begins.</span></span>|
|<span data-ttu-id="ed3ba-114">start</span><span class="sxs-lookup"><span data-stu-id="ed3ba-114">start</span></span>|[<span data-ttu-id="ed3ba-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="ed3ba-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="ed3ba-116">Die Endzeit des betreffenden Zeitfensters</span><span class="sxs-lookup"><span data-stu-id="ed3ba-116">The time the period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->