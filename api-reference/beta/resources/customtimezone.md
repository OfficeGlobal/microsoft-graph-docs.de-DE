---
title: customTimeZone-Ressourcentyp
description: Stellt eine Zeitzone dar, in der der Übergang von Standardzeit zu Sommerzeit oder umgekehrt nicht Standard ist.
localization_priority: Normal
ms.openlocfilehash: 0bb961e213956ef3142df1f3d55a83918a14fa78
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515251"
---
# <a name="customtimezone-resource-type"></a><span data-ttu-id="15ccc-103">customTimeZone-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="15ccc-103">customTimeZone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15ccc-104">Stellt eine Zeitzone dar, in der der Übergang von Standardzeit zu Sommerzeit oder umgekehrt nicht Standard ist.</span><span class="sxs-lookup"><span data-stu-id="15ccc-104">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="15ccc-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="15ccc-105">Properties</span></span>
| <span data-ttu-id="15ccc-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15ccc-106">Property</span></span>     | <span data-ttu-id="15ccc-107">Typ</span><span class="sxs-lookup"><span data-stu-id="15ccc-107">Type</span></span>   |<span data-ttu-id="15ccc-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15ccc-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="15ccc-109">bias</span><span class="sxs-lookup"><span data-stu-id="15ccc-109">bias</span></span> | <span data-ttu-id="15ccc-110">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="15ccc-110">Edm.Int32</span></span> | <span data-ttu-id="15ccc-111">Der Zeitversatz der Zeitzone von der Koordinierten Weltzeit (UTC).</span><span class="sxs-lookup"><span data-stu-id="15ccc-111">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="15ccc-112">Dieser Wert wird in Minuten angegeben.</span><span class="sxs-lookup"><span data-stu-id="15ccc-112">This value is in minutes.</span></span><span data-ttu-id="15ccc-113">Zeitzonen, die der UTC voraus sind, haben einen positiven Versatz; Zeitzonen, die hinter der UTC liegen, haben einen negativen Versatz.</span><span class="sxs-lookup"><span data-stu-id="15ccc-113"> Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="15ccc-114">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="15ccc-114">daylightOffset</span></span> | [<span data-ttu-id="15ccc-115">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="15ccc-115">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="15ccc-116">Gibt an, wann die Zeitzone von Standardzeit in Sommerzeit wechselt.</span><span class="sxs-lookup"><span data-stu-id="15ccc-116">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="15ccc-117">name</span><span class="sxs-lookup"><span data-stu-id="15ccc-117">name</span></span> | <span data-ttu-id="15ccc-118">string</span><span class="sxs-lookup"><span data-stu-id="15ccc-118">string</span></span> | <span data-ttu-id="15ccc-119">Der Name der benutzerdefinierten Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="15ccc-119">The name of the custom time zone.</span></span> |
| <span data-ttu-id="15ccc-120">standardOffset</span><span class="sxs-lookup"><span data-stu-id="15ccc-120">standardOffset</span></span> | [<span data-ttu-id="15ccc-121">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="15ccc-121">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="15ccc-122">Gibt an, wann die Zeitzone von Sommerzeit in Standardzeit wechselt.</span><span class="sxs-lookup"><span data-stu-id="15ccc-122">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="15ccc-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="15ccc-123">JSON representation</span></span>

<span data-ttu-id="15ccc-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="15ccc-124">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/customtimezone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
