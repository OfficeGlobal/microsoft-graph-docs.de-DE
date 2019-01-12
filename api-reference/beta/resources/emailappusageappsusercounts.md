---
title: Ressourcentyp emailAppUsageAppsUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 220770fab755c0e345af23f3fc3113732af63ff0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970381"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="47e43-103">Ressourcentyp emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="47e43-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="47e43-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="47e43-104">Properties</span></span>

| <span data-ttu-id="47e43-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="47e43-105">Property</span></span>          | <span data-ttu-id="47e43-106">Typ</span><span class="sxs-lookup"><span data-stu-id="47e43-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="47e43-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="47e43-107">reportRefreshDate</span></span> | <span data-ttu-id="47e43-108">Datum</span><span class="sxs-lookup"><span data-stu-id="47e43-108">Date</span></span>   |
| <span data-ttu-id="47e43-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="47e43-109">mailForMac</span></span>        | <span data-ttu-id="47e43-110">Int64</span><span class="sxs-lookup"><span data-stu-id="47e43-110">Int64</span></span>  |
| <span data-ttu-id="47e43-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="47e43-111">outlookForMac</span></span>     | <span data-ttu-id="47e43-112">Int64</span><span class="sxs-lookup"><span data-stu-id="47e43-112">Int64</span></span>  |
| <span data-ttu-id="47e43-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="47e43-113">outlookForWindows</span></span> | <span data-ttu-id="47e43-114">Int64</span><span class="sxs-lookup"><span data-stu-id="47e43-114">Int64</span></span>  |
| <span data-ttu-id="47e43-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="47e43-115">outlookForMobile</span></span>  | <span data-ttu-id="47e43-116">Int64</span><span class="sxs-lookup"><span data-stu-id="47e43-116">Int64</span></span>  |
| <span data-ttu-id="47e43-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="47e43-117">otherForMobile</span></span>    | <span data-ttu-id="47e43-118">Int64</span><span class="sxs-lookup"><span data-stu-id="47e43-118">Int64</span></span>  |
| <span data-ttu-id="47e43-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="47e43-119">outlookForWeb</span></span>     | <span data-ttu-id="47e43-120">Int64</span><span class="sxs-lookup"><span data-stu-id="47e43-120">Int64</span></span>  |
| <span data-ttu-id="47e43-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="47e43-121">pop3App</span></span>           | <span data-ttu-id="47e43-122">Int64</span><span class="sxs-lookup"><span data-stu-id="47e43-122">Int64</span></span>  |
| <span data-ttu-id="47e43-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="47e43-123">imap4App</span></span>          | <span data-ttu-id="47e43-124">Int64</span><span class="sxs-lookup"><span data-stu-id="47e43-124">Int64</span></span>  |
| <span data-ttu-id="47e43-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="47e43-125">smtpApp</span></span>           | <span data-ttu-id="47e43-126">Int64</span><span class="sxs-lookup"><span data-stu-id="47e43-126">Int64</span></span>  |
| <span data-ttu-id="47e43-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="47e43-127">reportPeriod</span></span>      | <span data-ttu-id="47e43-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="47e43-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="47e43-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="47e43-129">JSON representation</span></span>

<span data-ttu-id="47e43-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="47e43-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageAppsUserCounts"
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
  "reportPeriod": "String"
}
```
