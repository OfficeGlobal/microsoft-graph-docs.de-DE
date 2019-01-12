---
title: Ressourcentyp emailActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b871bf5dbaedd961fad09bf97be868f46e7430a1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938307"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="21d1f-103">Ressourcentyp emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="21d1f-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="21d1f-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="21d1f-104">Properties</span></span>

| <span data-ttu-id="21d1f-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="21d1f-105">Property</span></span>          | <span data-ttu-id="21d1f-106">Typ</span><span class="sxs-lookup"><span data-stu-id="21d1f-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="21d1f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="21d1f-107">reportRefreshDate</span></span> | <span data-ttu-id="21d1f-108">Datum</span><span class="sxs-lookup"><span data-stu-id="21d1f-108">Date</span></span>              |
| <span data-ttu-id="21d1f-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="21d1f-109">userPrincipalName</span></span> | <span data-ttu-id="21d1f-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21d1f-110">String</span></span>            |
| <span data-ttu-id="21d1f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="21d1f-111">displayName</span></span>       | <span data-ttu-id="21d1f-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21d1f-112">String</span></span>            |
| <span data-ttu-id="21d1f-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="21d1f-113">isDeleted</span></span>         | <span data-ttu-id="21d1f-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="21d1f-114">Boolean</span></span>           |
| <span data-ttu-id="21d1f-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="21d1f-115">deletedDate</span></span>       | <span data-ttu-id="21d1f-116">Datum</span><span class="sxs-lookup"><span data-stu-id="21d1f-116">Date</span></span>              |
| <span data-ttu-id="21d1f-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="21d1f-117">lastActivityDate</span></span>  | <span data-ttu-id="21d1f-118">Datum</span><span class="sxs-lookup"><span data-stu-id="21d1f-118">Date</span></span>              |
| <span data-ttu-id="21d1f-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="21d1f-119">sendCount</span></span>         | <span data-ttu-id="21d1f-120">Int64</span><span class="sxs-lookup"><span data-stu-id="21d1f-120">Int64</span></span>             |
| <span data-ttu-id="21d1f-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="21d1f-121">receiveCount</span></span>      | <span data-ttu-id="21d1f-122">Int64</span><span class="sxs-lookup"><span data-stu-id="21d1f-122">Int64</span></span>             |
| <span data-ttu-id="21d1f-123">readCount</span><span class="sxs-lookup"><span data-stu-id="21d1f-123">readCount</span></span>         | <span data-ttu-id="21d1f-124">Int64</span><span class="sxs-lookup"><span data-stu-id="21d1f-124">Int64</span></span>             |
| <span data-ttu-id="21d1f-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="21d1f-125">assignedProducts</span></span>  | <span data-ttu-id="21d1f-126">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="21d1f-126">String collection</span></span> |
| <span data-ttu-id="21d1f-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="21d1f-127">reportPeriod</span></span>      | <span data-ttu-id="21d1f-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21d1f-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="21d1f-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="21d1f-129">JSON representation</span></span>

<span data-ttu-id="21d1f-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="21d1f-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "sendCount": 1024, 
  "receiveCount": 1024, 
  "readCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
