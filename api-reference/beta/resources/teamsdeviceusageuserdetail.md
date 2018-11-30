---
title: Ressourcentyp teamsDeviceUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 4eeec5f07a0a604249617ac87a62ea12b4052395
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065430"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="f9054-103">Ressourcentyp teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="f9054-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f9054-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f9054-104">Properties</span></span>

| <span data-ttu-id="f9054-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f9054-105">Property</span></span>          | <span data-ttu-id="f9054-106">Typ</span><span class="sxs-lookup"><span data-stu-id="f9054-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="f9054-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f9054-107">reportRefreshDate</span></span> | <span data-ttu-id="f9054-108">Datum</span><span class="sxs-lookup"><span data-stu-id="f9054-108">Date</span></span>    |
| <span data-ttu-id="f9054-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f9054-109">userPrincipalName</span></span> | <span data-ttu-id="f9054-110">String</span><span class="sxs-lookup"><span data-stu-id="f9054-110">String</span></span>  |
| <span data-ttu-id="f9054-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="f9054-111">lastActivityDate</span></span>  | <span data-ttu-id="f9054-112">Datum</span><span class="sxs-lookup"><span data-stu-id="f9054-112">Date</span></span>    |
| <span data-ttu-id="f9054-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f9054-113">isDeleted</span></span>         | <span data-ttu-id="f9054-114">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f9054-114">Boolean</span></span> |
| <span data-ttu-id="f9054-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="f9054-115">deletedDate</span></span>       | <span data-ttu-id="f9054-116">Datum</span><span class="sxs-lookup"><span data-stu-id="f9054-116">Date</span></span>    |
| <span data-ttu-id="f9054-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="f9054-117">usedWeb</span></span>           | <span data-ttu-id="f9054-118">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f9054-118">Boolean</span></span> |
| <span data-ttu-id="f9054-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="f9054-119">usedWindowsPhone</span></span>  | <span data-ttu-id="f9054-120">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f9054-120">Boolean</span></span> |
| <span data-ttu-id="f9054-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="f9054-121">usediOS</span></span>           | <span data-ttu-id="f9054-122">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f9054-122">Boolean</span></span> |
| <span data-ttu-id="f9054-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="f9054-123">usedMac</span></span>           | <span data-ttu-id="f9054-124">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f9054-124">Boolean</span></span> |
| <span data-ttu-id="f9054-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="f9054-125">usedAndroidPhone</span></span>  | <span data-ttu-id="f9054-126">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f9054-126">Boolean</span></span> |
| <span data-ttu-id="f9054-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="f9054-127">usedWindows</span></span>       | <span data-ttu-id="f9054-128">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f9054-128">Boolean</span></span> |
| <span data-ttu-id="f9054-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f9054-129">reportPeriod</span></span>      | <span data-ttu-id="f9054-130">String</span><span class="sxs-lookup"><span data-stu-id="f9054-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="f9054-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f9054-131">JSON representation</span></span>

<span data-ttu-id="f9054-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f9054-132">The following is a JSON representation of the resource.</span></span>

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
