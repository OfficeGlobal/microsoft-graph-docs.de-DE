---
title: Ressourcentyp teamsUserActivityUserDetail
description: Es folgt ein JSON-Darstellung der Ressource.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 32b611ee9ec01b0339389256b8c8dff9eac99fa9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913429"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="99926-103">Ressourcentyp teamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="99926-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="99926-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="99926-104">Properties</span></span>

| <span data-ttu-id="99926-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="99926-105">Property</span></span>                | <span data-ttu-id="99926-106">Typ</span><span class="sxs-lookup"><span data-stu-id="99926-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="99926-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="99926-107">reportRefreshDate</span></span>       | <span data-ttu-id="99926-108">Datum</span><span class="sxs-lookup"><span data-stu-id="99926-108">Date</span></span>              |
| <span data-ttu-id="99926-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="99926-109">userPrincipalName</span></span>       | <span data-ttu-id="99926-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="99926-110">String</span></span>            |
| <span data-ttu-id="99926-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="99926-111">lastActivityDate</span></span>        | <span data-ttu-id="99926-112">Datum</span><span class="sxs-lookup"><span data-stu-id="99926-112">Date</span></span>              |
| <span data-ttu-id="99926-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="99926-113">isDeleted</span></span>               | <span data-ttu-id="99926-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="99926-114">Boolean</span></span>           |
| <span data-ttu-id="99926-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="99926-115">deletedDate</span></span>             | <span data-ttu-id="99926-116">Datum</span><span class="sxs-lookup"><span data-stu-id="99926-116">Date</span></span>              |
| <span data-ttu-id="99926-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="99926-117">assignedProducts</span></span>        | <span data-ttu-id="99926-118">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="99926-118">String collection</span></span> |
| <span data-ttu-id="99926-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="99926-119">teamChatMessageCount</span></span>    | <span data-ttu-id="99926-120">Int64</span><span class="sxs-lookup"><span data-stu-id="99926-120">Int64</span></span>             |
| <span data-ttu-id="99926-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="99926-121">privateChatMessageCount</span></span> | <span data-ttu-id="99926-122">Int64</span><span class="sxs-lookup"><span data-stu-id="99926-122">Int64</span></span>             |
| <span data-ttu-id="99926-123">callCount</span><span class="sxs-lookup"><span data-stu-id="99926-123">callCount</span></span>               | <span data-ttu-id="99926-124">Int64</span><span class="sxs-lookup"><span data-stu-id="99926-124">Int64</span></span>             |
| <span data-ttu-id="99926-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="99926-125">meetingCount</span></span>            | <span data-ttu-id="99926-126">Int64</span><span class="sxs-lookup"><span data-stu-id="99926-126">Int64</span></span>             |
| <span data-ttu-id="99926-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="99926-127">hasOtherAction</span></span>          | <span data-ttu-id="99926-128">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="99926-128">Boolean</span></span>           |
| <span data-ttu-id="99926-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="99926-129">reportPeriod</span></span>            | <span data-ttu-id="99926-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="99926-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="99926-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="99926-131">JSON representation</span></span>

<span data-ttu-id="99926-132">Es folgt ein JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="99926-132">The following is a JSON representaion of the resource.</span></span>

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
