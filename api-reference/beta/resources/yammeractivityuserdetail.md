---
title: Ressourcentyp yammerActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: d24e21c9525d49b7af5f8c4efaddd606c20c162b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923033"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="4b4b3-103">Ressourcentyp yammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="4b4b3-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4b4b3-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4b4b3-104">Properties</span></span>

| <span data-ttu-id="4b4b3-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4b4b3-105">Property</span></span>          | <span data-ttu-id="4b4b3-106">Typ</span><span class="sxs-lookup"><span data-stu-id="4b4b3-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="4b4b3-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4b4b3-107">reportRefreshDate</span></span> | <span data-ttu-id="4b4b3-108">Datum</span><span class="sxs-lookup"><span data-stu-id="4b4b3-108">Date</span></span>              |
| <span data-ttu-id="4b4b3-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4b4b3-109">userPrincipalName</span></span> | <span data-ttu-id="4b4b3-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b4b3-110">String</span></span>            |
| <span data-ttu-id="4b4b3-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4b4b3-111">displayName</span></span>       | <span data-ttu-id="4b4b3-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b4b3-112">String</span></span>            |
| <span data-ttu-id="4b4b3-113">userState</span><span class="sxs-lookup"><span data-stu-id="4b4b3-113">userState</span></span>         | <span data-ttu-id="4b4b3-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b4b3-114">String</span></span>            |
| <span data-ttu-id="4b4b3-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="4b4b3-115">stateChangeDate</span></span>   | <span data-ttu-id="4b4b3-116">Datum</span><span class="sxs-lookup"><span data-stu-id="4b4b3-116">Date</span></span>              |
| <span data-ttu-id="4b4b3-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="4b4b3-117">lastActivityDate</span></span>  | <span data-ttu-id="4b4b3-118">Datum</span><span class="sxs-lookup"><span data-stu-id="4b4b3-118">Date</span></span>              |
| <span data-ttu-id="4b4b3-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="4b4b3-119">postedCount</span></span>       | <span data-ttu-id="4b4b3-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4b4b3-120">Int64</span></span>             |
| <span data-ttu-id="4b4b3-121">readCount</span><span class="sxs-lookup"><span data-stu-id="4b4b3-121">readCount</span></span>         | <span data-ttu-id="4b4b3-122">Int64</span><span class="sxs-lookup"><span data-stu-id="4b4b3-122">Int64</span></span>             |
| <span data-ttu-id="4b4b3-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="4b4b3-123">likedCount</span></span>        | <span data-ttu-id="4b4b3-124">Int64</span><span class="sxs-lookup"><span data-stu-id="4b4b3-124">Int64</span></span>             |
| <span data-ttu-id="4b4b3-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="4b4b3-125">assignedProducts</span></span>  | <span data-ttu-id="4b4b3-126">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="4b4b3-126">String collection</span></span> |
| <span data-ttu-id="4b4b3-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4b4b3-127">reportPeriod</span></span>      | <span data-ttu-id="4b4b3-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b4b3-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="4b4b3-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4b4b3-129">JSON representation</span></span>

<span data-ttu-id="4b4b3-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4b4b3-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
