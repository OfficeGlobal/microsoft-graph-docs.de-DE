---
title: standardTimeZoneOffset-Ressourcentyp
description: Gibt an, wann eine Zeitzone von Sommerzeit in Standardzeit wechselt.
localization_priority: Normal
ms.openlocfilehash: 04808d73a6ac41be8eec2959f5ff1d8c5caa44d1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841244"
---
# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="9aacb-103">standardTimeZoneOffset-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9aacb-103">standardTimeZoneOffset resource type</span></span>

> <span data-ttu-id="9aacb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9aacb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9aacb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9aacb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9aacb-106">Gibt an, wann eine Zeitzone von Sommerzeit in Standardzeit wechselt.</span><span class="sxs-lookup"><span data-stu-id="9aacb-106">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="9aacb-107">Wenn eine Zeitzone beispielsweise mit den folgenden Eigenschaften angegeben wird:</span><span class="sxs-lookup"><span data-stu-id="9aacb-107">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="9aacb-108">**dayOccurrence** ist 3</span><span class="sxs-lookup"><span data-stu-id="9aacb-108">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="9aacb-109">**dayOfWeek** ist „Sonntag“</span><span class="sxs-lookup"><span data-stu-id="9aacb-109">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="9aacb-110">**month** ist 10</span><span class="sxs-lookup"><span data-stu-id="9aacb-110">**month** is 10</span></span>
- <span data-ttu-id="9aacb-111">**time** 02:00:00 _ ist **year** ist 0. Dies bedeutet, dass der Übergang von Sommerzeit zu Standardzeit jedes Jahr um 2 Uhr am dritten Sonntag im Oktober stattfindet.</span><span class="sxs-lookup"><span data-stu-id="9aacb-111">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="9aacb-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9aacb-112">Properties</span></span>
| <span data-ttu-id="9aacb-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9aacb-113">Property</span></span>     | <span data-ttu-id="9aacb-114">Typ</span><span class="sxs-lookup"><span data-stu-id="9aacb-114">Type</span></span>   |<span data-ttu-id="9aacb-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9aacb-115">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9aacb-116">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="9aacb-116">dayOccurrence</span></span> | <span data-ttu-id="9aacb-117">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="9aacb-117">Edm.Int32</span></span> | <span data-ttu-id="9aacb-118">Stellt das n-te Vorkommen des Wochentags dar, an dem der Übergang von Sommerzeit zu Standardzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="9aacb-118">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="9aacb-119">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="9aacb-119">dayOfWeek</span></span> | <span data-ttu-id="9aacb-120">string</span><span class="sxs-lookup"><span data-stu-id="9aacb-120">string</span></span> | <span data-ttu-id="9aacb-121">Stellt den Wochentag dar, an dem der Übergang von Sommerzeit zu Standardzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="9aacb-121">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="9aacb-122">month</span><span class="sxs-lookup"><span data-stu-id="9aacb-122">month</span></span> | <span data-ttu-id="9aacb-123">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="9aacb-123">Edm.Int32</span></span> | <span data-ttu-id="9aacb-124">Stellt den Monat dar, an dem der Übergang von Sommerzeit zu Standardzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="9aacb-124">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="9aacb-125">time</span><span class="sxs-lookup"><span data-stu-id="9aacb-125">time</span></span> | <span data-ttu-id="9aacb-126">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9aacb-126">Edm.TimeOfDay</span></span> | <span data-ttu-id="9aacb-127">Stellt die Uhrzeit dar, zu der der Übergang von Sommerzeit zu Standardzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="9aacb-127">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="9aacb-128">year</span><span class="sxs-lookup"><span data-stu-id="9aacb-128">year</span></span> | <span data-ttu-id="9aacb-129">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="9aacb-129">Edm.Int32</span></span> | <span data-ttu-id="9aacb-130">Stellt dar, wie häufig der Wechsel von Sommerzeit zu Standardzeit in einem Jahr erfolgt.</span><span class="sxs-lookup"><span data-stu-id="9aacb-130">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="9aacb-131">Der Wert 0 bedeutet z. B. jedes Jahr.</span><span class="sxs-lookup"><span data-stu-id="9aacb-131">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9aacb-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9aacb-132">JSON representation</span></span>

<span data-ttu-id="9aacb-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9aacb-133">Here is a JSON representation of the resource.</span></span>

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
