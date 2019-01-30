---
title: Ressourcentyp „timeConstraint“
description: Schränkt Vorschläge für Besprechungstermine entsprechend der angegebenen Art der Aktivität und der offenen Zeitfenster auf bestimmte Stunden und Tage der Woche ein.
localization_priority: Normal
ms.openlocfilehash: 88035d0617523c51bb01ee0a467e8c84785ad6aa
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643566"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="6a74a-103">Ressourcentyp „timeConstraint“</span><span class="sxs-lookup"><span data-stu-id="6a74a-103">timeConstraint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a74a-104">Schränkt Vorschläge für Besprechungstermine entsprechend der angegebenen Art der Aktivität und der offenen Zeitfenster auf bestimmte Stunden und Tage der Woche ein.</span><span class="sxs-lookup"><span data-stu-id="6a74a-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a74a-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6a74a-105">JSON representation</span></span>

<span data-ttu-id="6a74a-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6a74a-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeconstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="6a74a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6a74a-107">Properties</span></span>
| <span data-ttu-id="6a74a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6a74a-108">Property</span></span>     | <span data-ttu-id="6a74a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="6a74a-109">Type</span></span>   |<span data-ttu-id="6a74a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a74a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a74a-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="6a74a-111">activityDomain</span></span>|<span data-ttu-id="6a74a-112">String</span><span class="sxs-lookup"><span data-stu-id="6a74a-112">String</span></span>|<span data-ttu-id="6a74a-p101">Die Art der Aktivität. Diese Angabe ist optional. Mögliche Werte sind: `work`, `personal`, `unrestricted` oder `unknown`.</span><span class="sxs-lookup"><span data-stu-id="6a74a-p101">The nature of the activity, optional. Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="6a74a-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="6a74a-115">timeslots</span></span>|<span data-ttu-id="6a74a-116">[timeSlot](timeslot.md) collection</span><span class="sxs-lookup"><span data-stu-id="6a74a-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="6a74a-117">Ein Array von Zeitfenstern</span><span class="sxs-lookup"><span data-stu-id="6a74a-117">An array of time periods.</span></span>|

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
