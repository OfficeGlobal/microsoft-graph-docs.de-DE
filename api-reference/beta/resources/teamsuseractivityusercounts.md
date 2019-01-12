---
title: Ressourcentyp teamsUserActivityUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcb69c09d621ce3cce006fd9130afa0a70e4cdb8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912820"
---
# <a name="teamsuseractivityusercounts-resource-type"></a><span data-ttu-id="2a864-103">Ressourcentyp teamsUserActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="2a864-103">teamsUserActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2a864-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2a864-104">Properties</span></span>

| <span data-ttu-id="2a864-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a864-105">Property</span></span>            | <span data-ttu-id="2a864-106">Typ</span><span class="sxs-lookup"><span data-stu-id="2a864-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="2a864-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2a864-107">reportRefreshDate</span></span>   | <span data-ttu-id="2a864-108">Datum</span><span class="sxs-lookup"><span data-stu-id="2a864-108">Date</span></span>   |
| <span data-ttu-id="2a864-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="2a864-109">reportDate</span></span>          | <span data-ttu-id="2a864-110">Datum</span><span class="sxs-lookup"><span data-stu-id="2a864-110">Date</span></span>   |
| <span data-ttu-id="2a864-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="2a864-111">teamChatMessages</span></span>    | <span data-ttu-id="2a864-112">Int64</span><span class="sxs-lookup"><span data-stu-id="2a864-112">Int64</span></span>  |
| <span data-ttu-id="2a864-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="2a864-113">privateChatMessages</span></span> | <span data-ttu-id="2a864-114">Int64</span><span class="sxs-lookup"><span data-stu-id="2a864-114">Int64</span></span>  |
| <span data-ttu-id="2a864-115">Anrufe</span><span class="sxs-lookup"><span data-stu-id="2a864-115">calls</span></span>               | <span data-ttu-id="2a864-116">Int64</span><span class="sxs-lookup"><span data-stu-id="2a864-116">Int64</span></span>  |
| <span data-ttu-id="2a864-117">Besprechungen</span><span class="sxs-lookup"><span data-stu-id="2a864-117">meetings</span></span>            | <span data-ttu-id="2a864-118">Int64</span><span class="sxs-lookup"><span data-stu-id="2a864-118">Int64</span></span>  |
| <span data-ttu-id="2a864-119">otherActions</span><span class="sxs-lookup"><span data-stu-id="2a864-119">otherActions</span></span>        | <span data-ttu-id="2a864-120">Int64</span><span class="sxs-lookup"><span data-stu-id="2a864-120">Int64</span></span>  |
| <span data-ttu-id="2a864-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2a864-121">reportPeriod</span></span>        | <span data-ttu-id="2a864-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2a864-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2a864-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2a864-123">JSON representation</span></span>

<span data-ttu-id="2a864-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2a864-124">The following is a JSON representation of the resource.</span></span>

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
