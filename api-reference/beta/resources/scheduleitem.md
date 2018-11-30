---
title: von ScheduleItem Ressourcentyp
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: a7a31f47cde92549a72299b22a40b10c6f7845c6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063538"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="31300-104">von ScheduleItem Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="31300-104">scheduleItem resource type</span></span>

 > <span data-ttu-id="31300-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="31300-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31300-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="31300-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="31300-107">Ein Element, das beschreibt die Verfügbarkeit eines Benutzers auf ein Ereignis tatsächliche auf Standardkalender des Benutzers entspricht.</span><span class="sxs-lookup"><span data-stu-id="31300-107">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="31300-108">Dieses Element gilt für als auch eine Ressource.</span><span class="sxs-lookup"><span data-stu-id="31300-108">This item applies to a resource as well.</span></span>

## <a name="properties"></a><span data-ttu-id="31300-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="31300-109">Properties</span></span>
| <span data-ttu-id="31300-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="31300-110">Property</span></span>     | <span data-ttu-id="31300-111">Typ</span><span class="sxs-lookup"><span data-stu-id="31300-111">Type</span></span>   |<span data-ttu-id="31300-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31300-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31300-113">end</span><span class="sxs-lookup"><span data-stu-id="31300-113">end</span></span> |[<span data-ttu-id="31300-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="31300-114">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="31300-115">Das Datum, Uhrzeit und Zeitzone, die das zugehörige Ereignis endet.</span><span class="sxs-lookup"><span data-stu-id="31300-115">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="31300-116">isPrivate</span><span class="sxs-lookup"><span data-stu-id="31300-116">isPrivate</span></span> |<span data-ttu-id="31300-117">Boolesch</span><span class="sxs-lookup"><span data-stu-id="31300-117">Boolean</span></span> |<span data-ttu-id="31300-118">Die Vertraulichkeit des entsprechenden Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="31300-118">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="31300-119">True, wenn das Ereignis markiert wird `private`false andernfalls.</span><span class="sxs-lookup"><span data-stu-id="31300-119">True if the event is marked `private`, false otherwise.</span></span> |
|<span data-ttu-id="31300-120">location</span><span class="sxs-lookup"><span data-stu-id="31300-120">location</span></span> |<span data-ttu-id="31300-121">String</span><span class="sxs-lookup"><span data-stu-id="31300-121">String</span></span> | <span data-ttu-id="31300-122">Der Speicherort, an dem entsprechenden Ereigniscode gehalten oder teilnahmen aus.</span><span class="sxs-lookup"><span data-stu-id="31300-122">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="31300-123">Optional.</span><span class="sxs-lookup"><span data-stu-id="31300-123">Optional.</span></span>|
|<span data-ttu-id="31300-124">start</span><span class="sxs-lookup"><span data-stu-id="31300-124">start</span></span> |[<span data-ttu-id="31300-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="31300-125">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="31300-126">Das Datum, Uhrzeit und Zeitzone, die das zugehörige Ereignis beginnt.</span><span class="sxs-lookup"><span data-stu-id="31300-126">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="31300-127">status</span><span class="sxs-lookup"><span data-stu-id="31300-127">status</span></span> |<span data-ttu-id="31300-128">String</span><span class="sxs-lookup"><span data-stu-id="31300-128">String</span></span> | <span data-ttu-id="31300-129">Der Verfügbarkeitsstatus des Benutzers oder der Ressource während des entsprechenden Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="31300-129">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="31300-130">Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="31300-130">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="31300-131">Betreff</span><span class="sxs-lookup"><span data-stu-id="31300-131">subject</span></span> |<span data-ttu-id="31300-132">String</span><span class="sxs-lookup"><span data-stu-id="31300-132">String</span></span> | <span data-ttu-id="31300-133">Die Betreffzeile das entsprechende Ereignis.</span><span class="sxs-lookup"><span data-stu-id="31300-133">The corresponding event's subject line.</span></span> <span data-ttu-id="31300-134">Optional.</span><span class="sxs-lookup"><span data-stu-id="31300-134">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="31300-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="31300-135">JSON representation</span></span>

<span data-ttu-id="31300-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="31300-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

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
<!-- {
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->