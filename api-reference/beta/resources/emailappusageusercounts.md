---
title: Ressourcentyp emailAppUsageUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: a018776f092e9b7f378e8069666d015e1cd3e4a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835448"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="1c6d1-103">Ressourcentyp emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="1c6d1-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1c6d1-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1c6d1-104">Properties</span></span>

| <span data-ttu-id="1c6d1-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1c6d1-105">Property</span></span>          | <span data-ttu-id="1c6d1-106">Typ</span><span class="sxs-lookup"><span data-stu-id="1c6d1-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="1c6d1-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1c6d1-107">reportRefreshDate</span></span> | <span data-ttu-id="1c6d1-108">Datum</span><span class="sxs-lookup"><span data-stu-id="1c6d1-108">Date</span></span>   |
| <span data-ttu-id="1c6d1-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="1c6d1-109">mailForMac</span></span>        | <span data-ttu-id="1c6d1-110">Int64</span><span class="sxs-lookup"><span data-stu-id="1c6d1-110">Int64</span></span>  |
| <span data-ttu-id="1c6d1-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="1c6d1-111">outlookForMac</span></span>     | <span data-ttu-id="1c6d1-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1c6d1-112">Int64</span></span>  |
| <span data-ttu-id="1c6d1-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="1c6d1-113">outlookForWindows</span></span> | <span data-ttu-id="1c6d1-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1c6d1-114">Int64</span></span>  |
| <span data-ttu-id="1c6d1-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="1c6d1-115">outlookForMobile</span></span>  | <span data-ttu-id="1c6d1-116">Int64</span><span class="sxs-lookup"><span data-stu-id="1c6d1-116">Int64</span></span>  |
| <span data-ttu-id="1c6d1-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="1c6d1-117">otherForMobile</span></span>    | <span data-ttu-id="1c6d1-118">Int64</span><span class="sxs-lookup"><span data-stu-id="1c6d1-118">Int64</span></span>  |
| <span data-ttu-id="1c6d1-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="1c6d1-119">outlookForWeb</span></span>     | <span data-ttu-id="1c6d1-120">Int64</span><span class="sxs-lookup"><span data-stu-id="1c6d1-120">Int64</span></span>  |
| <span data-ttu-id="1c6d1-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="1c6d1-121">pop3App</span></span>           | <span data-ttu-id="1c6d1-122">Int64</span><span class="sxs-lookup"><span data-stu-id="1c6d1-122">Int64</span></span>  |
| <span data-ttu-id="1c6d1-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="1c6d1-123">imap4App</span></span>          | <span data-ttu-id="1c6d1-124">Int64</span><span class="sxs-lookup"><span data-stu-id="1c6d1-124">Int64</span></span>  |
| <span data-ttu-id="1c6d1-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="1c6d1-125">smtpApp</span></span>           | <span data-ttu-id="1c6d1-126">Int64</span><span class="sxs-lookup"><span data-stu-id="1c6d1-126">Int64</span></span>  |
| <span data-ttu-id="1c6d1-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="1c6d1-127">reportDate</span></span>        | <span data-ttu-id="1c6d1-128">Datum</span><span class="sxs-lookup"><span data-stu-id="1c6d1-128">Date</span></span>   |
| <span data-ttu-id="1c6d1-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1c6d1-129">reportPeriod</span></span>      | <span data-ttu-id="1c6d1-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1c6d1-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1c6d1-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1c6d1-131">JSON representation</span></span>

<span data-ttu-id="1c6d1-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1c6d1-132">The following is a JSON representation of the resource.</span></span>

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
