---
title: Verschiebungs Ressourcentyp
description: Stellt eine Aktivität in einer Schicht dar.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0a5b877c2c24d1764e9badb44dab1f25143c2dce
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657525"
---
# <a name="shiftactivity-resource-type"></a><span data-ttu-id="49f72-103">Verschiebungs Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="49f72-103">shiftActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49f72-104">Stellt eine Aktivität in einer [Schicht](shift.md)dar.</span><span class="sxs-lookup"><span data-stu-id="49f72-104">Represents an activity in a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="49f72-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="49f72-105">Properties</span></span>
| <span data-ttu-id="49f72-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="49f72-106">Property</span></span>                         | <span data-ttu-id="49f72-107">Typ</span><span class="sxs-lookup"><span data-stu-id="49f72-107">Type</span></span>                    | <span data-ttu-id="49f72-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49f72-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="49f72-109">isPaid</span><span class="sxs-lookup"><span data-stu-id="49f72-109">isPaid</span></span>               | `bool`                  | <span data-ttu-id="49f72-110">Gibt an, `microsoft.graph.user` ob der für die Aktivität während des Vorgangs `shift`bezahlt werden soll.</span><span class="sxs-lookup"><span data-stu-id="49f72-110">Indicates whether the `microsoft.graph.user` should be paid for the activity during their `shift`.</span></span> <span data-ttu-id="49f72-111">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="49f72-111">Required.</span></span>    |
| <span data-ttu-id="49f72-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="49f72-112">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="49f72-113">Startdatum und-Uhrzeit für `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="49f72-113">The start date and time for the `shiftActivity`.</span></span> <span data-ttu-id="49f72-114">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="49f72-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="49f72-115">Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="49f72-115">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="49f72-116">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="49f72-116">Required.</span></span> |
| <span data-ttu-id="49f72-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="49f72-117">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="49f72-118">Enddatum und-Uhrzeit für `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="49f72-118">The end date and time for the `shiftActivity`.</span></span> <span data-ttu-id="49f72-119">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="49f72-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="49f72-120">Beispielsweise würde Mitternacht UTC am 1. Januar 2014 wie folgt aussehen: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="49f72-120">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="49f72-121">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="49f72-121">Required.</span></span>    |
| <span data-ttu-id="49f72-122">code</span><span class="sxs-lookup"><span data-stu-id="49f72-122">code</span></span>               | `string`                  | <span data-ttu-id="49f72-123">Vom `shiftActivity`Kunden definierter Code für.</span><span class="sxs-lookup"><span data-stu-id="49f72-123">Customer defined code for the `shiftActivity`.</span></span> <span data-ttu-id="49f72-124">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="49f72-124">Required.</span></span>    |
| <span data-ttu-id="49f72-125">displayName</span><span class="sxs-lookup"><span data-stu-id="49f72-125">displayName</span></span>               | `string`                  | <span data-ttu-id="49f72-126">Der Name des `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="49f72-126">The name of the `shiftActivity`.</span></span> <span data-ttu-id="49f72-127">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="49f72-127">Required.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="49f72-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="49f72-128">JSON representation</span></span>

<span data-ttu-id="49f72-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="49f72-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftActivity"
}-->
```json
{
  "isPaid": true,
  "startDateTime": "2019-03-11T15:00:00Z",
  "endDateTime": "2019-03-11T15:15:00Z",
  "code": "",
  "displayName": "Lunch"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/shiftactivity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
