---
title: Ressourcentyp teamsUserActivityUserDetail
description: Es folgt ein JSON-Darstellung der Ressource.
author: nkramer
ms.openlocfilehash: a1f47bc52c2a0a613598ce663f16023dce208c51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331941"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="23aa9-103">Ressourcentyp teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="23aa9-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="23aa9-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="23aa9-104">Properties</span></span>

| <span data-ttu-id="23aa9-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23aa9-105">Property</span></span>                | <span data-ttu-id="23aa9-106">Typ</span><span class="sxs-lookup"><span data-stu-id="23aa9-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="23aa9-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="23aa9-107">reportRefreshDate</span></span>       | <span data-ttu-id="23aa9-108">Datum</span><span class="sxs-lookup"><span data-stu-id="23aa9-108">Date</span></span>              |
| <span data-ttu-id="23aa9-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="23aa9-109">userPrincipalName</span></span>       | <span data-ttu-id="23aa9-110">String</span><span class="sxs-lookup"><span data-stu-id="23aa9-110">String</span></span>            |
| <span data-ttu-id="23aa9-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="23aa9-111">lastActivityDate</span></span>        | <span data-ttu-id="23aa9-112">Datum</span><span class="sxs-lookup"><span data-stu-id="23aa9-112">Date</span></span>              |
| <span data-ttu-id="23aa9-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="23aa9-113">isDeleted</span></span>               | <span data-ttu-id="23aa9-114">Boolesch</span><span class="sxs-lookup"><span data-stu-id="23aa9-114">Boolean</span></span>           |
| <span data-ttu-id="23aa9-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="23aa9-115">deletedDate</span></span>             | <span data-ttu-id="23aa9-116">Datum</span><span class="sxs-lookup"><span data-stu-id="23aa9-116">Date</span></span>              |
| <span data-ttu-id="23aa9-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="23aa9-117">assignedProducts</span></span>        | <span data-ttu-id="23aa9-118">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="23aa9-118">String collection</span></span> |
| <span data-ttu-id="23aa9-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="23aa9-119">teamChatMessageCount</span></span>    | <span data-ttu-id="23aa9-120">Int64</span><span class="sxs-lookup"><span data-stu-id="23aa9-120">Int64</span></span>             |
| <span data-ttu-id="23aa9-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="23aa9-121">privateChatMessageCount</span></span> | <span data-ttu-id="23aa9-122">Int64</span><span class="sxs-lookup"><span data-stu-id="23aa9-122">Int64</span></span>             |
| <span data-ttu-id="23aa9-123">callCount</span><span class="sxs-lookup"><span data-stu-id="23aa9-123">callCount</span></span>               | <span data-ttu-id="23aa9-124">Int64</span><span class="sxs-lookup"><span data-stu-id="23aa9-124">Int64</span></span>             |
| <span data-ttu-id="23aa9-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="23aa9-125">meetingCount</span></span>            | <span data-ttu-id="23aa9-126">Int64</span><span class="sxs-lookup"><span data-stu-id="23aa9-126">Int64</span></span>             |
| <span data-ttu-id="23aa9-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="23aa9-127">hasOtherAction</span></span>          | <span data-ttu-id="23aa9-128">Boolesch</span><span class="sxs-lookup"><span data-stu-id="23aa9-128">Boolean</span></span>           |
| <span data-ttu-id="23aa9-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="23aa9-129">reportPeriod</span></span>            | <span data-ttu-id="23aa9-130">String</span><span class="sxs-lookup"><span data-stu-id="23aa9-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="23aa9-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="23aa9-131">JSON representation</span></span>

<span data-ttu-id="23aa9-132">Es folgt ein JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="23aa9-132">The following is a JSON representaion of the resource.</span></span>

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
