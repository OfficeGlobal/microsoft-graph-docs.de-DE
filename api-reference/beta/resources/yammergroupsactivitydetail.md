---
title: Ressourcentyp yammerGroupsActivityDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 9e4ac61f2af69b4229c2e9c3df7c653428cc2033
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832032"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="6306a-103">Ressourcentyp yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="6306a-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6306a-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6306a-104">Properties</span></span>

| <span data-ttu-id="6306a-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6306a-105">Property</span></span>           | <span data-ttu-id="6306a-106">Typ</span><span class="sxs-lookup"><span data-stu-id="6306a-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="6306a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6306a-107">reportRefreshDate</span></span>  | <span data-ttu-id="6306a-108">Datum</span><span class="sxs-lookup"><span data-stu-id="6306a-108">Date</span></span>    |
| <span data-ttu-id="6306a-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="6306a-109">groupDisplayName</span></span>   | <span data-ttu-id="6306a-110">String</span><span class="sxs-lookup"><span data-stu-id="6306a-110">String</span></span>  |
| <span data-ttu-id="6306a-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="6306a-111">isDeleted</span></span>          | <span data-ttu-id="6306a-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="6306a-112">Boolean</span></span> |
| <span data-ttu-id="6306a-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6306a-113">ownerPrincipalName</span></span> | <span data-ttu-id="6306a-114">String</span><span class="sxs-lookup"><span data-stu-id="6306a-114">String</span></span>  |
| <span data-ttu-id="6306a-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="6306a-115">lastActivityDate</span></span>   | <span data-ttu-id="6306a-116">Datum</span><span class="sxs-lookup"><span data-stu-id="6306a-116">Date</span></span>    |
| <span data-ttu-id="6306a-117">groupType</span><span class="sxs-lookup"><span data-stu-id="6306a-117">groupType</span></span>          | <span data-ttu-id="6306a-118">String</span><span class="sxs-lookup"><span data-stu-id="6306a-118">String</span></span>  |
| <span data-ttu-id="6306a-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="6306a-119">office365Connected</span></span> | <span data-ttu-id="6306a-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="6306a-120">Boolean</span></span> |
| <span data-ttu-id="6306a-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="6306a-121">memberCount</span></span>        | <span data-ttu-id="6306a-122">Int64</span><span class="sxs-lookup"><span data-stu-id="6306a-122">Int64</span></span>   |
| <span data-ttu-id="6306a-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="6306a-123">postedCount</span></span>        | <span data-ttu-id="6306a-124">Int64</span><span class="sxs-lookup"><span data-stu-id="6306a-124">Int64</span></span>   |
| <span data-ttu-id="6306a-125">readCount</span><span class="sxs-lookup"><span data-stu-id="6306a-125">readCount</span></span>          | <span data-ttu-id="6306a-126">Int64</span><span class="sxs-lookup"><span data-stu-id="6306a-126">Int64</span></span>   |
| <span data-ttu-id="6306a-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="6306a-127">likedCount</span></span>         | <span data-ttu-id="6306a-128">Int64</span><span class="sxs-lookup"><span data-stu-id="6306a-128">Int64</span></span>   |
| <span data-ttu-id="6306a-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6306a-129">reportPeriod</span></span>       | <span data-ttu-id="6306a-130">String</span><span class="sxs-lookup"><span data-stu-id="6306a-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="6306a-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6306a-131">JSON representation</span></span>

<span data-ttu-id="6306a-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6306a-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "office365Connected": true, 
  "memberCount": 1024, 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "reportPeriod": "String"
}
```
