---
title: Ressourcentyp oneDriveActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 2f498c7c9507c4210f12f76d57f62729f84da578
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820790"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="ed864-103">Ressourcentyp oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="ed864-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ed864-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ed864-104">Properties</span></span>

| <span data-ttu-id="ed864-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ed864-105">Property</span></span>                  | <span data-ttu-id="ed864-106">Typ</span><span class="sxs-lookup"><span data-stu-id="ed864-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="ed864-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ed864-107">reportRefreshDate</span></span>         | <span data-ttu-id="ed864-108">Datum</span><span class="sxs-lookup"><span data-stu-id="ed864-108">Date</span></span>              |
| <span data-ttu-id="ed864-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ed864-109">userPrincipalName</span></span>         | <span data-ttu-id="ed864-110">String</span><span class="sxs-lookup"><span data-stu-id="ed864-110">String</span></span>            |
| <span data-ttu-id="ed864-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="ed864-111">isDeleted</span></span>                 | <span data-ttu-id="ed864-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed864-112">Boolean</span></span>           |
| <span data-ttu-id="ed864-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="ed864-113">deletedDate</span></span>               | <span data-ttu-id="ed864-114">Datum</span><span class="sxs-lookup"><span data-stu-id="ed864-114">Date</span></span>              |
| <span data-ttu-id="ed864-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="ed864-115">lastActivityDate</span></span>          | <span data-ttu-id="ed864-116">Datum</span><span class="sxs-lookup"><span data-stu-id="ed864-116">Date</span></span>              |
| <span data-ttu-id="ed864-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="ed864-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="ed864-118">Int64</span><span class="sxs-lookup"><span data-stu-id="ed864-118">Int64</span></span>             |
| <span data-ttu-id="ed864-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="ed864-119">syncedFileCount</span></span>           | <span data-ttu-id="ed864-120">Int64</span><span class="sxs-lookup"><span data-stu-id="ed864-120">Int64</span></span>             |
| <span data-ttu-id="ed864-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="ed864-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="ed864-122">Int64</span><span class="sxs-lookup"><span data-stu-id="ed864-122">Int64</span></span>             |
| <span data-ttu-id="ed864-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="ed864-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="ed864-124">Int64</span><span class="sxs-lookup"><span data-stu-id="ed864-124">Int64</span></span>             |
| <span data-ttu-id="ed864-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="ed864-125">assignedProducts</span></span>          | <span data-ttu-id="ed864-126">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="ed864-126">String collection</span></span> |
| <span data-ttu-id="ed864-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ed864-127">reportPeriod</span></span>              | <span data-ttu-id="ed864-128">String</span><span class="sxs-lookup"><span data-stu-id="ed864-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="ed864-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ed864-129">JSON representation</span></span>

<span data-ttu-id="ed864-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ed864-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
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
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
