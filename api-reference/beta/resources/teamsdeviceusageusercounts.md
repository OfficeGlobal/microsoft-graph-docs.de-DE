---
title: Ressourcentyp teamsDeviceUsageUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 671dfada02b9c16d3392d0a97023b82020fd1218
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987398"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="61392-103">Ressourcentyp teamsDeviceUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="61392-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="61392-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="61392-104">Properties</span></span>

| <span data-ttu-id="61392-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61392-105">Property</span></span>          | <span data-ttu-id="61392-106">Typ</span><span class="sxs-lookup"><span data-stu-id="61392-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="61392-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="61392-107">reportRefreshDate</span></span> | <span data-ttu-id="61392-108">Datum</span><span class="sxs-lookup"><span data-stu-id="61392-108">Date</span></span>   |
| <span data-ttu-id="61392-109">web</span><span class="sxs-lookup"><span data-stu-id="61392-109">web</span></span>               | <span data-ttu-id="61392-110">Int64</span><span class="sxs-lookup"><span data-stu-id="61392-110">Int64</span></span>  |
| <span data-ttu-id="61392-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="61392-111">windowsPhone</span></span>      | <span data-ttu-id="61392-112">Int64</span><span class="sxs-lookup"><span data-stu-id="61392-112">Int64</span></span>  |
| <span data-ttu-id="61392-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="61392-113">androidPhone</span></span>      | <span data-ttu-id="61392-114">Int64</span><span class="sxs-lookup"><span data-stu-id="61392-114">Int64</span></span>  |
| <span data-ttu-id="61392-115">IOS</span><span class="sxs-lookup"><span data-stu-id="61392-115">ios</span></span>               | <span data-ttu-id="61392-116">Int64</span><span class="sxs-lookup"><span data-stu-id="61392-116">Int64</span></span>  |
| <span data-ttu-id="61392-117">mac</span><span class="sxs-lookup"><span data-stu-id="61392-117">mac</span></span>               | <span data-ttu-id="61392-118">Int64</span><span class="sxs-lookup"><span data-stu-id="61392-118">Int64</span></span>  |
| <span data-ttu-id="61392-119">Windows</span><span class="sxs-lookup"><span data-stu-id="61392-119">windows</span></span>           | <span data-ttu-id="61392-120">Int64</span><span class="sxs-lookup"><span data-stu-id="61392-120">Int64</span></span>  |
| <span data-ttu-id="61392-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="61392-121">reportDate</span></span>        | <span data-ttu-id="61392-122">Datum</span><span class="sxs-lookup"><span data-stu-id="61392-122">Date</span></span>   |
| <span data-ttu-id="61392-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="61392-123">reportPeriod</span></span>      | <span data-ttu-id="61392-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="61392-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="61392-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="61392-125">JSON representation</span></span>

<span data-ttu-id="61392-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="61392-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
