---
title: findMeetingTimesTimeConstraints-Ressourcentyp
description: Schränkt Vorschläge für Besprechungstermine entsprechend der angegebenen Art der Aktivität und der offenen Zeitfenster auf bestimmte Stunden und Tage der Woche ein.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e5790faf49fea03040dca05d457fededf5fdd683
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057386"
---
# <a name="findmeetingtimestimeconstraints-resource-type"></a><span data-ttu-id="1414f-103">findMeetingTimesTimeConstraints-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1414f-103">findMeetingTimesTimeConstraints resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1414f-104">Schränkt die Vorschläge für Besprechungszeiten auf die Art der Aktivität und bestimmte Zeiträume ein. |</span><span class="sxs-lookup"><span data-stu-id="1414f-104">Restricts meeting time suggestions to the nature of activity and certain ranges of time.|</span></span>

## <a name="json-representation"></a><span data-ttu-id="1414f-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1414f-105">JSON representation</span></span>

<span data-ttu-id="1414f-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1414f-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.findMeetingTimesTimeConstraints"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="1414f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1414f-107">Properties</span></span>
| <span data-ttu-id="1414f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1414f-108">Property</span></span>     | <span data-ttu-id="1414f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="1414f-109">Type</span></span>   |<span data-ttu-id="1414f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1414f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1414f-111">activityDomain</span><span class="sxs-lookup"><span data-stu-id="1414f-111">activityDomain</span></span>|<span data-ttu-id="1414f-112">activityDomain</span><span class="sxs-lookup"><span data-stu-id="1414f-112">activityDomain</span></span>|<span data-ttu-id="1414f-p101">Die Art der Aktivität. Diese Angabe ist optional. Mögliche Werte sind: `work`, `personal`, `unrestricted` oder `unknown`.</span><span class="sxs-lookup"><span data-stu-id="1414f-p101">The nature of the activity, optional. Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="1414f-115">timeslots</span><span class="sxs-lookup"><span data-stu-id="1414f-115">timeslots</span></span>|<span data-ttu-id="1414f-116">[searchWindowTimeSlot](searchwindowtimeslot.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="1414f-116">[searchWindowTimeSlot](searchwindowtimeslot.md) collection</span></span>|<span data-ttu-id="1414f-117">Ein Array von Zeitbereichen, in denen nach möglichen Besprechungszeiten gesucht werden soll.</span><span class="sxs-lookup"><span data-stu-id="1414f-117">An array of time ranges to look into for possible meeting times.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "findMeetingTimesTimeConstraints resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/findmeetingtimestimeconstraints.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->