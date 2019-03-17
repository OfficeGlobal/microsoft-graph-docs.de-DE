---
title: shiftItem-Ressourcentyp
description: Ein shiftItem stellt eine Version der Schicht dar.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7ff829ca0f43124404b4b99b048c9919368b6009
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657707"
---
# <a name="shiftitem-resource-type"></a><span data-ttu-id="dc670-103">shiftItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dc670-103">shiftItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc670-104">Stellt eine Version einer [Schicht](shift.md)dar.</span><span class="sxs-lookup"><span data-stu-id="dc670-104">Represents a version of a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dc670-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dc670-105">Properties</span></span>
| <span data-ttu-id="dc670-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dc670-106">Property</span></span>                         | <span data-ttu-id="dc670-107">Typ</span><span class="sxs-lookup"><span data-stu-id="dc670-107">Type</span></span>                    | <span data-ttu-id="dc670-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dc670-108">Description</span></span>                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="dc670-109">notes</span><span class="sxs-lookup"><span data-stu-id="dc670-109">notes</span></span>               | `string`                  | <span data-ttu-id="dc670-110">Die Hinweise für `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="dc670-110">The notes for the `shiftItem`.</span></span>      |
| <span data-ttu-id="dc670-111">displayName</span><span class="sxs-lookup"><span data-stu-id="dc670-111">displayName</span></span>               | `string`                  | <span data-ttu-id="dc670-112">Der Name des `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="dc670-112">The name of the `shiftItem`.</span></span> |
| <span data-ttu-id="dc670-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="dc670-113">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="dc670-114">Startdatum und-Uhrzeit für `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="dc670-114">The start date and time for the `shiftItem`.</span></span> <span data-ttu-id="dc670-115">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="dc670-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="dc670-116">Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="dc670-116">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="dc670-117">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dc670-117">Required.</span></span> |
| <span data-ttu-id="dc670-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="dc670-118">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="dc670-119">Enddatum und-Uhrzeit für `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="dc670-119">The end date and time for the `shiftItem`.</span></span> <span data-ttu-id="dc670-120">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dc670-120">Required.</span></span> <span data-ttu-id="dc670-121">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="dc670-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="dc670-122">Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="dc670-122">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="dc670-123">theme</span><span class="sxs-lookup"><span data-stu-id="dc670-123">theme</span></span> | `enum`   |    |  |  | <span data-ttu-id="dc670-124">Unterstützte Farben: weiß; blau grün lila Rosa gelb grau DarkBlue Dunkelgrün DarkPurple darkPink; darkYellow.</span><span class="sxs-lookup"><span data-stu-id="dc670-124">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |
| <span data-ttu-id="dc670-125">Aktivitäten</span><span class="sxs-lookup"><span data-stu-id="dc670-125">activities</span></span>    | `collection([shiftActivity](shiftactivity.md))`    | <span data-ttu-id="dc670-126">Ein inkrementeller Teil einer Schicht, der Details darüber abdecken kann, wann und wo sich ein Mitarbeiter während seiner Schicht befindet.</span><span class="sxs-lookup"><span data-stu-id="dc670-126">An incremental part of a shift which can cover details of when and where an employee is during their shift.</span></span> <span data-ttu-id="dc670-127">Zum Beispiel eine Zuordnung oder eine geplante Unterbrechung oder Mittagessen.</span><span class="sxs-lookup"><span data-stu-id="dc670-127">For example, an assignment or a scheduled break or lunch.</span></span> <span data-ttu-id="dc670-128">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="dc670-128">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dc670-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dc670-129">JSON representation</span></span>

<span data-ttu-id="dc670-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dc670-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftItem"
}-->
```json
{
  "displayName": "Day shift",
  "notes": "Please do inventory as part of your shift.",
  "startDateTime": "2019-03-11T15:00:00Z",
  "endDateTime": "2019-03-12T00:00:00Z",
  "theme": "blue",
  "activities": [
    {
      "isPaid": true,
      "startDateTime": "2019-03-11T15:00:00Z",
      "endDateTime": "2019-03-11T15:15:00Z",
      "code": "",
      "displayName": "Lunch"
    }
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/shiftitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
