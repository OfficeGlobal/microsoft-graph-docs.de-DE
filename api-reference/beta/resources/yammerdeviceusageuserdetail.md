---
title: Ressourcentyp yammerDeviceUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 2b74222c1a636fac271268e228c8140e7d1cf33f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912008"
---
# <a name="yammerdeviceusageuserdetail-resource-type"></a><span data-ttu-id="06963-103">Ressourcentyp yammerDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="06963-103">yammerDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="06963-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="06963-104">Properties</span></span>

| <span data-ttu-id="06963-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="06963-105">Property</span></span>          | <span data-ttu-id="06963-106">Typ</span><span class="sxs-lookup"><span data-stu-id="06963-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="06963-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="06963-107">reportRefreshDate</span></span> | <span data-ttu-id="06963-108">Datum</span><span class="sxs-lookup"><span data-stu-id="06963-108">Date</span></span>    |
| <span data-ttu-id="06963-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="06963-109">userPrincipalName</span></span> | <span data-ttu-id="06963-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06963-110">String</span></span>  |
| <span data-ttu-id="06963-111">displayName</span><span class="sxs-lookup"><span data-stu-id="06963-111">displayName</span></span>       | <span data-ttu-id="06963-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06963-112">String</span></span>  |
| <span data-ttu-id="06963-113">userState</span><span class="sxs-lookup"><span data-stu-id="06963-113">userState</span></span>         | <span data-ttu-id="06963-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06963-114">String</span></span>  |
| <span data-ttu-id="06963-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="06963-115">stateChangeDate</span></span>   | <span data-ttu-id="06963-116">Datum</span><span class="sxs-lookup"><span data-stu-id="06963-116">Date</span></span>    |
| <span data-ttu-id="06963-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="06963-117">lastActivityDate</span></span>  | <span data-ttu-id="06963-118">Datum</span><span class="sxs-lookup"><span data-stu-id="06963-118">Date</span></span>    |
| <span data-ttu-id="06963-119">usedWeb</span><span class="sxs-lookup"><span data-stu-id="06963-119">usedWeb</span></span>           | <span data-ttu-id="06963-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06963-120">Boolean</span></span> |
| <span data-ttu-id="06963-121">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="06963-121">usedWindowsPhone</span></span>  | <span data-ttu-id="06963-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06963-122">Boolean</span></span> |
| <span data-ttu-id="06963-123">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="06963-123">usedAndroidPhone</span></span>  | <span data-ttu-id="06963-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06963-124">Boolean</span></span> |
| <span data-ttu-id="06963-125">usediPhone</span><span class="sxs-lookup"><span data-stu-id="06963-125">usediPhone</span></span>        | <span data-ttu-id="06963-126">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06963-126">Boolean</span></span> |
| <span data-ttu-id="06963-127">usediPad</span><span class="sxs-lookup"><span data-stu-id="06963-127">usediPad</span></span>          | <span data-ttu-id="06963-128">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06963-128">Boolean</span></span> |
| <span data-ttu-id="06963-129">usedOthers</span><span class="sxs-lookup"><span data-stu-id="06963-129">usedOthers</span></span>        | <span data-ttu-id="06963-130">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06963-130">Boolean</span></span> |
| <span data-ttu-id="06963-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="06963-131">reportPeriod</span></span>      | <span data-ttu-id="06963-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06963-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="06963-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="06963-133">JSON representation</span></span>

<span data-ttu-id="06963-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="06963-134">The following is a JSON representation of the resource.</span></span>

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
