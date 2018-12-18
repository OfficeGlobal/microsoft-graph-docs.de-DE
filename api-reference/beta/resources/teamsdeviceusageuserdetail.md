---
title: Ressourcentyp teamsDeviceUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
author: nkramer
ms.openlocfilehash: 1947b66a59190945e5a6b823b47ef8df7d02683a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329001"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="58db5-103">Ressourcentyp teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="58db5-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="58db5-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="58db5-104">Properties</span></span>

| <span data-ttu-id="58db5-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="58db5-105">Property</span></span>          | <span data-ttu-id="58db5-106">Typ</span><span class="sxs-lookup"><span data-stu-id="58db5-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="58db5-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="58db5-107">reportRefreshDate</span></span> | <span data-ttu-id="58db5-108">Datum</span><span class="sxs-lookup"><span data-stu-id="58db5-108">Date</span></span>    |
| <span data-ttu-id="58db5-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="58db5-109">userPrincipalName</span></span> | <span data-ttu-id="58db5-110">String</span><span class="sxs-lookup"><span data-stu-id="58db5-110">String</span></span>  |
| <span data-ttu-id="58db5-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="58db5-111">lastActivityDate</span></span>  | <span data-ttu-id="58db5-112">Datum</span><span class="sxs-lookup"><span data-stu-id="58db5-112">Date</span></span>    |
| <span data-ttu-id="58db5-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="58db5-113">isDeleted</span></span>         | <span data-ttu-id="58db5-114">Boolesch</span><span class="sxs-lookup"><span data-stu-id="58db5-114">Boolean</span></span> |
| <span data-ttu-id="58db5-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="58db5-115">deletedDate</span></span>       | <span data-ttu-id="58db5-116">Datum</span><span class="sxs-lookup"><span data-stu-id="58db5-116">Date</span></span>    |
| <span data-ttu-id="58db5-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="58db5-117">usedWeb</span></span>           | <span data-ttu-id="58db5-118">Boolesch</span><span class="sxs-lookup"><span data-stu-id="58db5-118">Boolean</span></span> |
| <span data-ttu-id="58db5-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="58db5-119">usedWindowsPhone</span></span>  | <span data-ttu-id="58db5-120">Boolesch</span><span class="sxs-lookup"><span data-stu-id="58db5-120">Boolean</span></span> |
| <span data-ttu-id="58db5-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="58db5-121">usediOS</span></span>           | <span data-ttu-id="58db5-122">Boolesch</span><span class="sxs-lookup"><span data-stu-id="58db5-122">Boolean</span></span> |
| <span data-ttu-id="58db5-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="58db5-123">usedMac</span></span>           | <span data-ttu-id="58db5-124">Boolesch</span><span class="sxs-lookup"><span data-stu-id="58db5-124">Boolean</span></span> |
| <span data-ttu-id="58db5-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="58db5-125">usedAndroidPhone</span></span>  | <span data-ttu-id="58db5-126">Boolesch</span><span class="sxs-lookup"><span data-stu-id="58db5-126">Boolean</span></span> |
| <span data-ttu-id="58db5-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="58db5-127">usedWindows</span></span>       | <span data-ttu-id="58db5-128">Boolesch</span><span class="sxs-lookup"><span data-stu-id="58db5-128">Boolean</span></span> |
| <span data-ttu-id="58db5-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="58db5-129">reportPeriod</span></span>      | <span data-ttu-id="58db5-130">String</span><span class="sxs-lookup"><span data-stu-id="58db5-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="58db5-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="58db5-131">JSON representation</span></span>

<span data-ttu-id="58db5-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="58db5-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "reportPeriod": "String"
}
```
