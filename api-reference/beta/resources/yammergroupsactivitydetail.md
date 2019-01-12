---
title: Ressourcentyp yammerGroupsActivityDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 79ce924fff5d1ce9ca861c3d48589a0ecad149dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939168"
---
# <a name="yammergroupsactivitydetail-resource-type"></a><span data-ttu-id="a1710-103">Ressourcentyp yammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="a1710-103">yammerGroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a1710-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a1710-104">Properties</span></span>

| <span data-ttu-id="a1710-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a1710-105">Property</span></span>           | <span data-ttu-id="a1710-106">Typ</span><span class="sxs-lookup"><span data-stu-id="a1710-106">Type</span></span>    |
| :----------------- | :------ |
| <span data-ttu-id="a1710-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a1710-107">reportRefreshDate</span></span>  | <span data-ttu-id="a1710-108">Datum</span><span class="sxs-lookup"><span data-stu-id="a1710-108">Date</span></span>    |
| <span data-ttu-id="a1710-109">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="a1710-109">groupDisplayName</span></span>   | <span data-ttu-id="a1710-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1710-110">String</span></span>  |
| <span data-ttu-id="a1710-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a1710-111">isDeleted</span></span>          | <span data-ttu-id="a1710-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a1710-112">Boolean</span></span> |
| <span data-ttu-id="a1710-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a1710-113">ownerPrincipalName</span></span> | <span data-ttu-id="a1710-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1710-114">String</span></span>  |
| <span data-ttu-id="a1710-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a1710-115">lastActivityDate</span></span>   | <span data-ttu-id="a1710-116">Datum</span><span class="sxs-lookup"><span data-stu-id="a1710-116">Date</span></span>    |
| <span data-ttu-id="a1710-117">groupType</span><span class="sxs-lookup"><span data-stu-id="a1710-117">groupType</span></span>          | <span data-ttu-id="a1710-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1710-118">String</span></span>  |
| <span data-ttu-id="a1710-119">office365Connected</span><span class="sxs-lookup"><span data-stu-id="a1710-119">office365Connected</span></span> | <span data-ttu-id="a1710-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a1710-120">Boolean</span></span> |
| <span data-ttu-id="a1710-121">memberCount</span><span class="sxs-lookup"><span data-stu-id="a1710-121">memberCount</span></span>        | <span data-ttu-id="a1710-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a1710-122">Int64</span></span>   |
| <span data-ttu-id="a1710-123">postedCount</span><span class="sxs-lookup"><span data-stu-id="a1710-123">postedCount</span></span>        | <span data-ttu-id="a1710-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a1710-124">Int64</span></span>   |
| <span data-ttu-id="a1710-125">readCount</span><span class="sxs-lookup"><span data-stu-id="a1710-125">readCount</span></span>          | <span data-ttu-id="a1710-126">Int64</span><span class="sxs-lookup"><span data-stu-id="a1710-126">Int64</span></span>   |
| <span data-ttu-id="a1710-127">likedCount</span><span class="sxs-lookup"><span data-stu-id="a1710-127">likedCount</span></span>         | <span data-ttu-id="a1710-128">Int64</span><span class="sxs-lookup"><span data-stu-id="a1710-128">Int64</span></span>   |
| <span data-ttu-id="a1710-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a1710-129">reportPeriod</span></span>       | <span data-ttu-id="a1710-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a1710-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a1710-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a1710-131">JSON representation</span></span>

<span data-ttu-id="a1710-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a1710-132">The following is a JSON representation of the resource.</span></span>

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
