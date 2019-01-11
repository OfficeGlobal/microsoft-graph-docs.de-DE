---
title: Ressourcentyp yammerActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: d7869869466dc785b92db23f8b574eb2e77dd786
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816401"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="e22e6-103">Ressourcentyp yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="e22e6-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e22e6-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e22e6-104">Properties</span></span>

| <span data-ttu-id="e22e6-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e22e6-105">Property</span></span>          | <span data-ttu-id="e22e6-106">Typ</span><span class="sxs-lookup"><span data-stu-id="e22e6-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="e22e6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e22e6-107">reportRefreshDate</span></span> | <span data-ttu-id="e22e6-108">Datum</span><span class="sxs-lookup"><span data-stu-id="e22e6-108">Date</span></span>              |
| <span data-ttu-id="e22e6-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e22e6-109">userPrincipalName</span></span> | <span data-ttu-id="e22e6-110">String</span><span class="sxs-lookup"><span data-stu-id="e22e6-110">String</span></span>            |
| <span data-ttu-id="e22e6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e22e6-111">displayName</span></span>       | <span data-ttu-id="e22e6-112">String</span><span class="sxs-lookup"><span data-stu-id="e22e6-112">String</span></span>            |
| <span data-ttu-id="e22e6-113">userState</span><span class="sxs-lookup"><span data-stu-id="e22e6-113">userState</span></span>         | <span data-ttu-id="e22e6-114">String</span><span class="sxs-lookup"><span data-stu-id="e22e6-114">String</span></span>            |
| <span data-ttu-id="e22e6-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="e22e6-115">stateChangeDate</span></span>   | <span data-ttu-id="e22e6-116">Datum</span><span class="sxs-lookup"><span data-stu-id="e22e6-116">Date</span></span>              |
| <span data-ttu-id="e22e6-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="e22e6-117">lastActivityDate</span></span>  | <span data-ttu-id="e22e6-118">Datum</span><span class="sxs-lookup"><span data-stu-id="e22e6-118">Date</span></span>              |
| <span data-ttu-id="e22e6-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="e22e6-119">postedCount</span></span>       | <span data-ttu-id="e22e6-120">Int64</span><span class="sxs-lookup"><span data-stu-id="e22e6-120">Int64</span></span>             |
| <span data-ttu-id="e22e6-121">readCount</span><span class="sxs-lookup"><span data-stu-id="e22e6-121">readCount</span></span>         | <span data-ttu-id="e22e6-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e22e6-122">Int64</span></span>             |
| <span data-ttu-id="e22e6-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="e22e6-123">likedCount</span></span>        | <span data-ttu-id="e22e6-124">Int64</span><span class="sxs-lookup"><span data-stu-id="e22e6-124">Int64</span></span>             |
| <span data-ttu-id="e22e6-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="e22e6-125">assignedProducts</span></span>  | <span data-ttu-id="e22e6-126">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="e22e6-126">String collection</span></span> |
| <span data-ttu-id="e22e6-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e22e6-127">reportPeriod</span></span>      | <span data-ttu-id="e22e6-128">String</span><span class="sxs-lookup"><span data-stu-id="e22e6-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="e22e6-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e22e6-129">JSON representation</span></span>

<span data-ttu-id="e22e6-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e22e6-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
