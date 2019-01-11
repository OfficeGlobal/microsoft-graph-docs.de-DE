---
title: Ressourcentyp „timeConstraint“
description: Schränkt Vorschläge für Besprechungstermine entsprechend der angegebenen Art der Aktivität und der offenen Zeitfenster auf bestimmte Stunden und Tage der Woche ein.
localization_priority: Normal
ms.openlocfilehash: b6e239abbd0d9f7b4f83df4a60625a2f88131476
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815092"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="71077-103">Ressourcentyp „timeConstraint“</span><span class="sxs-lookup"><span data-stu-id="71077-103">timeConstraint resource type</span></span>

<span data-ttu-id="71077-104">Schränkt Vorschläge für Besprechungstermine entsprechend der angegebenen Art der Aktivität und der offenen Zeitfenster auf bestimmte Stunden und Tage der Woche ein.</span><span class="sxs-lookup"><span data-stu-id="71077-104">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="71077-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="71077-105">JSON representation</span></span>

<span data-ttu-id="71077-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="71077-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="71077-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="71077-107">Properties</span></span>
| <span data-ttu-id="71077-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71077-108">Property</span></span>     | <span data-ttu-id="71077-109">Typ</span><span class="sxs-lookup"><span data-stu-id="71077-109">Type</span></span>   |<span data-ttu-id="71077-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71077-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71077-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="71077-111">activityDomain</span></span>|<span data-ttu-id="71077-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="71077-112">activityDomain</span></span>|<span data-ttu-id="71077-113">Die Art der Aktivität, optional.</span><span class="sxs-lookup"><span data-stu-id="71077-113">The nature of the activity, optional.</span></span> <span data-ttu-id="71077-114">Die möglichen Werte sind: `work`, `personal`, `unrestricted`, oder `unknown`.</span><span class="sxs-lookup"><span data-stu-id="71077-114">The possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="71077-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="71077-115">timeslots</span></span>|<span data-ttu-id="71077-116">[timeSlot](timeslot.md) collection</span><span class="sxs-lookup"><span data-stu-id="71077-116">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="71077-117">Ein Array von Zeitfenstern</span><span class="sxs-lookup"><span data-stu-id="71077-117">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
