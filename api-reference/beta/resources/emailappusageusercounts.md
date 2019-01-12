---
title: Ressourcentyp emailAppUsageUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7822528aacc9d6f104012d43004fbb9aabba127c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990803"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="75062-103">Ressourcentyp emailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="75062-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="75062-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="75062-104">Properties</span></span>

| <span data-ttu-id="75062-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="75062-105">Property</span></span>          | <span data-ttu-id="75062-106">Typ</span><span class="sxs-lookup"><span data-stu-id="75062-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="75062-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="75062-107">reportRefreshDate</span></span> | <span data-ttu-id="75062-108">Datum</span><span class="sxs-lookup"><span data-stu-id="75062-108">Date</span></span>   |
| <span data-ttu-id="75062-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="75062-109">mailForMac</span></span>        | <span data-ttu-id="75062-110">Int64</span><span class="sxs-lookup"><span data-stu-id="75062-110">Int64</span></span>  |
| <span data-ttu-id="75062-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="75062-111">outlookForMac</span></span>     | <span data-ttu-id="75062-112">Int64</span><span class="sxs-lookup"><span data-stu-id="75062-112">Int64</span></span>  |
| <span data-ttu-id="75062-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="75062-113">outlookForWindows</span></span> | <span data-ttu-id="75062-114">Int64</span><span class="sxs-lookup"><span data-stu-id="75062-114">Int64</span></span>  |
| <span data-ttu-id="75062-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="75062-115">outlookForMobile</span></span>  | <span data-ttu-id="75062-116">Int64</span><span class="sxs-lookup"><span data-stu-id="75062-116">Int64</span></span>  |
| <span data-ttu-id="75062-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="75062-117">otherForMobile</span></span>    | <span data-ttu-id="75062-118">Int64</span><span class="sxs-lookup"><span data-stu-id="75062-118">Int64</span></span>  |
| <span data-ttu-id="75062-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="75062-119">outlookForWeb</span></span>     | <span data-ttu-id="75062-120">Int64</span><span class="sxs-lookup"><span data-stu-id="75062-120">Int64</span></span>  |
| <span data-ttu-id="75062-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="75062-121">pop3App</span></span>           | <span data-ttu-id="75062-122">Int64</span><span class="sxs-lookup"><span data-stu-id="75062-122">Int64</span></span>  |
| <span data-ttu-id="75062-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="75062-123">imap4App</span></span>          | <span data-ttu-id="75062-124">Int64</span><span class="sxs-lookup"><span data-stu-id="75062-124">Int64</span></span>  |
| <span data-ttu-id="75062-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="75062-125">smtpApp</span></span>           | <span data-ttu-id="75062-126">Int64</span><span class="sxs-lookup"><span data-stu-id="75062-126">Int64</span></span>  |
| <span data-ttu-id="75062-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="75062-127">reportDate</span></span>        | <span data-ttu-id="75062-128">Datum</span><span class="sxs-lookup"><span data-stu-id="75062-128">Date</span></span>   |
| <span data-ttu-id="75062-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="75062-129">reportPeriod</span></span>      | <span data-ttu-id="75062-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="75062-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="75062-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="75062-131">JSON representation</span></span>

<span data-ttu-id="75062-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="75062-132">The following is a JSON representation of the resource.</span></span>

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
