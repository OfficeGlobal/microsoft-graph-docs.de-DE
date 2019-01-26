---
title: Ressourcentyp yammerGroupsActivityDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c5b580f643686c27497fd24a6fe00c7750a6a938
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573263"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="38441-103">Ressourcentyp yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="38441-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="38441-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="38441-104">Properties</span></span>

| <span data-ttu-id="38441-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="38441-105">Property</span></span>           | <span data-ttu-id="38441-106">Typ</span><span class="sxs-lookup"><span data-stu-id="38441-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="38441-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="38441-107">reportRefreshDate</span></span>  | <span data-ttu-id="38441-108">Date</span><span class="sxs-lookup"><span data-stu-id="38441-108">Date</span></span>    |
| <span data-ttu-id="38441-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="38441-109">groupDisplayName</span></span>   | <span data-ttu-id="38441-110">String</span><span class="sxs-lookup"><span data-stu-id="38441-110">String</span></span>  |
| <span data-ttu-id="38441-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="38441-111">isDeleted</span></span>          | <span data-ttu-id="38441-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="38441-112">Boolean</span></span> |
| <span data-ttu-id="38441-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="38441-113">ownerPrincipalName</span></span> | <span data-ttu-id="38441-114">String</span><span class="sxs-lookup"><span data-stu-id="38441-114">String</span></span>  |
| <span data-ttu-id="38441-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="38441-115">lastActivityDate</span></span>   | <span data-ttu-id="38441-116">Date</span><span class="sxs-lookup"><span data-stu-id="38441-116">Date</span></span>    |
| <span data-ttu-id="38441-117">groupType</span><span class="sxs-lookup"><span data-stu-id="38441-117">groupType</span></span>          | <span data-ttu-id="38441-118">String</span><span class="sxs-lookup"><span data-stu-id="38441-118">String</span></span>  |
| <span data-ttu-id="38441-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="38441-119">office365Connected</span></span> | <span data-ttu-id="38441-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="38441-120">Boolean</span></span> |
| <span data-ttu-id="38441-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="38441-121">memberCount</span></span>        | <span data-ttu-id="38441-122">Int64</span><span class="sxs-lookup"><span data-stu-id="38441-122">Int64</span></span>   |
| <span data-ttu-id="38441-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="38441-123">postedCount</span></span>        | <span data-ttu-id="38441-124">Int64</span><span class="sxs-lookup"><span data-stu-id="38441-124">Int64</span></span>   |
| <span data-ttu-id="38441-125">readCount</span><span class="sxs-lookup"><span data-stu-id="38441-125">readCount</span></span>          | <span data-ttu-id="38441-126">Int64</span><span class="sxs-lookup"><span data-stu-id="38441-126">Int64</span></span>   |
| <span data-ttu-id="38441-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="38441-127">likedCount</span></span>         | <span data-ttu-id="38441-128">Int64</span><span class="sxs-lookup"><span data-stu-id="38441-128">Int64</span></span>   |
| <span data-ttu-id="38441-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="38441-129">reportPeriod</span></span>       | <span data-ttu-id="38441-130">String</span><span class="sxs-lookup"><span data-stu-id="38441-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="38441-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="38441-131">JSON representation</span></span>

<span data-ttu-id="38441-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="38441-132">The following is a JSON representation of the resource.</span></span>

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
