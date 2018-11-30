---
title: daylightTimeZoneOffset-Ressourcentyp
description: Gibt an, wann eine Zeitzone von Standardzeit in Sommerzeit wechselt.
ms.openlocfilehash: bab5be49e88de1c71c7d13f53c15158e4a253a6a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016004"
---
# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="ec96b-103">daylightTimeZoneOffset-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ec96b-103">daylightTimeZoneOffset resource type</span></span>

<span data-ttu-id="ec96b-104">Gibt an, wann eine Zeitzone von Standardzeit in Sommerzeit wechselt.</span><span class="sxs-lookup"><span data-stu-id="ec96b-104">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="ec96b-105">Wenn eine Zeitzone beispielsweise mit den folgenden Eigenschaften angegeben wird:</span><span class="sxs-lookup"><span data-stu-id="ec96b-105">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="ec96b-106">**bias** ist 300</span><span class="sxs-lookup"><span data-stu-id="ec96b-106">**bias** is 300</span></span>
- <span data-ttu-id="ec96b-107">**daylightBias** ist -100</span><span class="sxs-lookup"><span data-stu-id="ec96b-107">**daylightBias** is -100</span></span>
- <span data-ttu-id="ec96b-108">**dayOccurrence** ist 4</span><span class="sxs-lookup"><span data-stu-id="ec96b-108">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="ec96b-109">**dayOfWeek** ist „Sonntag“</span><span class="sxs-lookup"><span data-stu-id="ec96b-109">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="ec96b-110">**month** ist 5</span><span class="sxs-lookup"><span data-stu-id="ec96b-110">**month** is 5</span></span>
- <span data-ttu-id="ec96b-111">**time** ist  02:00:00 _ **year** ist 0. Dies bedeutet, dass die Zeit während der Sommerzeit +300-100=200 Minuten vor der UTC-Zeit liegt.</span><span class="sxs-lookup"><span data-stu-id="ec96b-111">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="ec96b-112">Der Übergang von Sommerzeit zu Standardzeit findet jedes Jahr um 2 Uhr am vierten Sonntag im Mai stattfindet.</span><span class="sxs-lookup"><span data-stu-id="ec96b-112">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="ec96b-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ec96b-113">Properties</span></span>
| <span data-ttu-id="ec96b-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ec96b-114">Property</span></span>     | <span data-ttu-id="ec96b-115">Typ</span><span class="sxs-lookup"><span data-stu-id="ec96b-115">Type</span></span>   |<span data-ttu-id="ec96b-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec96b-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ec96b-117">daylightBias</span><span class="sxs-lookup"><span data-stu-id="ec96b-117">daylightBias</span></span> | <span data-ttu-id="ec96b-118">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="ec96b-118">Edm.Int32</span></span> | <span data-ttu-id="ec96b-119">Der Zeitversatz der Sommerzeit von der Koordinierten Weltzeit (UTC).</span><span class="sxs-lookup"><span data-stu-id="ec96b-119">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="ec96b-120">Dieser Wert wird in Minuten angegeben.</span><span class="sxs-lookup"><span data-stu-id="ec96b-120">This value is in minutes.</span></span>  |
| <span data-ttu-id="ec96b-121">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="ec96b-121">dayOccurrence</span></span> | <span data-ttu-id="ec96b-122">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="ec96b-122">Edm.Int32</span></span> | <span data-ttu-id="ec96b-123">Stellt das n-te Vorkommen des Wochentags dar, an dem der Übergang von Standardzeit zu Sommerzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="ec96b-123">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="ec96b-124">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="ec96b-124">dayOfWeek</span></span> | <span data-ttu-id="ec96b-125">string</span><span class="sxs-lookup"><span data-stu-id="ec96b-125">string</span></span> | <span data-ttu-id="ec96b-126">Stellt den Wochentag dar, an dem der Übergang von Standardzeit zu Sommerzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="ec96b-126">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="ec96b-127">Monat</span><span class="sxs-lookup"><span data-stu-id="ec96b-127">month</span></span> | <span data-ttu-id="ec96b-128">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="ec96b-128">Edm.Int32</span></span> | <span data-ttu-id="ec96b-129">Stellt den Monat dar, in dem der Übergang von Standardzeit zu Sommerzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="ec96b-129">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="ec96b-130">Uhrzeit</span><span class="sxs-lookup"><span data-stu-id="ec96b-130">time</span></span> | <span data-ttu-id="ec96b-131">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ec96b-131">Edm.TimeOfDay</span></span> | <span data-ttu-id="ec96b-132">Stellt die Uhrzeit dar, zu der der Übergang von Standardzeit zu Sommerzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="ec96b-132">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="ec96b-133">Jahr</span><span class="sxs-lookup"><span data-stu-id="ec96b-133">year</span></span> | <span data-ttu-id="ec96b-134">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="ec96b-134">Edm.Int32</span></span> | <span data-ttu-id="ec96b-135">Stellt dar, wie häufig der Wechsel von Standardzeit zu Sommerzeit in einem Jahr erfolgt.</span><span class="sxs-lookup"><span data-stu-id="ec96b-135">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="ec96b-136">Der Wert 0 bedeutet z. B. jedes Jahr.</span><span class="sxs-lookup"><span data-stu-id="ec96b-136">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ec96b-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ec96b-137">JSON representation</span></span>

<span data-ttu-id="ec96b-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ec96b-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.standardTimeZoneOffset",
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}-->

```json
{
  "daylightBias": "Int32",
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->