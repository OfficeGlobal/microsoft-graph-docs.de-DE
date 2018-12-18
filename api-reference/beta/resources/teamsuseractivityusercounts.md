---
title: Ressourcentyp teamsUserActivityUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
author: nkramer
ms.openlocfilehash: f4e10f1e34d4c6bdbed83279b98632c504630bc7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330457"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="e103d-103">Ressourcentyp teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="e103d-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e103d-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e103d-104">Properties</span></span>

| <span data-ttu-id="e103d-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e103d-105">Property</span></span>            | <span data-ttu-id="e103d-106">Typ</span><span class="sxs-lookup"><span data-stu-id="e103d-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="e103d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e103d-107">reportRefreshDate</span></span>   | <span data-ttu-id="e103d-108">Datum</span><span class="sxs-lookup"><span data-stu-id="e103d-108">Date</span></span>   |
| <span data-ttu-id="e103d-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="e103d-109">reportDate</span></span>          | <span data-ttu-id="e103d-110">Datum</span><span class="sxs-lookup"><span data-stu-id="e103d-110">Date</span></span>   |
| <span data-ttu-id="e103d-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="e103d-111">teamChatMessages</span></span>    | <span data-ttu-id="e103d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e103d-112">Int64</span></span>  |
| <span data-ttu-id="e103d-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="e103d-113">privateChatMessages</span></span> | <span data-ttu-id="e103d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="e103d-114">Int64</span></span>  |
| <span data-ttu-id="e103d-115">Anrufe</span><span class="sxs-lookup"><span data-stu-id="e103d-115">calls</span></span>               | <span data-ttu-id="e103d-116">Int64</span><span class="sxs-lookup"><span data-stu-id="e103d-116">Int64</span></span>  |
| <span data-ttu-id="e103d-117">Besprechungen</span><span class="sxs-lookup"><span data-stu-id="e103d-117">meetings</span></span>            | <span data-ttu-id="e103d-118">Int64</span><span class="sxs-lookup"><span data-stu-id="e103d-118">Int64</span></span>  |
| <span data-ttu-id="e103d-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="e103d-119">otherActions</span></span>        | <span data-ttu-id="e103d-120">Int64</span><span class="sxs-lookup"><span data-stu-id="e103d-120">Int64</span></span>  |
| <span data-ttu-id="e103d-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e103d-121">reportPeriod</span></span>        | <span data-ttu-id="e103d-122">String</span><span class="sxs-lookup"><span data-stu-id="e103d-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e103d-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e103d-123">JSON representation</span></span>

<span data-ttu-id="e103d-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e103d-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "teamChatMessages": 1024, 
  "privateChatMessages": 1024, 
  "calls": 1024, 
  "meetings": 1024, 
  "otherActions": 1024, 
  "reportPeriod": "String"
}
```
