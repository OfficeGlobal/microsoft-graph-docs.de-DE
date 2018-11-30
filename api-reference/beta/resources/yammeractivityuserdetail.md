---
title: Ressourcentyp yammerActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: a1ca33efe8327b1c1e52de25714df9c0bd45ee05
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064132"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="4ab22-103">Ressourcentyp yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="4ab22-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4ab22-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4ab22-104">Properties</span></span>

| <span data-ttu-id="4ab22-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4ab22-105">Property</span></span>          | <span data-ttu-id="4ab22-106">Typ</span><span class="sxs-lookup"><span data-stu-id="4ab22-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="4ab22-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4ab22-107">reportRefreshDate</span></span> | <span data-ttu-id="4ab22-108">Datum</span><span class="sxs-lookup"><span data-stu-id="4ab22-108">Date</span></span>              |
| <span data-ttu-id="4ab22-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4ab22-109">userPrincipalName</span></span> | <span data-ttu-id="4ab22-110">String</span><span class="sxs-lookup"><span data-stu-id="4ab22-110">String</span></span>            |
| <span data-ttu-id="4ab22-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4ab22-111">displayName</span></span>       | <span data-ttu-id="4ab22-112">String</span><span class="sxs-lookup"><span data-stu-id="4ab22-112">String</span></span>            |
| <span data-ttu-id="4ab22-113">userState</span><span class="sxs-lookup"><span data-stu-id="4ab22-113">userState</span></span>         | <span data-ttu-id="4ab22-114">String</span><span class="sxs-lookup"><span data-stu-id="4ab22-114">String</span></span>            |
| <span data-ttu-id="4ab22-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="4ab22-115">stateChangeDate</span></span>   | <span data-ttu-id="4ab22-116">Datum</span><span class="sxs-lookup"><span data-stu-id="4ab22-116">Date</span></span>              |
| <span data-ttu-id="4ab22-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="4ab22-117">lastActivityDate</span></span>  | <span data-ttu-id="4ab22-118">Datum</span><span class="sxs-lookup"><span data-stu-id="4ab22-118">Date</span></span>              |
| <span data-ttu-id="4ab22-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="4ab22-119">postedCount</span></span>       | <span data-ttu-id="4ab22-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4ab22-120">Int64</span></span>             |
| <span data-ttu-id="4ab22-121">readCount</span><span class="sxs-lookup"><span data-stu-id="4ab22-121">readCount</span></span>         | <span data-ttu-id="4ab22-122">Int64</span><span class="sxs-lookup"><span data-stu-id="4ab22-122">Int64</span></span>             |
| <span data-ttu-id="4ab22-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="4ab22-123">likedCount</span></span>        | <span data-ttu-id="4ab22-124">Int64</span><span class="sxs-lookup"><span data-stu-id="4ab22-124">Int64</span></span>             |
| <span data-ttu-id="4ab22-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="4ab22-125">assignedProducts</span></span>  | <span data-ttu-id="4ab22-126">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="4ab22-126">String collection</span></span> |
| <span data-ttu-id="4ab22-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4ab22-127">reportPeriod</span></span>      | <span data-ttu-id="4ab22-128">String</span><span class="sxs-lookup"><span data-stu-id="4ab22-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="4ab22-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4ab22-129">JSON representation</span></span>

<span data-ttu-id="4ab22-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4ab22-130">The following is a JSON representation of the resource.</span></span>

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
