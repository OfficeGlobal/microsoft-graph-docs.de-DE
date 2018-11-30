---
title: Ressourcentyp teamsUserActivityCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 39e90b4c9dc6b9929959139ba67ddb090d143e38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064799"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="233ed-103">Ressourcentyp teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="233ed-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="233ed-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="233ed-104">Properties</span></span>

| <span data-ttu-id="233ed-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="233ed-105">Property</span></span>            | <span data-ttu-id="233ed-106">Typ</span><span class="sxs-lookup"><span data-stu-id="233ed-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="233ed-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="233ed-107">reportRefreshDate</span></span>   | <span data-ttu-id="233ed-108">Datum</span><span class="sxs-lookup"><span data-stu-id="233ed-108">Date</span></span>   |
| <span data-ttu-id="233ed-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="233ed-109">reportDate</span></span>          | <span data-ttu-id="233ed-110">Datum</span><span class="sxs-lookup"><span data-stu-id="233ed-110">Date</span></span>   |
| <span data-ttu-id="233ed-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="233ed-111">teamChatMessages</span></span>    | <span data-ttu-id="233ed-112">Int64</span><span class="sxs-lookup"><span data-stu-id="233ed-112">Int64</span></span>  |
| <span data-ttu-id="233ed-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="233ed-113">privateChatMessages</span></span> | <span data-ttu-id="233ed-114">Int64</span><span class="sxs-lookup"><span data-stu-id="233ed-114">Int64</span></span>  |
| <span data-ttu-id="233ed-115">Anrufe</span><span class="sxs-lookup"><span data-stu-id="233ed-115">calls</span></span>               | <span data-ttu-id="233ed-116">Int64</span><span class="sxs-lookup"><span data-stu-id="233ed-116">Int64</span></span>  |
| <span data-ttu-id="233ed-117">Besprechungen</span><span class="sxs-lookup"><span data-stu-id="233ed-117">meetings</span></span>            | <span data-ttu-id="233ed-118">Int64</span><span class="sxs-lookup"><span data-stu-id="233ed-118">Int64</span></span>  |
| <span data-ttu-id="233ed-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="233ed-119">reportPeriod</span></span>        | <span data-ttu-id="233ed-120">String</span><span class="sxs-lookup"><span data-stu-id="233ed-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="233ed-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="233ed-121">JSON representation</span></span>

<span data-ttu-id="233ed-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="233ed-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "reportPeriod": "String"
}
```
