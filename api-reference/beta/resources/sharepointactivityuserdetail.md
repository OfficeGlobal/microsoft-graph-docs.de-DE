---
title: Ressourcentyp sharePointActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: a5b6de8a4a9b82d9e6d34a2ae289f0c7589798ee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058809"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="70cf9-103">Ressourcentyp sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="70cf9-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="70cf9-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="70cf9-104">Properties</span></span>

| <span data-ttu-id="70cf9-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="70cf9-105">Property</span></span>                  | <span data-ttu-id="70cf9-106">Typ</span><span class="sxs-lookup"><span data-stu-id="70cf9-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="70cf9-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="70cf9-107">reportRefreshDate</span></span>         | <span data-ttu-id="70cf9-108">Datum</span><span class="sxs-lookup"><span data-stu-id="70cf9-108">Date</span></span>              |
| <span data-ttu-id="70cf9-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="70cf9-109">userPrincipalName</span></span>         | <span data-ttu-id="70cf9-110">String</span><span class="sxs-lookup"><span data-stu-id="70cf9-110">String</span></span>            |
| <span data-ttu-id="70cf9-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="70cf9-111">isDeleted</span></span>                 | <span data-ttu-id="70cf9-112">Boolesch</span><span class="sxs-lookup"><span data-stu-id="70cf9-112">Boolean</span></span>           |
| <span data-ttu-id="70cf9-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="70cf9-113">deletedDate</span></span>               | <span data-ttu-id="70cf9-114">Datum</span><span class="sxs-lookup"><span data-stu-id="70cf9-114">Date</span></span>              |
| <span data-ttu-id="70cf9-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="70cf9-115">lastActivityDate</span></span>          | <span data-ttu-id="70cf9-116">Datum</span><span class="sxs-lookup"><span data-stu-id="70cf9-116">Date</span></span>              |
| <span data-ttu-id="70cf9-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="70cf9-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="70cf9-118">Int64</span><span class="sxs-lookup"><span data-stu-id="70cf9-118">Int64</span></span>             |
| <span data-ttu-id="70cf9-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="70cf9-119">syncedFileCount</span></span>           | <span data-ttu-id="70cf9-120">Int64</span><span class="sxs-lookup"><span data-stu-id="70cf9-120">Int64</span></span>             |
| <span data-ttu-id="70cf9-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="70cf9-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="70cf9-122">Int64</span><span class="sxs-lookup"><span data-stu-id="70cf9-122">Int64</span></span>             |
| <span data-ttu-id="70cf9-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="70cf9-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="70cf9-124">Int64</span><span class="sxs-lookup"><span data-stu-id="70cf9-124">Int64</span></span>             |
| <span data-ttu-id="70cf9-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="70cf9-125">visitedPageCount</span></span>          | <span data-ttu-id="70cf9-126">Int64</span><span class="sxs-lookup"><span data-stu-id="70cf9-126">Int64</span></span>             |
| <span data-ttu-id="70cf9-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="70cf9-127">assignedProducts</span></span>          | <span data-ttu-id="70cf9-128">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="70cf9-128">String collection</span></span> |
| <span data-ttu-id="70cf9-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="70cf9-129">reportPeriod</span></span>              | <span data-ttu-id="70cf9-130">String</span><span class="sxs-lookup"><span data-stu-id="70cf9-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="70cf9-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="70cf9-131">JSON representation</span></span>

<span data-ttu-id="70cf9-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="70cf9-132">The following is a JSON representation of the resource.</span></span>

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
