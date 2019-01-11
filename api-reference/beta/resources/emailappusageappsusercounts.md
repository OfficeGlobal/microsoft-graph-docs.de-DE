---
title: Ressourcentyp emailAppUsageAppsUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: efbc4ce75293237813e9a835cb45ff0bf0ec4b26
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807819"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="0cc91-103">Ressourcentyp emailAppUsageAppsUserCounts</span><span class="sxs-lookup"><span data-stu-id="0cc91-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0cc91-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0cc91-104">Properties</span></span>

| <span data-ttu-id="0cc91-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0cc91-105">Property</span></span>          | <span data-ttu-id="0cc91-106">Typ</span><span class="sxs-lookup"><span data-stu-id="0cc91-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="0cc91-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0cc91-107">reportRefreshDate</span></span> | <span data-ttu-id="0cc91-108">Datum</span><span class="sxs-lookup"><span data-stu-id="0cc91-108">Date</span></span>   |
| <span data-ttu-id="0cc91-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="0cc91-109">mailForMac</span></span>        | <span data-ttu-id="0cc91-110">Int64</span><span class="sxs-lookup"><span data-stu-id="0cc91-110">Int64</span></span>  |
| <span data-ttu-id="0cc91-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="0cc91-111">outlookForMac</span></span>     | <span data-ttu-id="0cc91-112">Int64</span><span class="sxs-lookup"><span data-stu-id="0cc91-112">Int64</span></span>  |
| <span data-ttu-id="0cc91-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="0cc91-113">outlookForWindows</span></span> | <span data-ttu-id="0cc91-114">Int64</span><span class="sxs-lookup"><span data-stu-id="0cc91-114">Int64</span></span>  |
| <span data-ttu-id="0cc91-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="0cc91-115">outlookForMobile</span></span>  | <span data-ttu-id="0cc91-116">Int64</span><span class="sxs-lookup"><span data-stu-id="0cc91-116">Int64</span></span>  |
| <span data-ttu-id="0cc91-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="0cc91-117">otherForMobile</span></span>    | <span data-ttu-id="0cc91-118">Int64</span><span class="sxs-lookup"><span data-stu-id="0cc91-118">Int64</span></span>  |
| <span data-ttu-id="0cc91-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="0cc91-119">outlookForWeb</span></span>     | <span data-ttu-id="0cc91-120">Int64</span><span class="sxs-lookup"><span data-stu-id="0cc91-120">Int64</span></span>  |
| <span data-ttu-id="0cc91-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="0cc91-121">pop3App</span></span>           | <span data-ttu-id="0cc91-122">Int64</span><span class="sxs-lookup"><span data-stu-id="0cc91-122">Int64</span></span>  |
| <span data-ttu-id="0cc91-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="0cc91-123">imap4App</span></span>          | <span data-ttu-id="0cc91-124">Int64</span><span class="sxs-lookup"><span data-stu-id="0cc91-124">Int64</span></span>  |
| <span data-ttu-id="0cc91-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="0cc91-125">smtpApp</span></span>           | <span data-ttu-id="0cc91-126">Int64</span><span class="sxs-lookup"><span data-stu-id="0cc91-126">Int64</span></span>  |
| <span data-ttu-id="0cc91-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0cc91-127">reportPeriod</span></span>      | <span data-ttu-id="0cc91-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0cc91-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0cc91-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0cc91-129">JSON representation</span></span>

<span data-ttu-id="0cc91-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0cc91-130">The following is a JSON representation of the resource.</span></span>

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
