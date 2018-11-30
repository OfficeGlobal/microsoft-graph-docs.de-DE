---
title: Ressourcentyp yammerDeviceUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 8812b61d974815fd1cdf1bbe1549a21193e5a2f4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065433"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="cdaec-103">Ressourcentyp yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="cdaec-103">yammerDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="cdaec-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cdaec-104">Properties</span></span>

| <span data-ttu-id="cdaec-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cdaec-105">Property</span></span>          | <span data-ttu-id="cdaec-106">Typ</span><span class="sxs-lookup"><span data-stu-id="cdaec-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="cdaec-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="cdaec-107">reportRefreshDate</span></span> | <span data-ttu-id="cdaec-108">Datum</span><span class="sxs-lookup"><span data-stu-id="cdaec-108">Date</span></span>    |
| <span data-ttu-id="cdaec-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cdaec-109">userPrincipalName</span></span> | <span data-ttu-id="cdaec-110">String</span><span class="sxs-lookup"><span data-stu-id="cdaec-110">String</span></span>  |
| <span data-ttu-id="cdaec-111">displayName</span><span class="sxs-lookup"><span data-stu-id="cdaec-111">displayName</span></span>       | <span data-ttu-id="cdaec-112">String</span><span class="sxs-lookup"><span data-stu-id="cdaec-112">String</span></span>  |
| <span data-ttu-id="cdaec-113">userState</span><span class="sxs-lookup"><span data-stu-id="cdaec-113">userState</span></span>         | <span data-ttu-id="cdaec-114">String</span><span class="sxs-lookup"><span data-stu-id="cdaec-114">String</span></span>  |
| <span data-ttu-id="cdaec-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="cdaec-115">stateChangeDate</span></span>   | <span data-ttu-id="cdaec-116">Datum</span><span class="sxs-lookup"><span data-stu-id="cdaec-116">Date</span></span>    |
| <span data-ttu-id="cdaec-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="cdaec-117">lastActivityDate</span></span>  | <span data-ttu-id="cdaec-118">Datum</span><span class="sxs-lookup"><span data-stu-id="cdaec-118">Date</span></span>    |
| <span data-ttu-id="cdaec-119">usedWeb</span><span class="sxs-lookup"><span data-stu-id="cdaec-119">usedWeb</span></span>           | <span data-ttu-id="cdaec-120">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cdaec-120">Boolean</span></span> |
| <span data-ttu-id="cdaec-121">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="cdaec-121">usedWindowsPhone</span></span>  | <span data-ttu-id="cdaec-122">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cdaec-122">Boolean</span></span> |
| <span data-ttu-id="cdaec-123">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="cdaec-123">usedAndroidPhone</span></span>  | <span data-ttu-id="cdaec-124">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cdaec-124">Boolean</span></span> |
| <span data-ttu-id="cdaec-125">usediPhone</span><span class="sxs-lookup"><span data-stu-id="cdaec-125">usediPhone</span></span>        | <span data-ttu-id="cdaec-126">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cdaec-126">Boolean</span></span> |
| <span data-ttu-id="cdaec-127">usediPad</span><span class="sxs-lookup"><span data-stu-id="cdaec-127">usediPad</span></span>          | <span data-ttu-id="cdaec-128">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cdaec-128">Boolean</span></span> |
| <span data-ttu-id="cdaec-129">usedOthers</span><span class="sxs-lookup"><span data-stu-id="cdaec-129">usedOthers</span></span>        | <span data-ttu-id="cdaec-130">Boolesch</span><span class="sxs-lookup"><span data-stu-id="cdaec-130">Boolean</span></span> |
| <span data-ttu-id="cdaec-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="cdaec-131">reportPeriod</span></span>      | <span data-ttu-id="cdaec-132">String</span><span class="sxs-lookup"><span data-stu-id="cdaec-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="cdaec-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cdaec-133">JSON representation</span></span>

<span data-ttu-id="cdaec-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cdaec-134">The following is a JSON representation of the resource.</span></span>

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
