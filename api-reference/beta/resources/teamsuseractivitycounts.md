---
title: Ressourcentyp teamsUserActivityCounts
description: Es folgt eine JSON-Darstellung der Ressource.
author: nkramer
ms.openlocfilehash: f67540f4172993b1076d9590438262b0d4da1846
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334517"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="216ad-103">Ressourcentyp teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="216ad-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="216ad-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="216ad-104">Properties</span></span>

| <span data-ttu-id="216ad-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="216ad-105">Property</span></span>            | <span data-ttu-id="216ad-106">Typ</span><span class="sxs-lookup"><span data-stu-id="216ad-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="216ad-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="216ad-107">reportRefreshDate</span></span>   | <span data-ttu-id="216ad-108">Datum</span><span class="sxs-lookup"><span data-stu-id="216ad-108">Date</span></span>   |
| <span data-ttu-id="216ad-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="216ad-109">reportDate</span></span>          | <span data-ttu-id="216ad-110">Datum</span><span class="sxs-lookup"><span data-stu-id="216ad-110">Date</span></span>   |
| <span data-ttu-id="216ad-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="216ad-111">teamChatMessages</span></span>    | <span data-ttu-id="216ad-112">Int64</span><span class="sxs-lookup"><span data-stu-id="216ad-112">Int64</span></span>  |
| <span data-ttu-id="216ad-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="216ad-113">privateChatMessages</span></span> | <span data-ttu-id="216ad-114">Int64</span><span class="sxs-lookup"><span data-stu-id="216ad-114">Int64</span></span>  |
| <span data-ttu-id="216ad-115">Anrufe</span><span class="sxs-lookup"><span data-stu-id="216ad-115">calls</span></span>               | <span data-ttu-id="216ad-116">Int64</span><span class="sxs-lookup"><span data-stu-id="216ad-116">Int64</span></span>  |
| <span data-ttu-id="216ad-117">Besprechungen</span><span class="sxs-lookup"><span data-stu-id="216ad-117">meetings</span></span>            | <span data-ttu-id="216ad-118">Int64</span><span class="sxs-lookup"><span data-stu-id="216ad-118">Int64</span></span>  |
| <span data-ttu-id="216ad-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="216ad-119">reportPeriod</span></span>        | <span data-ttu-id="216ad-120">String</span><span class="sxs-lookup"><span data-stu-id="216ad-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="216ad-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="216ad-121">JSON representation</span></span>

<span data-ttu-id="216ad-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="216ad-122">The following is a JSON representation of the resource.</span></span>

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
