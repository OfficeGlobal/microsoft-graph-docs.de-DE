---
title: Ressourcentyp emailActivityUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 16512c3a8a4dab62d4a71406d6c33d52a5a9bc08
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818002"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="238a9-103">Ressourcentyp emailActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="238a9-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="238a9-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="238a9-104">Properties</span></span>

| <span data-ttu-id="238a9-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="238a9-105">Property</span></span>          | <span data-ttu-id="238a9-106">Typ</span><span class="sxs-lookup"><span data-stu-id="238a9-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="238a9-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="238a9-107">reportRefreshDate</span></span> | <span data-ttu-id="238a9-108">Datum</span><span class="sxs-lookup"><span data-stu-id="238a9-108">Date</span></span>              |
| <span data-ttu-id="238a9-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="238a9-109">userPrincipalName</span></span> | <span data-ttu-id="238a9-110">String</span><span class="sxs-lookup"><span data-stu-id="238a9-110">String</span></span>            |
| <span data-ttu-id="238a9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="238a9-111">displayName</span></span>       | <span data-ttu-id="238a9-112">String</span><span class="sxs-lookup"><span data-stu-id="238a9-112">String</span></span>            |
| <span data-ttu-id="238a9-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="238a9-113">isDeleted</span></span>         | <span data-ttu-id="238a9-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="238a9-114">Boolean</span></span>           |
| <span data-ttu-id="238a9-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="238a9-115">deletedDate</span></span>       | <span data-ttu-id="238a9-116">Datum</span><span class="sxs-lookup"><span data-stu-id="238a9-116">Date</span></span>              |
| <span data-ttu-id="238a9-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="238a9-117">lastActivityDate</span></span>  | <span data-ttu-id="238a9-118">Datum</span><span class="sxs-lookup"><span data-stu-id="238a9-118">Date</span></span>              |
| <span data-ttu-id="238a9-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="238a9-119">sendCount</span></span>         | <span data-ttu-id="238a9-120">Int64</span><span class="sxs-lookup"><span data-stu-id="238a9-120">Int64</span></span>             |
| <span data-ttu-id="238a9-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="238a9-121">receiveCount</span></span>      | <span data-ttu-id="238a9-122">Int64</span><span class="sxs-lookup"><span data-stu-id="238a9-122">Int64</span></span>             |
| <span data-ttu-id="238a9-123">readCount</span><span class="sxs-lookup"><span data-stu-id="238a9-123">readCount</span></span>         | <span data-ttu-id="238a9-124">Int64</span><span class="sxs-lookup"><span data-stu-id="238a9-124">Int64</span></span>             |
| <span data-ttu-id="238a9-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="238a9-125">assignedProducts</span></span>  | <span data-ttu-id="238a9-126">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="238a9-126">String collection</span></span> |
| <span data-ttu-id="238a9-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="238a9-127">reportPeriod</span></span>      | <span data-ttu-id="238a9-128">String</span><span class="sxs-lookup"><span data-stu-id="238a9-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="238a9-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="238a9-129">JSON representation</span></span>

<span data-ttu-id="238a9-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="238a9-130">The following is a JSON representation of the resource.</span></span>

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
