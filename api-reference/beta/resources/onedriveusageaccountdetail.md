---
title: Ressourcentyp oneDriveUsageAccountDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 92695f509302ede4b3ce64320e8f4ed42418f7e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842609"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="c7567-103">Ressourcentyp oneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="c7567-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c7567-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c7567-104">Properties</span></span>

| <span data-ttu-id="c7567-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c7567-105">Property</span></span>                | <span data-ttu-id="c7567-106">Typ</span><span class="sxs-lookup"><span data-stu-id="c7567-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="c7567-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c7567-107">reportRefreshDate</span></span>       | <span data-ttu-id="c7567-108">Datum</span><span class="sxs-lookup"><span data-stu-id="c7567-108">Date</span></span>    |
| <span data-ttu-id="c7567-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="c7567-109">siteUrl</span></span>                 | <span data-ttu-id="c7567-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c7567-110">String</span></span>  |
| <span data-ttu-id="c7567-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="c7567-111">ownerDisplayName</span></span>        | <span data-ttu-id="c7567-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c7567-112">String</span></span>  |
| <span data-ttu-id="c7567-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c7567-113">isDeleted</span></span>               | <span data-ttu-id="c7567-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="c7567-114">Boolean</span></span> |
| <span data-ttu-id="c7567-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c7567-115">lastActivityDate</span></span>        | <span data-ttu-id="c7567-116">Datum</span><span class="sxs-lookup"><span data-stu-id="c7567-116">Date</span></span>    |
| <span data-ttu-id="c7567-117">fileCount</span><span class="sxs-lookup"><span data-stu-id="c7567-117">fileCount</span></span>               | <span data-ttu-id="c7567-118">Int64</span><span class="sxs-lookup"><span data-stu-id="c7567-118">Int64</span></span>   |
| <span data-ttu-id="c7567-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="c7567-119">activeFileCount</span></span>         | <span data-ttu-id="c7567-120">Int64</span><span class="sxs-lookup"><span data-stu-id="c7567-120">Int64</span></span>   |
| <span data-ttu-id="c7567-121">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="c7567-121">storageUsedInBytes</span></span>      | <span data-ttu-id="c7567-122">Int64</span><span class="sxs-lookup"><span data-stu-id="c7567-122">Int64</span></span>   |
| <span data-ttu-id="c7567-123">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="c7567-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="c7567-124">Int64</span><span class="sxs-lookup"><span data-stu-id="c7567-124">Int64</span></span>   |
| <span data-ttu-id="c7567-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c7567-125">reportPeriod</span></span>            | <span data-ttu-id="c7567-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c7567-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="c7567-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c7567-127">JSON representation</span></span>

<span data-ttu-id="c7567-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c7567-128">The following is a JSON representation of the resource.</span></span>

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
