---
title: von ScheduleItem Ressourcentyp
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: e5d14826a27153af27648484554ec864d62ed6c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890433"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="eda23-104">von ScheduleItem Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="eda23-104">scheduleItem resource type</span></span>

 > <span data-ttu-id="eda23-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="eda23-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eda23-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eda23-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="eda23-107">Ein Element, das beschreibt die Verfügbarkeit eines Benutzers auf ein Ereignis tatsächliche auf Standardkalender des Benutzers entspricht.</span><span class="sxs-lookup"><span data-stu-id="eda23-107">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="eda23-108">Dieses Element gilt für als auch eine Ressource.</span><span class="sxs-lookup"><span data-stu-id="eda23-108">This item applies to a resource as well.</span></span>

## <a name="properties"></a><span data-ttu-id="eda23-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="eda23-109">Properties</span></span>
| <span data-ttu-id="eda23-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eda23-110">Property</span></span>     | <span data-ttu-id="eda23-111">Typ</span><span class="sxs-lookup"><span data-stu-id="eda23-111">Type</span></span>   |<span data-ttu-id="eda23-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eda23-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eda23-113">end</span><span class="sxs-lookup"><span data-stu-id="eda23-113">end</span></span> |[<span data-ttu-id="eda23-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="eda23-114">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="eda23-115">Das Datum, Uhrzeit und Zeitzone, die das zugehörige Ereignis endet.</span><span class="sxs-lookup"><span data-stu-id="eda23-115">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="eda23-116">isPrivate</span><span class="sxs-lookup"><span data-stu-id="eda23-116">isPrivate</span></span> |<span data-ttu-id="eda23-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="eda23-117">Boolean</span></span> |<span data-ttu-id="eda23-118">Die Vertraulichkeit des entsprechenden Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="eda23-118">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="eda23-119">True, wenn das Ereignis markiert wird `private`false andernfalls.</span><span class="sxs-lookup"><span data-stu-id="eda23-119">True if the event is marked `private`, false otherwise.</span></span> |
|<span data-ttu-id="eda23-120">location</span><span class="sxs-lookup"><span data-stu-id="eda23-120">location</span></span> |<span data-ttu-id="eda23-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eda23-121">String</span></span> | <span data-ttu-id="eda23-122">Der Speicherort, an dem entsprechenden Ereigniscode gehalten oder teilnahmen aus.</span><span class="sxs-lookup"><span data-stu-id="eda23-122">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="eda23-123">Optional.</span><span class="sxs-lookup"><span data-stu-id="eda23-123">Optional.</span></span>|
|<span data-ttu-id="eda23-124">start</span><span class="sxs-lookup"><span data-stu-id="eda23-124">start</span></span> |[<span data-ttu-id="eda23-125">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="eda23-125">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="eda23-126">Das Datum, Uhrzeit und Zeitzone, die das zugehörige Ereignis beginnt.</span><span class="sxs-lookup"><span data-stu-id="eda23-126">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="eda23-127">status</span><span class="sxs-lookup"><span data-stu-id="eda23-127">status</span></span> |<span data-ttu-id="eda23-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eda23-128">String</span></span> | <span data-ttu-id="eda23-129">Der Verfügbarkeitsstatus des Benutzers oder der Ressource während des entsprechenden Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="eda23-129">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="eda23-130">Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="eda23-130">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="eda23-131">Betreff</span><span class="sxs-lookup"><span data-stu-id="eda23-131">subject</span></span> |<span data-ttu-id="eda23-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eda23-132">String</span></span> | <span data-ttu-id="eda23-133">Die Betreffzeile das entsprechende Ereignis.</span><span class="sxs-lookup"><span data-stu-id="eda23-133">The corresponding event's subject line.</span></span> <span data-ttu-id="eda23-134">Optional.</span><span class="sxs-lookup"><span data-stu-id="eda23-134">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="eda23-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="eda23-135">JSON representation</span></span>

<span data-ttu-id="eda23-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="eda23-136">The following is a JSON representation of the resource.</span></span>

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
