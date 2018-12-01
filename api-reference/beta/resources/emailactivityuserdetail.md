---
title: Ressourcentyp emailActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 4f74b4af41c44e41b07bae1a8421011bc5188efc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058137"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="4e549-103">Ressourcentyp emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="4e549-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4e549-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4e549-104">Properties</span></span>

| <span data-ttu-id="4e549-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4e549-105">Property</span></span>          | <span data-ttu-id="4e549-106">Typ</span><span class="sxs-lookup"><span data-stu-id="4e549-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="4e549-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4e549-107">reportRefreshDate</span></span> | <span data-ttu-id="4e549-108">Datum</span><span class="sxs-lookup"><span data-stu-id="4e549-108">Date</span></span>              |
| <span data-ttu-id="4e549-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4e549-109">userPrincipalName</span></span> | <span data-ttu-id="4e549-110">String</span><span class="sxs-lookup"><span data-stu-id="4e549-110">String</span></span>            |
| <span data-ttu-id="4e549-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4e549-111">displayName</span></span>       | <span data-ttu-id="4e549-112">String</span><span class="sxs-lookup"><span data-stu-id="4e549-112">String</span></span>            |
| <span data-ttu-id="4e549-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="4e549-113">isDeleted</span></span>         | <span data-ttu-id="4e549-114">Boolesch</span><span class="sxs-lookup"><span data-stu-id="4e549-114">Boolean</span></span>           |
| <span data-ttu-id="4e549-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="4e549-115">deletedDate</span></span>       | <span data-ttu-id="4e549-116">Datum</span><span class="sxs-lookup"><span data-stu-id="4e549-116">Date</span></span>              |
| <span data-ttu-id="4e549-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="4e549-117">lastActivityDate</span></span>  | <span data-ttu-id="4e549-118">Datum</span><span class="sxs-lookup"><span data-stu-id="4e549-118">Date</span></span>              |
| <span data-ttu-id="4e549-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="4e549-119">sendCount</span></span>         | <span data-ttu-id="4e549-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4e549-120">Int64</span></span>             |
| <span data-ttu-id="4e549-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="4e549-121">receiveCount</span></span>      | <span data-ttu-id="4e549-122">Int64</span><span class="sxs-lookup"><span data-stu-id="4e549-122">Int64</span></span>             |
| <span data-ttu-id="4e549-123">readCount</span><span class="sxs-lookup"><span data-stu-id="4e549-123">readCount</span></span>         | <span data-ttu-id="4e549-124">Int64</span><span class="sxs-lookup"><span data-stu-id="4e549-124">Int64</span></span>             |
| <span data-ttu-id="4e549-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="4e549-125">assignedProducts</span></span>  | <span data-ttu-id="4e549-126">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="4e549-126">String collection</span></span> |
| <span data-ttu-id="4e549-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4e549-127">reportPeriod</span></span>      | <span data-ttu-id="4e549-128">String</span><span class="sxs-lookup"><span data-stu-id="4e549-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="4e549-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4e549-129">JSON representation</span></span>

<span data-ttu-id="4e549-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4e549-130">The following is a JSON representation of the resource.</span></span>

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
