---
title: daylightTimeZoneOffset-Ressourcentyp
description: Gibt an, wann eine Zeitzone von Standardzeit in Sommerzeit wechselt.
ms.openlocfilehash: 1504a3c1bb1b2d6c691aadf1d073a95453f76d2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058525"
---
# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="b03e1-103">daylightTimeZoneOffset-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b03e1-103">daylightTimeZoneOffset resource type</span></span>

> <span data-ttu-id="b03e1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b03e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b03e1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b03e1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b03e1-106">Gibt an, wann eine Zeitzone von Standardzeit in Sommerzeit wechselt.</span><span class="sxs-lookup"><span data-stu-id="b03e1-106">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="b03e1-107">Wenn eine Zeitzone beispielsweise mit den folgenden Eigenschaften angegeben wird:</span><span class="sxs-lookup"><span data-stu-id="b03e1-107">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="b03e1-108">**bias** ist 300</span><span class="sxs-lookup"><span data-stu-id="b03e1-108">**bias** is 300</span></span>
- <span data-ttu-id="b03e1-109">**daylightBias** ist -100</span><span class="sxs-lookup"><span data-stu-id="b03e1-109">**daylightBias** is -100</span></span>
- <span data-ttu-id="b03e1-110">**dayOccurrence** ist 4</span><span class="sxs-lookup"><span data-stu-id="b03e1-110">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="b03e1-111">**dayOfWeek** ist „Sonntag“</span><span class="sxs-lookup"><span data-stu-id="b03e1-111">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="b03e1-112">**month** ist 5</span><span class="sxs-lookup"><span data-stu-id="b03e1-112">**month** is 5</span></span>
- <span data-ttu-id="b03e1-113">**time** ist  02:00:00 _ **year** ist 0. Dies bedeutet, dass die Zeit während der Sommerzeit +300-100=200 Minuten vor der UTC-Zeit liegt.</span><span class="sxs-lookup"><span data-stu-id="b03e1-113">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="b03e1-114">Der Übergang von Sommerzeit zu Standardzeit findet jedes Jahr um 2 Uhr am vierten Sonntag im Mai stattfindet.</span><span class="sxs-lookup"><span data-stu-id="b03e1-114">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="b03e1-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b03e1-115">Properties</span></span>
| <span data-ttu-id="b03e1-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b03e1-116">Property</span></span>     | <span data-ttu-id="b03e1-117">Typ</span><span class="sxs-lookup"><span data-stu-id="b03e1-117">Type</span></span>   |<span data-ttu-id="b03e1-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b03e1-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b03e1-119">daylightBias</span><span class="sxs-lookup"><span data-stu-id="b03e1-119">daylightBias</span></span> | <span data-ttu-id="b03e1-120">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="b03e1-120">Edm.Int32</span></span> | <span data-ttu-id="b03e1-121">Der Zeitversatz der Sommerzeit von der Koordinierten Weltzeit (UTC).</span><span class="sxs-lookup"><span data-stu-id="b03e1-121">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="b03e1-122">Dieser Wert wird in Minuten angegeben.</span><span class="sxs-lookup"><span data-stu-id="b03e1-122">This value is in minutes.</span></span>  |
| <span data-ttu-id="b03e1-123">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="b03e1-123">dayOccurrence</span></span> | <span data-ttu-id="b03e1-124">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="b03e1-124">Edm.Int32</span></span> | <span data-ttu-id="b03e1-125">Stellt das n-te Vorkommen des Wochentags dar, an dem der Übergang von Standardzeit zu Sommerzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="b03e1-125">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="b03e1-126">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="b03e1-126">dayOfWeek</span></span> | <span data-ttu-id="b03e1-127">string</span><span class="sxs-lookup"><span data-stu-id="b03e1-127">string</span></span> | <span data-ttu-id="b03e1-128">Stellt den Wochentag dar, an dem der Übergang von Standardzeit zu Sommerzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="b03e1-128">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="b03e1-129">Monat</span><span class="sxs-lookup"><span data-stu-id="b03e1-129">month</span></span> | <span data-ttu-id="b03e1-130">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="b03e1-130">Edm.Int32</span></span> | <span data-ttu-id="b03e1-131">Stellt den Monat dar, in dem der Übergang von Standardzeit zu Sommerzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="b03e1-131">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="b03e1-132">Uhrzeit</span><span class="sxs-lookup"><span data-stu-id="b03e1-132">time</span></span> | <span data-ttu-id="b03e1-133">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b03e1-133">Edm.TimeOfDay</span></span> | <span data-ttu-id="b03e1-134">Stellt die Uhrzeit dar, zu der der Übergang von Standardzeit zu Sommerzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="b03e1-134">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="b03e1-135">Jahr</span><span class="sxs-lookup"><span data-stu-id="b03e1-135">year</span></span> | <span data-ttu-id="b03e1-136">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="b03e1-136">Edm.Int32</span></span> | <span data-ttu-id="b03e1-137">Stellt dar, wie häufig der Wechsel von Standardzeit zu Sommerzeit in einem Jahr erfolgt.</span><span class="sxs-lookup"><span data-stu-id="b03e1-137">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="b03e1-138">Der Wert 0 bedeutet z. B. jedes Jahr.</span><span class="sxs-lookup"><span data-stu-id="b03e1-138">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b03e1-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b03e1-139">JSON representation</span></span>

<span data-ttu-id="b03e1-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b03e1-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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