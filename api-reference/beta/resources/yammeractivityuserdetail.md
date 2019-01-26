---
title: Ressourcentyp yammerActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: eea520e6024bb050001461fb5ada5c90ea2b2125
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575828"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="307f0-103">Ressourcentyp yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="307f0-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="307f0-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="307f0-104">Properties</span></span>

| <span data-ttu-id="307f0-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="307f0-105">Property</span></span>          | <span data-ttu-id="307f0-106">Typ</span><span class="sxs-lookup"><span data-stu-id="307f0-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="307f0-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="307f0-107">reportRefreshDate</span></span> | <span data-ttu-id="307f0-108">Date</span><span class="sxs-lookup"><span data-stu-id="307f0-108">Date</span></span>              |
| <span data-ttu-id="307f0-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="307f0-109">userPrincipalName</span></span> | <span data-ttu-id="307f0-110">String</span><span class="sxs-lookup"><span data-stu-id="307f0-110">String</span></span>            |
| <span data-ttu-id="307f0-111">displayName</span><span class="sxs-lookup"><span data-stu-id="307f0-111">displayName</span></span>       | <span data-ttu-id="307f0-112">String</span><span class="sxs-lookup"><span data-stu-id="307f0-112">String</span></span>            |
| <span data-ttu-id="307f0-113">userState</span><span class="sxs-lookup"><span data-stu-id="307f0-113">userState</span></span>         | <span data-ttu-id="307f0-114">String</span><span class="sxs-lookup"><span data-stu-id="307f0-114">String</span></span>            |
| <span data-ttu-id="307f0-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="307f0-115">stateChangeDate</span></span>   | <span data-ttu-id="307f0-116">Date</span><span class="sxs-lookup"><span data-stu-id="307f0-116">Date</span></span>              |
| <span data-ttu-id="307f0-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="307f0-117">lastActivityDate</span></span>  | <span data-ttu-id="307f0-118">Date</span><span class="sxs-lookup"><span data-stu-id="307f0-118">Date</span></span>              |
| <span data-ttu-id="307f0-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="307f0-119">postedCount</span></span>       | <span data-ttu-id="307f0-120">Int64</span><span class="sxs-lookup"><span data-stu-id="307f0-120">Int64</span></span>             |
| <span data-ttu-id="307f0-121">readCount</span><span class="sxs-lookup"><span data-stu-id="307f0-121">readCount</span></span>         | <span data-ttu-id="307f0-122">Int64</span><span class="sxs-lookup"><span data-stu-id="307f0-122">Int64</span></span>             |
| <span data-ttu-id="307f0-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="307f0-123">likedCount</span></span>        | <span data-ttu-id="307f0-124">Int64</span><span class="sxs-lookup"><span data-stu-id="307f0-124">Int64</span></span>             |
| <span data-ttu-id="307f0-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="307f0-125">assignedProducts</span></span>  | <span data-ttu-id="307f0-126">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="307f0-126">String collection</span></span> |
| <span data-ttu-id="307f0-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="307f0-127">reportPeriod</span></span>      | <span data-ttu-id="307f0-128">String</span><span class="sxs-lookup"><span data-stu-id="307f0-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="307f0-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="307f0-129">JSON representation</span></span>

<span data-ttu-id="307f0-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="307f0-130">The following is a JSON representation of the resource.</span></span>

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
