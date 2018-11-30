---
title: standardTimeZoneOffset-Ressourcentyp
description: Gibt an, wann eine Zeitzone von Sommerzeit in Standardzeit wechselt.
ms.openlocfilehash: 53c02a231d31dbdd1723fb0d8b476c988ff1d4ec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018593"
---
# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="61c2d-103">standardTimeZoneOffset-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="61c2d-103">standardTimeZoneOffset resource type</span></span>

<span data-ttu-id="61c2d-104">Gibt an, wann eine Zeitzone von Sommerzeit in Standardzeit wechselt.</span><span class="sxs-lookup"><span data-stu-id="61c2d-104">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="61c2d-105">Wenn eine Zeitzone beispielsweise mit den folgenden Eigenschaften angegeben wird:</span><span class="sxs-lookup"><span data-stu-id="61c2d-105">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="61c2d-106">**dayOccurrence** ist 3</span><span class="sxs-lookup"><span data-stu-id="61c2d-106">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="61c2d-107">**dayOfWeek** ist „Sonntag“</span><span class="sxs-lookup"><span data-stu-id="61c2d-107">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="61c2d-108">**month** ist 10</span><span class="sxs-lookup"><span data-stu-id="61c2d-108">**month** is 10</span></span>
- <span data-ttu-id="61c2d-109">**time** 02:00:00 _ ist **year** ist 0. Dies bedeutet, dass der Übergang von Sommerzeit zu Standardzeit jedes Jahr um 2 Uhr am dritten Sonntag im Oktober stattfindet.</span><span class="sxs-lookup"><span data-stu-id="61c2d-109">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="61c2d-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="61c2d-110">Properties</span></span>
| <span data-ttu-id="61c2d-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61c2d-111">Property</span></span>     | <span data-ttu-id="61c2d-112">Typ</span><span class="sxs-lookup"><span data-stu-id="61c2d-112">Type</span></span>   |<span data-ttu-id="61c2d-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61c2d-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="61c2d-114">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="61c2d-114">dayOccurrence</span></span> | <span data-ttu-id="61c2d-115">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="61c2d-115">Edm.Int32</span></span> | <span data-ttu-id="61c2d-116">Stellt das n-te Vorkommen des Wochentags dar, an dem der Übergang von Sommerzeit zu Standardzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="61c2d-116">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="61c2d-117">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="61c2d-117">dayOfWeek</span></span> | <span data-ttu-id="61c2d-118">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="61c2d-118">dayOfWeek</span></span> | <span data-ttu-id="61c2d-119">Stellt den Wochentag dar, an dem der Übergang von Sommerzeit zu Standardzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="61c2d-119">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="61c2d-120">month</span><span class="sxs-lookup"><span data-stu-id="61c2d-120">month</span></span> | <span data-ttu-id="61c2d-121">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="61c2d-121">Edm.Int32</span></span> | <span data-ttu-id="61c2d-122">Stellt den Monat dar, an dem der Übergang von Sommerzeit zu Standardzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="61c2d-122">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="61c2d-123">time</span><span class="sxs-lookup"><span data-stu-id="61c2d-123">time</span></span> | <span data-ttu-id="61c2d-124">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="61c2d-124">Edm.TimeOfDay</span></span> | <span data-ttu-id="61c2d-125">Stellt die Uhrzeit dar, zu der der Übergang von Sommerzeit zu Standardzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="61c2d-125">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="61c2d-126">year</span><span class="sxs-lookup"><span data-stu-id="61c2d-126">year</span></span> | <span data-ttu-id="61c2d-127">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="61c2d-127">Edm.Int32</span></span> | <span data-ttu-id="61c2d-128">Stellt dar, wie häufig der Wechsel von Sommerzeit zu Standardzeit in einem Jahr erfolgt.</span><span class="sxs-lookup"><span data-stu-id="61c2d-128">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="61c2d-129">Der Wert 0 bedeutet z. B. jedes Jahr.</span><span class="sxs-lookup"><span data-stu-id="61c2d-129">For example, a value of 0 means every year.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61c2d-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="61c2d-130">JSON representation</span></span>

<span data-ttu-id="61c2d-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="61c2d-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.standardTimeZoneOffset"
}-->

```json
{
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
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->