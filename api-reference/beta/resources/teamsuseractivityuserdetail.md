---
title: Ressourcentyp teamsUserActivityUserDetail
description: Es folgt ein JSON-Darstellung der Ressource.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 2e3f64c7065343712f6a9d9c6a114bf95f24c171
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823653"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="f02b1-103">Ressourcentyp teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="f02b1-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f02b1-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f02b1-104">Properties</span></span>

| <span data-ttu-id="f02b1-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f02b1-105">Property</span></span>                | <span data-ttu-id="f02b1-106">Typ</span><span class="sxs-lookup"><span data-stu-id="f02b1-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="f02b1-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f02b1-107">reportRefreshDate</span></span>       | <span data-ttu-id="f02b1-108">Datum</span><span class="sxs-lookup"><span data-stu-id="f02b1-108">Date</span></span>              |
| <span data-ttu-id="f02b1-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f02b1-109">userPrincipalName</span></span>       | <span data-ttu-id="f02b1-110">String</span><span class="sxs-lookup"><span data-stu-id="f02b1-110">String</span></span>            |
| <span data-ttu-id="f02b1-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="f02b1-111">lastActivityDate</span></span>        | <span data-ttu-id="f02b1-112">Datum</span><span class="sxs-lookup"><span data-stu-id="f02b1-112">Date</span></span>              |
| <span data-ttu-id="f02b1-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f02b1-113">isDeleted</span></span>               | <span data-ttu-id="f02b1-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f02b1-114">Boolean</span></span>           |
| <span data-ttu-id="f02b1-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="f02b1-115">deletedDate</span></span>             | <span data-ttu-id="f02b1-116">Datum</span><span class="sxs-lookup"><span data-stu-id="f02b1-116">Date</span></span>              |
| <span data-ttu-id="f02b1-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="f02b1-117">assignedProducts</span></span>        | <span data-ttu-id="f02b1-118">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="f02b1-118">String collection</span></span> |
| <span data-ttu-id="f02b1-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="f02b1-119">teamChatMessageCount</span></span>    | <span data-ttu-id="f02b1-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f02b1-120">Int64</span></span>             |
| <span data-ttu-id="f02b1-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="f02b1-121">privateChatMessageCount</span></span> | <span data-ttu-id="f02b1-122">Int64</span><span class="sxs-lookup"><span data-stu-id="f02b1-122">Int64</span></span>             |
| <span data-ttu-id="f02b1-123">callCount</span><span class="sxs-lookup"><span data-stu-id="f02b1-123">callCount</span></span>               | <span data-ttu-id="f02b1-124">Int64</span><span class="sxs-lookup"><span data-stu-id="f02b1-124">Int64</span></span>             |
| <span data-ttu-id="f02b1-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="f02b1-125">meetingCount</span></span>            | <span data-ttu-id="f02b1-126">Int64</span><span class="sxs-lookup"><span data-stu-id="f02b1-126">Int64</span></span>             |
| <span data-ttu-id="f02b1-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="f02b1-127">hasOtherAction</span></span>          | <span data-ttu-id="f02b1-128">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f02b1-128">Boolean</span></span>           |
| <span data-ttu-id="f02b1-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f02b1-129">reportPeriod</span></span>            | <span data-ttu-id="f02b1-130">String</span><span class="sxs-lookup"><span data-stu-id="f02b1-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="f02b1-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f02b1-131">JSON representation</span></span>

<span data-ttu-id="f02b1-132">Es folgt ein JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f02b1-132">The following is a JSON representaion of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "assignedProducts": ["String"],
  "teamChatMessageCount": 1024, 
  "privateChatMessageCount": 1024, 
  "callCount": 1024, 
  "meetingCount": 1024, 
  "hasOtherAction": true, 
  "reportPeriod": "String"
}
```
