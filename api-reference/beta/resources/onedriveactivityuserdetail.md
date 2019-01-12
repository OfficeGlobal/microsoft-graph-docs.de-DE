---
title: Ressourcentyp oneDriveActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 29c9c8b723d4f87fa9858e26906878c973b37b09
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948247"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="bfb2e-103">Ressourcentyp oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="bfb2e-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bfb2e-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bfb2e-104">Properties</span></span>

| <span data-ttu-id="bfb2e-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bfb2e-105">Property</span></span>                  | <span data-ttu-id="bfb2e-106">Typ</span><span class="sxs-lookup"><span data-stu-id="bfb2e-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="bfb2e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bfb2e-107">reportRefreshDate</span></span>         | <span data-ttu-id="bfb2e-108">Datum</span><span class="sxs-lookup"><span data-stu-id="bfb2e-108">Date</span></span>              |
| <span data-ttu-id="bfb2e-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bfb2e-109">userPrincipalName</span></span>         | <span data-ttu-id="bfb2e-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bfb2e-110">String</span></span>            |
| <span data-ttu-id="bfb2e-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="bfb2e-111">isDeleted</span></span>                 | <span data-ttu-id="bfb2e-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="bfb2e-112">Boolean</span></span>           |
| <span data-ttu-id="bfb2e-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="bfb2e-113">deletedDate</span></span>               | <span data-ttu-id="bfb2e-114">Datum</span><span class="sxs-lookup"><span data-stu-id="bfb2e-114">Date</span></span>              |
| <span data-ttu-id="bfb2e-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="bfb2e-115">lastActivityDate</span></span>          | <span data-ttu-id="bfb2e-116">Datum</span><span class="sxs-lookup"><span data-stu-id="bfb2e-116">Date</span></span>              |
| <span data-ttu-id="bfb2e-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="bfb2e-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="bfb2e-118">Int64</span><span class="sxs-lookup"><span data-stu-id="bfb2e-118">Int64</span></span>             |
| <span data-ttu-id="bfb2e-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="bfb2e-119">syncedFileCount</span></span>           | <span data-ttu-id="bfb2e-120">Int64</span><span class="sxs-lookup"><span data-stu-id="bfb2e-120">Int64</span></span>             |
| <span data-ttu-id="bfb2e-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="bfb2e-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="bfb2e-122">Int64</span><span class="sxs-lookup"><span data-stu-id="bfb2e-122">Int64</span></span>             |
| <span data-ttu-id="bfb2e-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="bfb2e-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="bfb2e-124">Int64</span><span class="sxs-lookup"><span data-stu-id="bfb2e-124">Int64</span></span>             |
| <span data-ttu-id="bfb2e-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="bfb2e-125">assignedProducts</span></span>          | <span data-ttu-id="bfb2e-126">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="bfb2e-126">String collection</span></span> |
| <span data-ttu-id="bfb2e-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bfb2e-127">reportPeriod</span></span>              | <span data-ttu-id="bfb2e-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bfb2e-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="bfb2e-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bfb2e-129">JSON representation</span></span>

<span data-ttu-id="bfb2e-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bfb2e-130">The following is a JSON representation of the resource.</span></span>

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
