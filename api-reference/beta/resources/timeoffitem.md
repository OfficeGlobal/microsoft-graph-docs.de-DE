---
title: timeOffItem-Ressourcentyp
description: Stellt eine Version von timeOff dar.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c83a8725a0048a622ed88ec8265be76c30e46cc0
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657854"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="5dbd7-103">timeOffItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5dbd7-103">timeOffItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dbd7-104">Stellt eine Version von [timeOFF](timeoff.md)dar.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-104">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5dbd7-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5dbd7-105">Properties</span></span>
| <span data-ttu-id="5dbd7-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5dbd7-106">Property</span></span>                         | <span data-ttu-id="5dbd7-107">Typ</span><span class="sxs-lookup"><span data-stu-id="5dbd7-107">Type</span></span>                    | <span data-ttu-id="5dbd7-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5dbd7-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="5dbd7-109">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="5dbd7-109">timeOffReasonId</span></span>               | `string`                  | <span data-ttu-id="5dbd7-110">ID des `timeOffReason` for this `timeOffItem`.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-110">ID of the `timeOffReason` for this `timeOffItem`.</span></span> <span data-ttu-id="5dbd7-111">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-111">Required.</span></span>     |
| <span data-ttu-id="5dbd7-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5dbd7-112">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="5dbd7-113">Startdatum und-Uhrzeit für `timeOffItem`.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-113">The start date and time for the `timeOffItem`.</span></span> <span data-ttu-id="5dbd7-114">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-114">Required.</span></span> <span data-ttu-id="5dbd7-115">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5dbd7-116">Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-116">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="5dbd7-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5dbd7-117">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="5dbd7-118">Enddatum und-Uhrzeit für `timeOffItem`.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-118">The end date and time for the `timeOffItem`.</span></span> <span data-ttu-id="5dbd7-119">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-119">Required.</span></span> <span data-ttu-id="5dbd7-120">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5dbd7-121">Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-121">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="5dbd7-122">theme</span><span class="sxs-lookup"><span data-stu-id="5dbd7-122">theme</span></span> | `enum`   | <span data-ttu-id="5dbd7-123">Unterstützte Farben: weiß; blau grün lila Rosa gelb grau DarkBlue Dunkelgrün DarkPurple darkPink; darkYellow.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-123">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5dbd7-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5dbd7-124">JSON representation</span></span>

<span data-ttu-id="5dbd7-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5dbd7-125">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffItem"
}-->
```json
{
  "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "startDateTime": "2019-03-11T07:00:00Z",
  "endDateTime": "2019-03-12T07:00:00Z",
  "theme": "pink"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoffitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
