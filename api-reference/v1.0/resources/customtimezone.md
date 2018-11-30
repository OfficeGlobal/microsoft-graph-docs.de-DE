---
title: customTimeZone-Ressourcentyp
description: Stellt eine Zeitzone dar, in der der Übergang von Standardzeit zu Sommerzeit oder umgekehrt nicht Standard ist.
ms.openlocfilehash: 36d497e3e6ad52ca5a59f4bc322410ee271e73bf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017338"
---
# <a name="customtimezone-resource-type"></a><span data-ttu-id="a054b-103">customTimeZone-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a054b-103">customTimeZone resource type</span></span>

<span data-ttu-id="a054b-104">Stellt eine Zeitzone dar, in der der Übergang von Standardzeit zu Sommerzeit oder umgekehrt nicht Standard ist.</span><span class="sxs-lookup"><span data-stu-id="a054b-104">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="a054b-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a054b-105">Properties</span></span>
| <span data-ttu-id="a054b-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a054b-106">Property</span></span>     | <span data-ttu-id="a054b-107">Typ</span><span class="sxs-lookup"><span data-stu-id="a054b-107">Type</span></span>   |<span data-ttu-id="a054b-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a054b-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a054b-109">bias</span><span class="sxs-lookup"><span data-stu-id="a054b-109">bias</span></span> | <span data-ttu-id="a054b-110">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="a054b-110">Edm.Int32</span></span> | <span data-ttu-id="a054b-111">Der Zeitversatz der Zeitzone von der Koordinierten Weltzeit (UTC).</span><span class="sxs-lookup"><span data-stu-id="a054b-111">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="a054b-112">Dieser Wert wird in Minuten angegeben.</span><span class="sxs-lookup"><span data-stu-id="a054b-112">This value is in minutes.</span></span><span data-ttu-id="a054b-113">Zeitzonen, die der UTC voraus sind, haben einen positiven Versatz; Zeitzonen, die hinter der UTC liegen, haben einen negativen Versatz.</span><span class="sxs-lookup"><span data-stu-id="a054b-113"> Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="a054b-114">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="a054b-114">daylightOffset</span></span> | [<span data-ttu-id="a054b-115">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="a054b-115">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="a054b-116">Gibt an, wann die Zeitzone von Standardzeit in Sommerzeit wechselt.</span><span class="sxs-lookup"><span data-stu-id="a054b-116">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="a054b-117">name</span><span class="sxs-lookup"><span data-stu-id="a054b-117">name</span></span> | <span data-ttu-id="a054b-118">string</span><span class="sxs-lookup"><span data-stu-id="a054b-118">string</span></span> | <span data-ttu-id="a054b-119">Der Name der benutzerdefinierten Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="a054b-119">The name of the custom time zone.</span></span> |
| <span data-ttu-id="a054b-120">standardOffset</span><span class="sxs-lookup"><span data-stu-id="a054b-120">standardOffset</span></span> | [<span data-ttu-id="a054b-121">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="a054b-121">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="a054b-122">Gibt an, wann die Zeitzone von Sommerzeit in Standardzeit wechselt.</span><span class="sxs-lookup"><span data-stu-id="a054b-122">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="a054b-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a054b-123">JSON representation</span></span>

<span data-ttu-id="a054b-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a054b-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.timeZoneBase",
  "@odata.type": "microsoft.graph.customTimeZone"
}-->

```json
{
  "bias": "Int32",
  "daylightOffset": {"@odata.type": "microsoft.graph.daylightTimeZoneOffset"},
  "name": "string",
  "standardOffset": {"@odata.type": "microsoft.graph.standardTimeZoneOffset"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->