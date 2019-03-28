---
title: Ressourcentyp „timeSlot“
description: Ein Zeitfenster
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7b09ae7f1c60a8348e9f22b856c65f326432e408
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936241"
---
# <a name="timeslot-resource-type"></a><span data-ttu-id="646b2-103">Ressourcentyp „timeSlot“</span><span class="sxs-lookup"><span data-stu-id="646b2-103">timeSlot resource type</span></span>

<span data-ttu-id="646b2-104">Stellt ein Zeitfenster für eine Besprechung dar.</span><span class="sxs-lookup"><span data-stu-id="646b2-104">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="646b2-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="646b2-105">JSON representation</span></span>

<span data-ttu-id="646b2-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="646b2-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="646b2-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="646b2-107">Properties</span></span>
| <span data-ttu-id="646b2-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="646b2-108">Property</span></span>     | <span data-ttu-id="646b2-109">Typ</span><span class="sxs-lookup"><span data-stu-id="646b2-109">Type</span></span>   |<span data-ttu-id="646b2-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="646b2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="646b2-111">end</span><span class="sxs-lookup"><span data-stu-id="646b2-111">end</span></span>|[<span data-ttu-id="646b2-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="646b2-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="646b2-113">Das Datum, die Uhrzeit und die Zeitzone, an denen ein Punkt beginnt.</span><span class="sxs-lookup"><span data-stu-id="646b2-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="646b2-114">start</span><span class="sxs-lookup"><span data-stu-id="646b2-114">start</span></span>|[<span data-ttu-id="646b2-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="646b2-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="646b2-116">Das Datum, die Uhrzeit und die Zeitzone, die ein Punkt endet.</span><span class="sxs-lookup"><span data-stu-id="646b2-116">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
