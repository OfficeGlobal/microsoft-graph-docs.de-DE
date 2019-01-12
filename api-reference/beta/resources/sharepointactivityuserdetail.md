---
title: Ressourcentyp sharePointActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a7dc324d821dca26ff1083f1e48c258e1955d72f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979943"
---
# <a name="sharepointactivityuserdetail-resource-type"></a><span data-ttu-id="83ad1-103">Ressourcentyp sharePointActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="83ad1-103">sharePointActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="83ad1-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="83ad1-104">Properties</span></span>

| <span data-ttu-id="83ad1-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="83ad1-105">Property</span></span>                  | <span data-ttu-id="83ad1-106">Typ</span><span class="sxs-lookup"><span data-stu-id="83ad1-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="83ad1-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="83ad1-107">reportRefreshDate</span></span>         | <span data-ttu-id="83ad1-108">Datum</span><span class="sxs-lookup"><span data-stu-id="83ad1-108">Date</span></span>              |
| <span data-ttu-id="83ad1-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="83ad1-109">userPrincipalName</span></span>         | <span data-ttu-id="83ad1-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83ad1-110">String</span></span>            |
| <span data-ttu-id="83ad1-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="83ad1-111">isDeleted</span></span>                 | <span data-ttu-id="83ad1-112">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="83ad1-112">Boolean</span></span>           |
| <span data-ttu-id="83ad1-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="83ad1-113">deletedDate</span></span>               | <span data-ttu-id="83ad1-114">Datum</span><span class="sxs-lookup"><span data-stu-id="83ad1-114">Date</span></span>              |
| <span data-ttu-id="83ad1-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="83ad1-115">lastActivityDate</span></span>          | <span data-ttu-id="83ad1-116">Datum</span><span class="sxs-lookup"><span data-stu-id="83ad1-116">Date</span></span>              |
| <span data-ttu-id="83ad1-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="83ad1-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="83ad1-118">Int64</span><span class="sxs-lookup"><span data-stu-id="83ad1-118">Int64</span></span>             |
| <span data-ttu-id="83ad1-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="83ad1-119">syncedFileCount</span></span>           | <span data-ttu-id="83ad1-120">Int64</span><span class="sxs-lookup"><span data-stu-id="83ad1-120">Int64</span></span>             |
| <span data-ttu-id="83ad1-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="83ad1-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="83ad1-122">Int64</span><span class="sxs-lookup"><span data-stu-id="83ad1-122">Int64</span></span>             |
| <span data-ttu-id="83ad1-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="83ad1-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="83ad1-124">Int64</span><span class="sxs-lookup"><span data-stu-id="83ad1-124">Int64</span></span>             |
| <span data-ttu-id="83ad1-125">visitedPageCount</span><span class="sxs-lookup"><span data-stu-id="83ad1-125">visitedPageCount</span></span>          | <span data-ttu-id="83ad1-126">Int64</span><span class="sxs-lookup"><span data-stu-id="83ad1-126">Int64</span></span>             |
| <span data-ttu-id="83ad1-127">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="83ad1-127">assignedProducts</span></span>          | <span data-ttu-id="83ad1-128">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="83ad1-128">String collection</span></span> |
| <span data-ttu-id="83ad1-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="83ad1-129">reportPeriod</span></span>              | <span data-ttu-id="83ad1-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83ad1-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="83ad1-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="83ad1-131">JSON representation</span></span>

<span data-ttu-id="83ad1-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="83ad1-132">The following is a JSON representation of the resource.</span></span>

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
