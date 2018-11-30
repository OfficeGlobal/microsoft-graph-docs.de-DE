---
title: Ressourcentyp yammerGroupsActivityDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 9a4bb00aecb2ae1d14b68a5388e0dedc7c41b1cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059110"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="b26ee-103">Ressourcentyp yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="b26ee-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b26ee-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b26ee-104">Properties</span></span>

| <span data-ttu-id="b26ee-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b26ee-105">Property</span></span>           | <span data-ttu-id="b26ee-106">Typ</span><span class="sxs-lookup"><span data-stu-id="b26ee-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="b26ee-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b26ee-107">reportRefreshDate</span></span>  | <span data-ttu-id="b26ee-108">Datum</span><span class="sxs-lookup"><span data-stu-id="b26ee-108">Date</span></span>    |
| <span data-ttu-id="b26ee-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="b26ee-109">groupDisplayName</span></span>   | <span data-ttu-id="b26ee-110">String</span><span class="sxs-lookup"><span data-stu-id="b26ee-110">String</span></span>  |
| <span data-ttu-id="b26ee-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="b26ee-111">isDeleted</span></span>          | <span data-ttu-id="b26ee-112">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b26ee-112">Boolean</span></span> |
| <span data-ttu-id="b26ee-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b26ee-113">ownerPrincipalName</span></span> | <span data-ttu-id="b26ee-114">String</span><span class="sxs-lookup"><span data-stu-id="b26ee-114">String</span></span>  |
| <span data-ttu-id="b26ee-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="b26ee-115">lastActivityDate</span></span>   | <span data-ttu-id="b26ee-116">Datum</span><span class="sxs-lookup"><span data-stu-id="b26ee-116">Date</span></span>    |
| <span data-ttu-id="b26ee-117">groupType</span><span class="sxs-lookup"><span data-stu-id="b26ee-117">groupType</span></span>          | <span data-ttu-id="b26ee-118">String</span><span class="sxs-lookup"><span data-stu-id="b26ee-118">String</span></span>  |
| <span data-ttu-id="b26ee-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="b26ee-119">office365Connected</span></span> | <span data-ttu-id="b26ee-120">Boolesch</span><span class="sxs-lookup"><span data-stu-id="b26ee-120">Boolean</span></span> |
| <span data-ttu-id="b26ee-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="b26ee-121">memberCount</span></span>        | <span data-ttu-id="b26ee-122">Int64</span><span class="sxs-lookup"><span data-stu-id="b26ee-122">Int64</span></span>   |
| <span data-ttu-id="b26ee-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="b26ee-123">postedCount</span></span>        | <span data-ttu-id="b26ee-124">Int64</span><span class="sxs-lookup"><span data-stu-id="b26ee-124">Int64</span></span>   |
| <span data-ttu-id="b26ee-125">readCount</span><span class="sxs-lookup"><span data-stu-id="b26ee-125">readCount</span></span>          | <span data-ttu-id="b26ee-126">Int64</span><span class="sxs-lookup"><span data-stu-id="b26ee-126">Int64</span></span>   |
| <span data-ttu-id="b26ee-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="b26ee-127">likedCount</span></span>         | <span data-ttu-id="b26ee-128">Int64</span><span class="sxs-lookup"><span data-stu-id="b26ee-128">Int64</span></span>   |
| <span data-ttu-id="b26ee-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b26ee-129">reportPeriod</span></span>       | <span data-ttu-id="b26ee-130">String</span><span class="sxs-lookup"><span data-stu-id="b26ee-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="b26ee-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b26ee-131">JSON representation</span></span>

<span data-ttu-id="b26ee-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b26ee-132">The following is a JSON representation of the resource.</span></span>

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
