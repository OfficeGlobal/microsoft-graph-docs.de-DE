---
title: customTimeZone-Ressourcentyp
description: Stellt eine Zeitzone dar, in der der Übergang von Standardzeit zu Sommerzeit oder umgekehrt nicht Standard ist.
ms.openlocfilehash: 83375c96e4247cb0ddf2d17b1bede2c295f0b27f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058250"
---
# <a name="customtimezone-resource-type"></a><span data-ttu-id="b1563-103">customTimeZone-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b1563-103">customTimeZone resource type</span></span>

> <span data-ttu-id="b1563-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b1563-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1563-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b1563-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1563-106">Stellt eine Zeitzone dar, in der der Übergang von Standardzeit zu Sommerzeit oder umgekehrt nicht Standard ist.</span><span class="sxs-lookup"><span data-stu-id="b1563-106">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="b1563-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b1563-107">Properties</span></span>
| <span data-ttu-id="b1563-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b1563-108">Property</span></span>     | <span data-ttu-id="b1563-109">Typ</span><span class="sxs-lookup"><span data-stu-id="b1563-109">Type</span></span>   |<span data-ttu-id="b1563-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1563-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b1563-111">bias</span><span class="sxs-lookup"><span data-stu-id="b1563-111">bias</span></span> | <span data-ttu-id="b1563-112">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="b1563-112">Edm.Int32</span></span> | <span data-ttu-id="b1563-113">Der Zeitversatz der Zeitzone von der Koordinierten Weltzeit (UTC).</span><span class="sxs-lookup"><span data-stu-id="b1563-113">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="b1563-114">Dieser Wert wird in Minuten angegeben.</span><span class="sxs-lookup"><span data-stu-id="b1563-114">This value is in minutes.</span></span><span data-ttu-id="b1563-115">Zeitzonen, die der UTC voraus sind, haben einen positiven Versatz; Zeitzonen, die hinter der UTC liegen, haben einen negativen Versatz.</span><span class="sxs-lookup"><span data-stu-id="b1563-115"> Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="b1563-116">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="b1563-116">daylightOffset</span></span> | [<span data-ttu-id="b1563-117">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="b1563-117">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="b1563-118">Gibt an, wann die Zeitzone von Standardzeit in Sommerzeit wechselt.</span><span class="sxs-lookup"><span data-stu-id="b1563-118">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="b1563-119">name</span><span class="sxs-lookup"><span data-stu-id="b1563-119">name</span></span> | <span data-ttu-id="b1563-120">string</span><span class="sxs-lookup"><span data-stu-id="b1563-120">string</span></span> | <span data-ttu-id="b1563-121">Der Name der benutzerdefinierten Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="b1563-121">The name of the custom time zone.</span></span> |
| <span data-ttu-id="b1563-122">standardOffset</span><span class="sxs-lookup"><span data-stu-id="b1563-122">standardOffset</span></span> | [<span data-ttu-id="b1563-123">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="b1563-123">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="b1563-124">Gibt an, wann die Zeitzone von Sommerzeit in Standardzeit wechselt.</span><span class="sxs-lookup"><span data-stu-id="b1563-124">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="b1563-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b1563-125">JSON representation</span></span>

<span data-ttu-id="b1563-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b1563-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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