---
title: Ressourcentyp oneDriveActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 679ec9b8452d388fe311e67d88bcfffd6fe73d93
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060854"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="939e9-103">Ressourcentyp oneDriveActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="939e9-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="939e9-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="939e9-104">Properties</span></span>

| <span data-ttu-id="939e9-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="939e9-105">Property</span></span>                  | <span data-ttu-id="939e9-106">Typ</span><span class="sxs-lookup"><span data-stu-id="939e9-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="939e9-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="939e9-107">reportRefreshDate</span></span>         | <span data-ttu-id="939e9-108">Datum</span><span class="sxs-lookup"><span data-stu-id="939e9-108">Date</span></span>              |
| <span data-ttu-id="939e9-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="939e9-109">userPrincipalName</span></span>         | <span data-ttu-id="939e9-110">String</span><span class="sxs-lookup"><span data-stu-id="939e9-110">String</span></span>            |
| <span data-ttu-id="939e9-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="939e9-111">isDeleted</span></span>                 | <span data-ttu-id="939e9-112">Boolesch</span><span class="sxs-lookup"><span data-stu-id="939e9-112">Boolean</span></span>           |
| <span data-ttu-id="939e9-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="939e9-113">deletedDate</span></span>               | <span data-ttu-id="939e9-114">Datum</span><span class="sxs-lookup"><span data-stu-id="939e9-114">Date</span></span>              |
| <span data-ttu-id="939e9-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="939e9-115">lastActivityDate</span></span>          | <span data-ttu-id="939e9-116">Datum</span><span class="sxs-lookup"><span data-stu-id="939e9-116">Date</span></span>              |
| <span data-ttu-id="939e9-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="939e9-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="939e9-118">Int64</span><span class="sxs-lookup"><span data-stu-id="939e9-118">Int64</span></span>             |
| <span data-ttu-id="939e9-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="939e9-119">syncedFileCount</span></span>           | <span data-ttu-id="939e9-120">Int64</span><span class="sxs-lookup"><span data-stu-id="939e9-120">Int64</span></span>             |
| <span data-ttu-id="939e9-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="939e9-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="939e9-122">Int64</span><span class="sxs-lookup"><span data-stu-id="939e9-122">Int64</span></span>             |
| <span data-ttu-id="939e9-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="939e9-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="939e9-124">Int64</span><span class="sxs-lookup"><span data-stu-id="939e9-124">Int64</span></span>             |
| <span data-ttu-id="939e9-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="939e9-125">assignedProducts</span></span>          | <span data-ttu-id="939e9-126">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="939e9-126">String collection</span></span> |
| <span data-ttu-id="939e9-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="939e9-127">reportPeriod</span></span>              | <span data-ttu-id="939e9-128">String</span><span class="sxs-lookup"><span data-stu-id="939e9-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="939e9-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="939e9-129">JSON representation</span></span>

<span data-ttu-id="939e9-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="939e9-130">The following is a JSON representation of the resource.</span></span>

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
