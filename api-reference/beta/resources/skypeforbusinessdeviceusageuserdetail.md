---
title: Ressourcentyp skypeForBusinessDeviceUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: b62920d124fd52e0f653c128eeb0956cdfe0c680
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059714"
---
# <a name="skypeforbusinessdeviceusageuserdetail-resource-type"></a><span data-ttu-id="5c40c-103">Ressourcentyp skypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="5c40c-103">skypeForBusinessDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5c40c-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5c40c-104">Properties</span></span>

| <span data-ttu-id="5c40c-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5c40c-105">Property</span></span>          | <span data-ttu-id="5c40c-106">Typ</span><span class="sxs-lookup"><span data-stu-id="5c40c-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="5c40c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5c40c-107">reportRefreshDate</span></span> | <span data-ttu-id="5c40c-108">Datum</span><span class="sxs-lookup"><span data-stu-id="5c40c-108">Date</span></span>    |
| <span data-ttu-id="5c40c-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5c40c-109">userPrincipalName</span></span> | <span data-ttu-id="5c40c-110">String</span><span class="sxs-lookup"><span data-stu-id="5c40c-110">String</span></span>  |
| <span data-ttu-id="5c40c-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="5c40c-111">lastActivityDate</span></span>  | <span data-ttu-id="5c40c-112">Datum</span><span class="sxs-lookup"><span data-stu-id="5c40c-112">Date</span></span>    |
| <span data-ttu-id="5c40c-113">usedWindows</span><span class="sxs-lookup"><span data-stu-id="5c40c-113">usedWindows</span></span>       | <span data-ttu-id="5c40c-114">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5c40c-114">Boolean</span></span> |
| <span data-ttu-id="5c40c-115">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="5c40c-115">usedWindowsPhone</span></span>  | <span data-ttu-id="5c40c-116">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5c40c-116">Boolean</span></span> |
| <span data-ttu-id="5c40c-117">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="5c40c-117">usedAndroidPhone</span></span>  | <span data-ttu-id="5c40c-118">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5c40c-118">Boolean</span></span> |
| <span data-ttu-id="5c40c-119">usediPhone</span><span class="sxs-lookup"><span data-stu-id="5c40c-119">usediPhone</span></span>        | <span data-ttu-id="5c40c-120">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5c40c-120">Boolean</span></span> |
| <span data-ttu-id="5c40c-121">usediPad</span><span class="sxs-lookup"><span data-stu-id="5c40c-121">usediPad</span></span>          | <span data-ttu-id="5c40c-122">Boolesch</span><span class="sxs-lookup"><span data-stu-id="5c40c-122">Boolean</span></span> |
| <span data-ttu-id="5c40c-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5c40c-123">reportPeriod</span></span>      | <span data-ttu-id="5c40c-124">String</span><span class="sxs-lookup"><span data-stu-id="5c40c-124">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="5c40c-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5c40c-125">JSON representation</span></span>

<span data-ttu-id="5c40c-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5c40c-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "usedWindows": true, 
  "usedWindowsPhone": true, 
  "usedAndroidPhone": true, 
  "usediPhone": true, 
  "usediPad": true, 
  "reportPeriod": "String"
}
```
