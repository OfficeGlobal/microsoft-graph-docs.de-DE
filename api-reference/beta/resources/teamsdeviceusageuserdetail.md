---
title: Ressourcentyp teamsDeviceUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8cdd2fe1a212bb1d36846b80fc1b558c576deb47
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953785"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="021ef-103">Ressourcentyp teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="021ef-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="021ef-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="021ef-104">Properties</span></span>

| <span data-ttu-id="021ef-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="021ef-105">Property</span></span>          | <span data-ttu-id="021ef-106">Typ</span><span class="sxs-lookup"><span data-stu-id="021ef-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="021ef-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="021ef-107">reportRefreshDate</span></span> | <span data-ttu-id="021ef-108">Datum</span><span class="sxs-lookup"><span data-stu-id="021ef-108">Date</span></span>    |
| <span data-ttu-id="021ef-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="021ef-109">userPrincipalName</span></span> | <span data-ttu-id="021ef-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="021ef-110">String</span></span>  |
| <span data-ttu-id="021ef-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="021ef-111">lastActivityDate</span></span>  | <span data-ttu-id="021ef-112">Datum</span><span class="sxs-lookup"><span data-stu-id="021ef-112">Date</span></span>    |
| <span data-ttu-id="021ef-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="021ef-113">isDeleted</span></span>         | <span data-ttu-id="021ef-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="021ef-114">Boolean</span></span> |
| <span data-ttu-id="021ef-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="021ef-115">deletedDate</span></span>       | <span data-ttu-id="021ef-116">Datum</span><span class="sxs-lookup"><span data-stu-id="021ef-116">Date</span></span>    |
| <span data-ttu-id="021ef-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="021ef-117">usedWeb</span></span>           | <span data-ttu-id="021ef-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="021ef-118">Boolean</span></span> |
| <span data-ttu-id="021ef-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="021ef-119">usedWindowsPhone</span></span>  | <span data-ttu-id="021ef-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="021ef-120">Boolean</span></span> |
| <span data-ttu-id="021ef-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="021ef-121">usediOS</span></span>           | <span data-ttu-id="021ef-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="021ef-122">Boolean</span></span> |
| <span data-ttu-id="021ef-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="021ef-123">usedMac</span></span>           | <span data-ttu-id="021ef-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="021ef-124">Boolean</span></span> |
| <span data-ttu-id="021ef-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="021ef-125">usedAndroidPhone</span></span>  | <span data-ttu-id="021ef-126">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="021ef-126">Boolean</span></span> |
| <span data-ttu-id="021ef-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="021ef-127">usedWindows</span></span>       | <span data-ttu-id="021ef-128">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="021ef-128">Boolean</span></span> |
| <span data-ttu-id="021ef-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="021ef-129">reportPeriod</span></span>      | <span data-ttu-id="021ef-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="021ef-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="021ef-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="021ef-131">JSON representation</span></span>

<span data-ttu-id="021ef-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="021ef-132">The following is a JSON representation of the resource.</span></span>

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
