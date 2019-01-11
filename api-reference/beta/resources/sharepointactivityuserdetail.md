---
title: Ressourcentyp sharePointActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 4503739a7b2e13cade72951ae56ab410f22608b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880696"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="d95ea-103">Ressourcentyp sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="d95ea-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d95ea-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d95ea-104">Properties</span></span>

| <span data-ttu-id="d95ea-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d95ea-105">Property</span></span>                  | <span data-ttu-id="d95ea-106">Typ</span><span class="sxs-lookup"><span data-stu-id="d95ea-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="d95ea-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d95ea-107">reportRefreshDate</span></span>         | <span data-ttu-id="d95ea-108">Datum</span><span class="sxs-lookup"><span data-stu-id="d95ea-108">Date</span></span>              |
| <span data-ttu-id="d95ea-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d95ea-109">userPrincipalName</span></span>         | <span data-ttu-id="d95ea-110">String</span><span class="sxs-lookup"><span data-stu-id="d95ea-110">String</span></span>            |
| <span data-ttu-id="d95ea-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="d95ea-111">isDeleted</span></span>                 | <span data-ttu-id="d95ea-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="d95ea-112">Boolean</span></span>           |
| <span data-ttu-id="d95ea-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="d95ea-113">deletedDate</span></span>               | <span data-ttu-id="d95ea-114">Datum</span><span class="sxs-lookup"><span data-stu-id="d95ea-114">Date</span></span>              |
| <span data-ttu-id="d95ea-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="d95ea-115">lastActivityDate</span></span>          | <span data-ttu-id="d95ea-116">Datum</span><span class="sxs-lookup"><span data-stu-id="d95ea-116">Date</span></span>              |
| <span data-ttu-id="d95ea-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="d95ea-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="d95ea-118">Int64</span><span class="sxs-lookup"><span data-stu-id="d95ea-118">Int64</span></span>             |
| <span data-ttu-id="d95ea-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="d95ea-119">syncedFileCount</span></span>           | <span data-ttu-id="d95ea-120">Int64</span><span class="sxs-lookup"><span data-stu-id="d95ea-120">Int64</span></span>             |
| <span data-ttu-id="d95ea-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="d95ea-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="d95ea-122">Int64</span><span class="sxs-lookup"><span data-stu-id="d95ea-122">Int64</span></span>             |
| <span data-ttu-id="d95ea-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="d95ea-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="d95ea-124">Int64</span><span class="sxs-lookup"><span data-stu-id="d95ea-124">Int64</span></span>             |
| <span data-ttu-id="d95ea-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="d95ea-125">visitedPageCount</span></span>          | <span data-ttu-id="d95ea-126">Int64</span><span class="sxs-lookup"><span data-stu-id="d95ea-126">Int64</span></span>             |
| <span data-ttu-id="d95ea-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="d95ea-127">assignedProducts</span></span>          | <span data-ttu-id="d95ea-128">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="d95ea-128">String collection</span></span> |
| <span data-ttu-id="d95ea-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d95ea-129">reportPeriod</span></span>              | <span data-ttu-id="d95ea-130">String</span><span class="sxs-lookup"><span data-stu-id="d95ea-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="d95ea-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d95ea-131">JSON representation</span></span>

<span data-ttu-id="d95ea-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d95ea-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "viewedOrEditedFileCount": 1024, 
  "syncedFileCount": 1024, 
  "sharedInternallyFileCount": 1024, 
  "sharedExternallyFileCount": 1024, 
  "visitedPageCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
