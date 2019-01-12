---
title: Ressourcentyp oneDriveUsageAccountDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c13e03d1170b0ebbc53394541c4564c60c67e78
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957396"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="cb961-103">Ressourcentyp oneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="cb961-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="cb961-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cb961-104">Properties</span></span>

| <span data-ttu-id="cb961-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cb961-105">Property</span></span>                | <span data-ttu-id="cb961-106">Typ</span><span class="sxs-lookup"><span data-stu-id="cb961-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="cb961-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="cb961-107">reportRefreshDate</span></span>       | <span data-ttu-id="cb961-108">Datum</span><span class="sxs-lookup"><span data-stu-id="cb961-108">Date</span></span>    |
| <span data-ttu-id="cb961-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="cb961-109">siteUrl</span></span>                 | <span data-ttu-id="cb961-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb961-110">String</span></span>  |
| <span data-ttu-id="cb961-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="cb961-111">ownerDisplayName</span></span>        | <span data-ttu-id="cb961-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb961-112">String</span></span>  |
| <span data-ttu-id="cb961-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="cb961-113">isDeleted</span></span>               | <span data-ttu-id="cb961-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="cb961-114">Boolean</span></span> |
| <span data-ttu-id="cb961-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="cb961-115">lastActivityDate</span></span>        | <span data-ttu-id="cb961-116">Datum</span><span class="sxs-lookup"><span data-stu-id="cb961-116">Date</span></span>    |
| <span data-ttu-id="cb961-117">fileCount</span><span class="sxs-lookup"><span data-stu-id="cb961-117">fileCount</span></span>               | <span data-ttu-id="cb961-118">Int64</span><span class="sxs-lookup"><span data-stu-id="cb961-118">Int64</span></span>   |
| <span data-ttu-id="cb961-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="cb961-119">activeFileCount</span></span>         | <span data-ttu-id="cb961-120">Int64</span><span class="sxs-lookup"><span data-stu-id="cb961-120">Int64</span></span>   |
| <span data-ttu-id="cb961-121">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="cb961-121">storageUsedInBytes</span></span>      | <span data-ttu-id="cb961-122">Int64</span><span class="sxs-lookup"><span data-stu-id="cb961-122">Int64</span></span>   |
| <span data-ttu-id="cb961-123">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="cb961-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="cb961-124">Int64</span><span class="sxs-lookup"><span data-stu-id="cb961-124">Int64</span></span>   |
| <span data-ttu-id="cb961-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="cb961-125">reportPeriod</span></span>            | <span data-ttu-id="cb961-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb961-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="cb961-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cb961-127">JSON representation</span></span>

<span data-ttu-id="cb961-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cb961-128">The following is a JSON representation of the resource.</span></span>

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
