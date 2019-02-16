---
title: meetingTimeSlotDataModel-Ressourcentyp
description: Ein Zeitfenster
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: acbd08da5e15dd733c63c0141db5b58cee896666
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057378"
---
# <a name="meetingtimeslotdatamodel-resource-type"></a><span data-ttu-id="be098-103">meetingTimeSlotDataModel-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="be098-103">meetingTimeSlotDataModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be098-104">Stellt ein Zeitfenster für eine Besprechung dar.</span><span class="sxs-lookup"><span data-stu-id="be098-104">Represents a time slot for a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="be098-105">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="be098-105">JSON representation</span></span>

<span data-ttu-id="be098-106">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="be098-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSlotDataModel"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```
## <a name="properties"></a><span data-ttu-id="be098-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="be098-107">Properties</span></span>
| <span data-ttu-id="be098-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="be098-108">Property</span></span>     | <span data-ttu-id="be098-109">Typ</span><span class="sxs-lookup"><span data-stu-id="be098-109">Type</span></span>   |<span data-ttu-id="be098-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="be098-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be098-111">end</span><span class="sxs-lookup"><span data-stu-id="be098-111">end</span></span>|[<span data-ttu-id="be098-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="be098-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="be098-113">Das Datum, die Uhrzeit und die Zeitzone, an denen ein Punkt beginnt.</span><span class="sxs-lookup"><span data-stu-id="be098-113">The date, time, and time zone that a period begins.</span></span> |
|<span data-ttu-id="be098-114">start</span><span class="sxs-lookup"><span data-stu-id="be098-114">start</span></span>|[<span data-ttu-id="be098-115">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="be098-115">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="be098-116">Das Datum, die Uhrzeit und die Zeitzone, die ein Punkt endet.</span><span class="sxs-lookup"><span data-stu-id="be098-116">The date, time, and time zone that a period ends.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSlotDataModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/meetingtimeslotdatamodel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->