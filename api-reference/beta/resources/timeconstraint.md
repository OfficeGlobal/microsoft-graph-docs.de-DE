---
title: Ressourcentyp „timeConstraint“
description: Schränkt die Vorschläge für Besprechungszeiten auf bestimmte Stunden und Tage der Woche entsprechend der angegebenen Aktivität und den geöffneten Zeitschlitzen ein.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 680ada778ea64f982e9ed5fac11c935a6cce55d5
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/28/2019
ms.locfileid: "30937784"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="66659-103">Ressourcentyp „timeConstraint“</span><span class="sxs-lookup"><span data-stu-id="66659-103">timeConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66659-104">Schränkt die Vorschläge für Besprechungszeiten auf bestimmte Stunden und Tage der Woche entsprechend der angegebenen Aktivität und den geöffneten Zeitschlitzen ein.</span><span class="sxs-lookup"><span data-stu-id="66659-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>


## <a name="json-representation"></a><span data-ttu-id="66659-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="66659-105">JSON representation</span></span>
<span data-ttu-id="66659-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="66659-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeConstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}
```

## <a name="properties"></a><span data-ttu-id="66659-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="66659-107">Properties</span></span>
| <span data-ttu-id="66659-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="66659-108">Property</span></span>     | <span data-ttu-id="66659-109">Typ</span><span class="sxs-lookup"><span data-stu-id="66659-109">Type</span></span>   |<span data-ttu-id="66659-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66659-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66659-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="66659-111">activityDomain</span></span>|<span data-ttu-id="66659-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="66659-112">activityDomain</span></span>|<span data-ttu-id="66659-113">Die Art der Aktivität, optional.</span><span class="sxs-lookup"><span data-stu-id="66659-113">The nature of the activity, optional.</span></span> <span data-ttu-id="66659-114">Mögliche Werte sind: `work`, `personal`, `unrestricted`oder `unknown`.</span><span class="sxs-lookup"><span data-stu-id="66659-114">Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="66659-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="66659-115">timeslots</span></span>|<span data-ttu-id="66659-116">[timeSlot](timeslot.md) collection</span><span class="sxs-lookup"><span data-stu-id="66659-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="66659-117">Ein Array von Zeitfenstern</span><span class="sxs-lookup"><span data-stu-id="66659-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeconstraint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->