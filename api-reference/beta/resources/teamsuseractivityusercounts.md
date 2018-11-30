---
title: Ressourcentyp teamsUserActivityUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: f6478175252e99af2bfe5561d29eebe75b638eb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059095"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="92ff4-103">Ressourcentyp teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="92ff4-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="92ff4-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="92ff4-104">Properties</span></span>

| <span data-ttu-id="92ff4-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="92ff4-105">Property</span></span>            | <span data-ttu-id="92ff4-106">Typ</span><span class="sxs-lookup"><span data-stu-id="92ff4-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="92ff4-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="92ff4-107">reportRefreshDate</span></span>   | <span data-ttu-id="92ff4-108">Datum</span><span class="sxs-lookup"><span data-stu-id="92ff4-108">Date</span></span>   |
| <span data-ttu-id="92ff4-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="92ff4-109">reportDate</span></span>          | <span data-ttu-id="92ff4-110">Datum</span><span class="sxs-lookup"><span data-stu-id="92ff4-110">Date</span></span>   |
| <span data-ttu-id="92ff4-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="92ff4-111">teamChatMessages</span></span>    | <span data-ttu-id="92ff4-112">Int64</span><span class="sxs-lookup"><span data-stu-id="92ff4-112">Int64</span></span>  |
| <span data-ttu-id="92ff4-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="92ff4-113">privateChatMessages</span></span> | <span data-ttu-id="92ff4-114">Int64</span><span class="sxs-lookup"><span data-stu-id="92ff4-114">Int64</span></span>  |
| <span data-ttu-id="92ff4-115">Anrufe</span><span class="sxs-lookup"><span data-stu-id="92ff4-115">calls</span></span>               | <span data-ttu-id="92ff4-116">Int64</span><span class="sxs-lookup"><span data-stu-id="92ff4-116">Int64</span></span>  |
| <span data-ttu-id="92ff4-117">Besprechungen</span><span class="sxs-lookup"><span data-stu-id="92ff4-117">meetings</span></span>            | <span data-ttu-id="92ff4-118">Int64</span><span class="sxs-lookup"><span data-stu-id="92ff4-118">Int64</span></span>  |
| <span data-ttu-id="92ff4-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="92ff4-119">otherActions</span></span>        | <span data-ttu-id="92ff4-120">Int64</span><span class="sxs-lookup"><span data-stu-id="92ff4-120">Int64</span></span>  |
| <span data-ttu-id="92ff4-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="92ff4-121">reportPeriod</span></span>        | <span data-ttu-id="92ff4-122">String</span><span class="sxs-lookup"><span data-stu-id="92ff4-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="92ff4-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="92ff4-123">JSON representation</span></span>

<span data-ttu-id="92ff4-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="92ff4-124">The following is a JSON representation of the resource.</span></span>

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
