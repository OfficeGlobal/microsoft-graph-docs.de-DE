---
title: Ressourcentyp yammerDeviceUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 5fe3aa7fa9da243c9cc8f9b015ee85d779b84eb3
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574152"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="02a36-103">Ressourcentyp yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="02a36-103">yammerDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="02a36-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="02a36-104">Properties</span></span>

| <span data-ttu-id="02a36-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="02a36-105">Property</span></span>          | <span data-ttu-id="02a36-106">Typ</span><span class="sxs-lookup"><span data-stu-id="02a36-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="02a36-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="02a36-107">reportRefreshDate</span></span> | <span data-ttu-id="02a36-108">Date</span><span class="sxs-lookup"><span data-stu-id="02a36-108">Date</span></span>    |
| <span data-ttu-id="02a36-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="02a36-109">userPrincipalName</span></span> | <span data-ttu-id="02a36-110">String</span><span class="sxs-lookup"><span data-stu-id="02a36-110">String</span></span>  |
| <span data-ttu-id="02a36-111">displayName</span><span class="sxs-lookup"><span data-stu-id="02a36-111">displayName</span></span>       | <span data-ttu-id="02a36-112">String</span><span class="sxs-lookup"><span data-stu-id="02a36-112">String</span></span>  |
| <span data-ttu-id="02a36-113">userState</span><span class="sxs-lookup"><span data-stu-id="02a36-113">userState</span></span>         | <span data-ttu-id="02a36-114">String</span><span class="sxs-lookup"><span data-stu-id="02a36-114">String</span></span>  |
| <span data-ttu-id="02a36-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="02a36-115">stateChangeDate</span></span>   | <span data-ttu-id="02a36-116">Date</span><span class="sxs-lookup"><span data-stu-id="02a36-116">Date</span></span>    |
| <span data-ttu-id="02a36-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="02a36-117">lastActivityDate</span></span>  | <span data-ttu-id="02a36-118">Date</span><span class="sxs-lookup"><span data-stu-id="02a36-118">Date</span></span>    |
| <span data-ttu-id="02a36-119">usedWeb</span><span class="sxs-lookup"><span data-stu-id="02a36-119">usedWeb</span></span>           | <span data-ttu-id="02a36-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="02a36-120">Boolean</span></span> |
| <span data-ttu-id="02a36-121">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="02a36-121">usedWindowsPhone</span></span>  | <span data-ttu-id="02a36-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="02a36-122">Boolean</span></span> |
| <span data-ttu-id="02a36-123">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="02a36-123">usedAndroidPhone</span></span>  | <span data-ttu-id="02a36-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="02a36-124">Boolean</span></span> |
| <span data-ttu-id="02a36-125">usediPhone</span><span class="sxs-lookup"><span data-stu-id="02a36-125">usediPhone</span></span>        | <span data-ttu-id="02a36-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="02a36-126">Boolean</span></span> |
| <span data-ttu-id="02a36-127">usediPad</span><span class="sxs-lookup"><span data-stu-id="02a36-127">usediPad</span></span>          | <span data-ttu-id="02a36-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="02a36-128">Boolean</span></span> |
| <span data-ttu-id="02a36-129">usedOthers</span><span class="sxs-lookup"><span data-stu-id="02a36-129">usedOthers</span></span>        | <span data-ttu-id="02a36-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="02a36-130">Boolean</span></span> |
| <span data-ttu-id="02a36-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="02a36-131">reportPeriod</span></span>      | <span data-ttu-id="02a36-132">String</span><span class="sxs-lookup"><span data-stu-id="02a36-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="02a36-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="02a36-133">JSON representation</span></span>

<span data-ttu-id="02a36-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="02a36-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "usedOthers": true, 
  "reportPeriod": "String"
}
```
