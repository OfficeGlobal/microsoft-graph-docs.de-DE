---
title: Ressourcentyp teamsUserActivityCounts
description: Es folgt eine JSON-Darstellung der Ressource.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bcc0e9d1ed5c93c3d9f4ba97165d0413025a89cd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987524"
---
# <a name="teamsuseractivitycounts-resource-type"></a><span data-ttu-id="44692-103">Ressourcentyp teamsUserActivityCounts</span><span class="sxs-lookup"><span data-stu-id="44692-103">teamsUserActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="44692-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="44692-104">Properties</span></span>

| <span data-ttu-id="44692-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="44692-105">Property</span></span>            | <span data-ttu-id="44692-106">Typ</span><span class="sxs-lookup"><span data-stu-id="44692-106">Type</span></span>   |
| :------------------ | :----- |
| <span data-ttu-id="44692-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="44692-107">reportRefreshDate</span></span>   | <span data-ttu-id="44692-108">Datum</span><span class="sxs-lookup"><span data-stu-id="44692-108">Date</span></span>   |
| <span data-ttu-id="44692-109">reportDate</span><span class="sxs-lookup"><span data-stu-id="44692-109">reportDate</span></span>          | <span data-ttu-id="44692-110">Datum</span><span class="sxs-lookup"><span data-stu-id="44692-110">Date</span></span>   |
| <span data-ttu-id="44692-111">teamChatMessages</span><span class="sxs-lookup"><span data-stu-id="44692-111">teamChatMessages</span></span>    | <span data-ttu-id="44692-112">Int64</span><span class="sxs-lookup"><span data-stu-id="44692-112">Int64</span></span>  |
| <span data-ttu-id="44692-113">privateChatMessages</span><span class="sxs-lookup"><span data-stu-id="44692-113">privateChatMessages</span></span> | <span data-ttu-id="44692-114">Int64</span><span class="sxs-lookup"><span data-stu-id="44692-114">Int64</span></span>  |
| <span data-ttu-id="44692-115">Anrufe</span><span class="sxs-lookup"><span data-stu-id="44692-115">calls</span></span>               | <span data-ttu-id="44692-116">Int64</span><span class="sxs-lookup"><span data-stu-id="44692-116">Int64</span></span>  |
| <span data-ttu-id="44692-117">Besprechungen</span><span class="sxs-lookup"><span data-stu-id="44692-117">meetings</span></span>            | <span data-ttu-id="44692-118">Int64</span><span class="sxs-lookup"><span data-stu-id="44692-118">Int64</span></span>  |
| <span data-ttu-id="44692-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="44692-119">reportPeriod</span></span>        | <span data-ttu-id="44692-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="44692-120">String</span></span> |


## <a name="json-representation"></a><span data-ttu-id="44692-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="44692-121">JSON representation</span></span>

<span data-ttu-id="44692-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="44692-122">The following is a JSON representation of the resource.</span></span>

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
