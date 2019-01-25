---
title: standardTimeZoneOffset-Ressourcentyp
description: Gibt an, wann eine Zeitzone von Sommerzeit in Standardzeit wechselt.
localization_priority: Normal
ms.openlocfilehash: cc3de9a0977caf6c222291fdff2b4e0f96a9d9e5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514481"
---
# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="0b559-103">standardTimeZoneOffset-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0b559-103">standardTimeZoneOffset resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b559-104">Gibt an, wann eine Zeitzone von Sommerzeit in Standardzeit wechselt.</span><span class="sxs-lookup"><span data-stu-id="0b559-104">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="0b559-105">Wenn eine Zeitzone beispielsweise mit den folgenden Eigenschaften angegeben wird:</span><span class="sxs-lookup"><span data-stu-id="0b559-105">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="0b559-106">**dayOccurrence** ist 3</span><span class="sxs-lookup"><span data-stu-id="0b559-106">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="0b559-107">**dayOfWeek** ist „Sonntag“</span><span class="sxs-lookup"><span data-stu-id="0b559-107">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="0b559-108">**month** ist 10</span><span class="sxs-lookup"><span data-stu-id="0b559-108">**month** is 10</span></span>
- <span data-ttu-id="0b559-109">**time** 02:00:00 _ ist **year** ist 0. Dies bedeutet, dass der Übergang von Sommerzeit zu Standardzeit jedes Jahr um 2 Uhr am dritten Sonntag im Oktober stattfindet.</span><span class="sxs-lookup"><span data-stu-id="0b559-109">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="0b559-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0b559-110">Properties</span></span>
| <span data-ttu-id="0b559-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0b559-111">Property</span></span>     | <span data-ttu-id="0b559-112">Typ</span><span class="sxs-lookup"><span data-stu-id="0b559-112">Type</span></span>   |<span data-ttu-id="0b559-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b559-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0b559-114">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="0b559-114">dayOccurrence</span></span> | <span data-ttu-id="0b559-115">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="0b559-115">Edm.Int32</span></span> | <span data-ttu-id="0b559-116">Stellt das n-te Vorkommen des Wochentags dar, an dem der Übergang von Sommerzeit zu Standardzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="0b559-116">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="0b559-117">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="0b559-117">dayOfWeek</span></span> | <span data-ttu-id="0b559-118">string</span><span class="sxs-lookup"><span data-stu-id="0b559-118">string</span></span> | <span data-ttu-id="0b559-119">Stellt den Wochentag dar, an dem der Übergang von Sommerzeit zu Standardzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="0b559-119">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="0b559-120">month</span><span class="sxs-lookup"><span data-stu-id="0b559-120">month</span></span> | <span data-ttu-id="0b559-121">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="0b559-121">Edm.Int32</span></span> | <span data-ttu-id="0b559-122">Stellt den Monat dar, an dem der Übergang von Sommerzeit zu Standardzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="0b559-122">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="0b559-123">time</span><span class="sxs-lookup"><span data-stu-id="0b559-123">time</span></span> | <span data-ttu-id="0b559-124">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0b559-124">Edm.TimeOfDay</span></span> | <span data-ttu-id="0b559-125">Stellt die Uhrzeit dar, zu der der Übergang von Sommerzeit zu Standardzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="0b559-125">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="0b559-126">year</span><span class="sxs-lookup"><span data-stu-id="0b559-126">year</span></span> | <span data-ttu-id="0b559-127">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="0b559-127">Edm.Int32</span></span> | <span data-ttu-id="0b559-128">Stellt dar, wie häufig der Wechsel von Sommerzeit zu Standardzeit in einem Jahr erfolgt.</span><span class="sxs-lookup"><span data-stu-id="0b559-128">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="0b559-129">Der Wert 0 bedeutet z. B. jedes Jahr.</span><span class="sxs-lookup"><span data-stu-id="0b559-129">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0b559-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0b559-130">JSON representation</span></span>

<span data-ttu-id="0b559-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0b559-131">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/standardtimezoneoffset.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
