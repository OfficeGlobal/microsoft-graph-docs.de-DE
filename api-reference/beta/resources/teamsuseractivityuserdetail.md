---
title: Ressourcentyp teamsUserActivityUserDetail
description: Es folgt ein JSON-Darstellung der Ressource.
ms.openlocfilehash: 4e40ea4adf07450e6b51555df47579955a2a0286
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064811"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="498c3-103">Ressourcentyp teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="498c3-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="498c3-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="498c3-104">Properties</span></span>

| <span data-ttu-id="498c3-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="498c3-105">Property</span></span>                | <span data-ttu-id="498c3-106">Typ</span><span class="sxs-lookup"><span data-stu-id="498c3-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="498c3-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="498c3-107">reportRefreshDate</span></span>       | <span data-ttu-id="498c3-108">Datum</span><span class="sxs-lookup"><span data-stu-id="498c3-108">Date</span></span>              |
| <span data-ttu-id="498c3-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="498c3-109">userPrincipalName</span></span>       | <span data-ttu-id="498c3-110">String</span><span class="sxs-lookup"><span data-stu-id="498c3-110">String</span></span>            |
| <span data-ttu-id="498c3-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="498c3-111">lastActivityDate</span></span>        | <span data-ttu-id="498c3-112">Datum</span><span class="sxs-lookup"><span data-stu-id="498c3-112">Date</span></span>              |
| <span data-ttu-id="498c3-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="498c3-113">isDeleted</span></span>               | <span data-ttu-id="498c3-114">Boolesch</span><span class="sxs-lookup"><span data-stu-id="498c3-114">Boolean</span></span>           |
| <span data-ttu-id="498c3-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="498c3-115">deletedDate</span></span>             | <span data-ttu-id="498c3-116">Datum</span><span class="sxs-lookup"><span data-stu-id="498c3-116">Date</span></span>              |
| <span data-ttu-id="498c3-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="498c3-117">assignedProducts</span></span>        | <span data-ttu-id="498c3-118">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="498c3-118">String collection</span></span> |
| <span data-ttu-id="498c3-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="498c3-119">teamChatMessageCount</span></span>    | <span data-ttu-id="498c3-120">Int64</span><span class="sxs-lookup"><span data-stu-id="498c3-120">Int64</span></span>             |
| <span data-ttu-id="498c3-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="498c3-121">privateChatMessageCount</span></span> | <span data-ttu-id="498c3-122">Int64</span><span class="sxs-lookup"><span data-stu-id="498c3-122">Int64</span></span>             |
| <span data-ttu-id="498c3-123">callCount</span><span class="sxs-lookup"><span data-stu-id="498c3-123">callCount</span></span>               | <span data-ttu-id="498c3-124">Int64</span><span class="sxs-lookup"><span data-stu-id="498c3-124">Int64</span></span>             |
| <span data-ttu-id="498c3-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="498c3-125">meetingCount</span></span>            | <span data-ttu-id="498c3-126">Int64</span><span class="sxs-lookup"><span data-stu-id="498c3-126">Int64</span></span>             |
| <span data-ttu-id="498c3-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="498c3-127">hasOtherAction</span></span>          | <span data-ttu-id="498c3-128">Boolesch</span><span class="sxs-lookup"><span data-stu-id="498c3-128">Boolean</span></span>           |
| <span data-ttu-id="498c3-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="498c3-129">reportPeriod</span></span>            | <span data-ttu-id="498c3-130">String</span><span class="sxs-lookup"><span data-stu-id="498c3-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="498c3-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="498c3-131">JSON representation</span></span>

<span data-ttu-id="498c3-132">Es folgt ein JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="498c3-132">The following is a JSON representaion of the resource.</span></span>

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
