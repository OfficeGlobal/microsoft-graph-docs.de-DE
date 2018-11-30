---
title: Ressourcentyp emailAppUsageUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: c8669c8a34987bc1e71152ae717f9be3ba101107
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063547"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="9496b-103">Ressourcentyp emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="9496b-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="9496b-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9496b-104">Properties</span></span>

| <span data-ttu-id="9496b-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9496b-105">Property</span></span>          | <span data-ttu-id="9496b-106">Typ</span><span class="sxs-lookup"><span data-stu-id="9496b-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="9496b-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9496b-107">reportRefreshDate</span></span> | <span data-ttu-id="9496b-108">Datum</span><span class="sxs-lookup"><span data-stu-id="9496b-108">Date</span></span>   |
| <span data-ttu-id="9496b-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="9496b-109">mailForMac</span></span>        | <span data-ttu-id="9496b-110">Int64</span><span class="sxs-lookup"><span data-stu-id="9496b-110">Int64</span></span>  |
| <span data-ttu-id="9496b-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="9496b-111">outlookForMac</span></span>     | <span data-ttu-id="9496b-112">Int64</span><span class="sxs-lookup"><span data-stu-id="9496b-112">Int64</span></span>  |
| <span data-ttu-id="9496b-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="9496b-113">outlookForWindows</span></span> | <span data-ttu-id="9496b-114">Int64</span><span class="sxs-lookup"><span data-stu-id="9496b-114">Int64</span></span>  |
| <span data-ttu-id="9496b-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="9496b-115">outlookForMobile</span></span>  | <span data-ttu-id="9496b-116">Int64</span><span class="sxs-lookup"><span data-stu-id="9496b-116">Int64</span></span>  |
| <span data-ttu-id="9496b-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="9496b-117">otherForMobile</span></span>    | <span data-ttu-id="9496b-118">Int64</span><span class="sxs-lookup"><span data-stu-id="9496b-118">Int64</span></span>  |
| <span data-ttu-id="9496b-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="9496b-119">outlookForWeb</span></span>     | <span data-ttu-id="9496b-120">Int64</span><span class="sxs-lookup"><span data-stu-id="9496b-120">Int64</span></span>  |
| <span data-ttu-id="9496b-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="9496b-121">pop3App</span></span>           | <span data-ttu-id="9496b-122">Int64</span><span class="sxs-lookup"><span data-stu-id="9496b-122">Int64</span></span>  |
| <span data-ttu-id="9496b-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="9496b-123">imap4App</span></span>          | <span data-ttu-id="9496b-124">Int64</span><span class="sxs-lookup"><span data-stu-id="9496b-124">Int64</span></span>  |
| <span data-ttu-id="9496b-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="9496b-125">smtpApp</span></span>           | <span data-ttu-id="9496b-126">Int64</span><span class="sxs-lookup"><span data-stu-id="9496b-126">Int64</span></span>  |
| <span data-ttu-id="9496b-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="9496b-127">reportDate</span></span>        | <span data-ttu-id="9496b-128">Datum</span><span class="sxs-lookup"><span data-stu-id="9496b-128">Date</span></span>   |
| <span data-ttu-id="9496b-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="9496b-129">reportPeriod</span></span>      | <span data-ttu-id="9496b-130">String</span><span class="sxs-lookup"><span data-stu-id="9496b-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9496b-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9496b-131">JSON representation</span></span>

<span data-ttu-id="9496b-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9496b-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailForMac": 1024, 
  "outlookForMac": 1024, 
  "outlookForWindows": 1024, 
  "outlookForMobile": 1024, 
  "otherForMobile": 1024, 
  "outlookForWeb": 1024, 
  "pop3App": 1024, 
  "imap4App": 1024, 
  "smtpApp": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
