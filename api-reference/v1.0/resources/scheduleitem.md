---
title: scheduleItem-Ressourcentyp
description: Ein Element, das die Verfügbarkeit eines Benutzers beschreibt, der einem tatsächlichen Ereignis im Standardkalender des Benutzers entspricht. Dieses Element gilt auch für eine Ressource (Raum oder Gerät).
localization_priority: Normal
ms.openlocfilehash: 8a30dcb4394a963e35047fab00391f0cc7eb7715
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30926603"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="61bc1-104">scheduleItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="61bc1-104">scheduleItem resource type</span></span>

<span data-ttu-id="61bc1-105">Ein Element, das die Verfügbarkeit eines Benutzers beschreibt, der einem tatsächlichen Ereignis im Standardkalender des Benutzers entspricht.</span><span class="sxs-lookup"><span data-stu-id="61bc1-105">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="61bc1-106">Dieses Element gilt auch für eine Ressource (Raum oder Gerät).</span><span class="sxs-lookup"><span data-stu-id="61bc1-106">This item applies to a resource (room or equipment) as well.</span></span>

## <a name="properties"></a><span data-ttu-id="61bc1-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="61bc1-107">Properties</span></span>
| <span data-ttu-id="61bc1-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61bc1-108">Property</span></span>     | <span data-ttu-id="61bc1-109">Typ</span><span class="sxs-lookup"><span data-stu-id="61bc1-109">Type</span></span>   |<span data-ttu-id="61bc1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61bc1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="61bc1-111">end</span><span class="sxs-lookup"><span data-stu-id="61bc1-111">end</span></span> |[<span data-ttu-id="61bc1-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="61bc1-112">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="61bc1-113">Das Datum, die Uhrzeit und die Zeitzone, die das entsprechende Ereignis beendet.</span><span class="sxs-lookup"><span data-stu-id="61bc1-113">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="61bc1-114">isPrivate</span><span class="sxs-lookup"><span data-stu-id="61bc1-114">isPrivate</span></span> |<span data-ttu-id="61bc1-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="61bc1-115">Boolean</span></span> |<span data-ttu-id="61bc1-116">Die Vertraulichkeit des entsprechenden Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="61bc1-116">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="61bc1-117">True, wenn das Ereignis markiert `private`ist, andernfalls false.</span><span class="sxs-lookup"><span data-stu-id="61bc1-117">True if the event is marked `private`, false otherwise.</span></span> <span data-ttu-id="61bc1-118">Optional.</span><span class="sxs-lookup"><span data-stu-id="61bc1-118">Optional.</span></span>|
|<span data-ttu-id="61bc1-119">location</span><span class="sxs-lookup"><span data-stu-id="61bc1-119">location</span></span> |<span data-ttu-id="61bc1-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="61bc1-120">String</span></span> | <span data-ttu-id="61bc1-121">Der Ort, an dem das entsprechende Ereignis gehalten oder besucht wird.</span><span class="sxs-lookup"><span data-stu-id="61bc1-121">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="61bc1-122">Optional.</span><span class="sxs-lookup"><span data-stu-id="61bc1-122">Optional.</span></span>|
|<span data-ttu-id="61bc1-123">start</span><span class="sxs-lookup"><span data-stu-id="61bc1-123">start</span></span> |[<span data-ttu-id="61bc1-124">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="61bc1-124">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="61bc1-125">Das Datum, die Uhrzeit und die Zeitzone, die das entsprechende Ereignis startet.</span><span class="sxs-lookup"><span data-stu-id="61bc1-125">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="61bc1-126">status</span><span class="sxs-lookup"><span data-stu-id="61bc1-126">status</span></span> |<span data-ttu-id="61bc1-127">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="61bc1-127">freeBusyStatus</span></span> | <span data-ttu-id="61bc1-128">Der Verfügbarkeitsstatus des Benutzers oder der Ressource während des entsprechenden Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="61bc1-128">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="61bc1-129">Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="61bc1-129">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="61bc1-130">subject</span><span class="sxs-lookup"><span data-stu-id="61bc1-130">subject</span></span> |<span data-ttu-id="61bc1-131">String</span><span class="sxs-lookup"><span data-stu-id="61bc1-131">String</span></span> | <span data-ttu-id="61bc1-132">Die Betreffzeile des entsprechenden Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="61bc1-132">The corresponding event's subject line.</span></span> <span data-ttu-id="61bc1-133">Optional.</span><span class="sxs-lookup"><span data-stu-id="61bc1-133">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="61bc1-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="61bc1-134">JSON representation</span></span>

<span data-ttu-id="61bc1-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="61bc1-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "isPrivate",
    "location",
    "subject"
  ],
  "@odata.type": "microsoft.graph.scheduleItem"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "isPrivate": true,
  "location": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
