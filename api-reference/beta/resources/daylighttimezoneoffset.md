---
title: daylightTimeZoneOffset-Ressourcentyp
description: Gibt an, wann eine Zeitzone von Standardzeit in Sommerzeit wechselt.
localization_priority: Normal
ms.openlocfilehash: 37e08ec0e695fd245678510ac4a40bc978b1a93e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825606"
---
# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="34541-103">daylightTimeZoneOffset-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="34541-103">daylightTimeZoneOffset resource type</span></span>

> <span data-ttu-id="34541-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="34541-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34541-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34541-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34541-106">Gibt an, wann eine Zeitzone von Standardzeit in Sommerzeit wechselt.</span><span class="sxs-lookup"><span data-stu-id="34541-106">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="34541-107">Wenn eine Zeitzone beispielsweise mit den folgenden Eigenschaften angegeben wird:</span><span class="sxs-lookup"><span data-stu-id="34541-107">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="34541-108">**bias** ist 300</span><span class="sxs-lookup"><span data-stu-id="34541-108">**bias** is 300</span></span>
- <span data-ttu-id="34541-109">**daylightBias** ist -100</span><span class="sxs-lookup"><span data-stu-id="34541-109">**daylightBias** is -100</span></span>
- <span data-ttu-id="34541-110">**dayOccurrence** ist 4</span><span class="sxs-lookup"><span data-stu-id="34541-110">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="34541-111">**dayOfWeek** ist „Sonntag“</span><span class="sxs-lookup"><span data-stu-id="34541-111">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="34541-112">**month** ist 5</span><span class="sxs-lookup"><span data-stu-id="34541-112">**month** is 5</span></span>
- <span data-ttu-id="34541-113">**time** ist  02:00:00 _ **year** ist 0. Dies bedeutet, dass die Zeit während der Sommerzeit +300-100=200 Minuten vor der UTC-Zeit liegt.</span><span class="sxs-lookup"><span data-stu-id="34541-113">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="34541-114">Der Übergang von Sommerzeit zu Standardzeit findet jedes Jahr um 2 Uhr am vierten Sonntag im Mai stattfindet.</span><span class="sxs-lookup"><span data-stu-id="34541-114">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="34541-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="34541-115">Properties</span></span>
| <span data-ttu-id="34541-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="34541-116">Property</span></span>     | <span data-ttu-id="34541-117">Typ</span><span class="sxs-lookup"><span data-stu-id="34541-117">Type</span></span>   |<span data-ttu-id="34541-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34541-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="34541-119">daylightBias</span><span class="sxs-lookup"><span data-stu-id="34541-119">daylightBias</span></span> | <span data-ttu-id="34541-120">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="34541-120">Edm.Int32</span></span> | <span data-ttu-id="34541-121">Der Zeitversatz der Sommerzeit von der Koordinierten Weltzeit (UTC).</span><span class="sxs-lookup"><span data-stu-id="34541-121">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="34541-122">Dieser Wert wird in Minuten angegeben.</span><span class="sxs-lookup"><span data-stu-id="34541-122">This value is in minutes.</span></span>  |
| <span data-ttu-id="34541-123">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="34541-123">dayOccurrence</span></span> | <span data-ttu-id="34541-124">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="34541-124">Edm.Int32</span></span> | <span data-ttu-id="34541-125">Stellt das n-te Vorkommen des Wochentags dar, an dem der Übergang von Standardzeit zu Sommerzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="34541-125">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="34541-126">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="34541-126">dayOfWeek</span></span> | <span data-ttu-id="34541-127">string</span><span class="sxs-lookup"><span data-stu-id="34541-127">string</span></span> | <span data-ttu-id="34541-128">Stellt den Wochentag dar, an dem der Übergang von Standardzeit zu Sommerzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="34541-128">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="34541-129">Monat</span><span class="sxs-lookup"><span data-stu-id="34541-129">month</span></span> | <span data-ttu-id="34541-130">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="34541-130">Edm.Int32</span></span> | <span data-ttu-id="34541-131">Stellt den Monat dar, in dem der Übergang von Standardzeit zu Sommerzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="34541-131">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="34541-132">Uhrzeit</span><span class="sxs-lookup"><span data-stu-id="34541-132">time</span></span> | <span data-ttu-id="34541-133">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="34541-133">Edm.TimeOfDay</span></span> | <span data-ttu-id="34541-134">Stellt die Uhrzeit dar, zu der der Übergang von Standardzeit zu Sommerzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="34541-134">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="34541-135">Jahr</span><span class="sxs-lookup"><span data-stu-id="34541-135">year</span></span> | <span data-ttu-id="34541-136">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="34541-136">Edm.Int32</span></span> | <span data-ttu-id="34541-137">Stellt dar, wie häufig der Wechsel von Standardzeit zu Sommerzeit in einem Jahr erfolgt.</span><span class="sxs-lookup"><span data-stu-id="34541-137">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="34541-138">Der Wert 0 bedeutet z. B. jedes Jahr.</span><span class="sxs-lookup"><span data-stu-id="34541-138">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="34541-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="34541-139">JSON representation</span></span>

<span data-ttu-id="34541-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="34541-140">Here is a JSON representation of the resource.</span></span>

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
