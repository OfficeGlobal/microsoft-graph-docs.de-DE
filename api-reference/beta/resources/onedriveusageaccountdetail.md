---
title: Ressourcentyp oneDriveUsageAccountDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 4b80ebc24aa45be0368dbb59d6d3e99e7adacc8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063031"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="79eae-103">Ressourcentyp oneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="79eae-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="79eae-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="79eae-104">Properties</span></span>

| <span data-ttu-id="79eae-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="79eae-105">Property</span></span>                | <span data-ttu-id="79eae-106">Typ</span><span class="sxs-lookup"><span data-stu-id="79eae-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="79eae-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="79eae-107">reportRefreshDate</span></span>       | <span data-ttu-id="79eae-108">Datum</span><span class="sxs-lookup"><span data-stu-id="79eae-108">Date</span></span>    |
| <span data-ttu-id="79eae-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="79eae-109">siteUrl</span></span>                 | <span data-ttu-id="79eae-110">String</span><span class="sxs-lookup"><span data-stu-id="79eae-110">String</span></span>  |
| <span data-ttu-id="79eae-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="79eae-111">ownerDisplayName</span></span>        | <span data-ttu-id="79eae-112">String</span><span class="sxs-lookup"><span data-stu-id="79eae-112">String</span></span>  |
| <span data-ttu-id="79eae-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="79eae-113">isDeleted</span></span>               | <span data-ttu-id="79eae-114">Boolesch</span><span class="sxs-lookup"><span data-stu-id="79eae-114">Boolean</span></span> |
| <span data-ttu-id="79eae-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="79eae-115">lastActivityDate</span></span>        | <span data-ttu-id="79eae-116">Datum</span><span class="sxs-lookup"><span data-stu-id="79eae-116">Date</span></span>    |
| <span data-ttu-id="79eae-117">fileCount</span><span class="sxs-lookup"><span data-stu-id="79eae-117">fileCount</span></span>               | <span data-ttu-id="79eae-118">Int64</span><span class="sxs-lookup"><span data-stu-id="79eae-118">Int64</span></span>   |
| <span data-ttu-id="79eae-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="79eae-119">activeFileCount</span></span>         | <span data-ttu-id="79eae-120">Int64</span><span class="sxs-lookup"><span data-stu-id="79eae-120">Int64</span></span>   |
| <span data-ttu-id="79eae-121">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="79eae-121">storageUsedInBytes</span></span>      | <span data-ttu-id="79eae-122">Int64</span><span class="sxs-lookup"><span data-stu-id="79eae-122">Int64</span></span>   |
| <span data-ttu-id="79eae-123">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="79eae-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="79eae-124">Int64</span><span class="sxs-lookup"><span data-stu-id="79eae-124">Int64</span></span>   |
| <span data-ttu-id="79eae-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="79eae-125">reportPeriod</span></span>            | <span data-ttu-id="79eae-126">String</span><span class="sxs-lookup"><span data-stu-id="79eae-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="79eae-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="79eae-127">JSON representation</span></span>

<span data-ttu-id="79eae-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="79eae-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "reportPeriod": "String"
}
```
