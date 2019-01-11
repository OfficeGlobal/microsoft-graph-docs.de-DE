---
title: Ressourcentyp teamsDeviceUsageUserDetail
description: Es folgt eine JSON-Darstellung der Ressource.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 06e2cea1154c608b61642b07adbd96aae1710903
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807105"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="17d5d-103">Ressourcentyp teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="17d5d-103">teamsDeviceUsageUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="17d5d-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="17d5d-104">Properties</span></span>

| <span data-ttu-id="17d5d-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="17d5d-105">Property</span></span>          | <span data-ttu-id="17d5d-106">Typ</span><span class="sxs-lookup"><span data-stu-id="17d5d-106">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="17d5d-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="17d5d-107">reportRefreshDate</span></span> | <span data-ttu-id="17d5d-108">Datum</span><span class="sxs-lookup"><span data-stu-id="17d5d-108">Date</span></span>    |
| <span data-ttu-id="17d5d-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="17d5d-109">userPrincipalName</span></span> | <span data-ttu-id="17d5d-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17d5d-110">String</span></span>  |
| <span data-ttu-id="17d5d-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="17d5d-111">lastActivityDate</span></span>  | <span data-ttu-id="17d5d-112">Datum</span><span class="sxs-lookup"><span data-stu-id="17d5d-112">Date</span></span>    |
| <span data-ttu-id="17d5d-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="17d5d-113">isDeleted</span></span>         | <span data-ttu-id="17d5d-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="17d5d-114">Boolean</span></span> |
| <span data-ttu-id="17d5d-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="17d5d-115">deletedDate</span></span>       | <span data-ttu-id="17d5d-116">Datum</span><span class="sxs-lookup"><span data-stu-id="17d5d-116">Date</span></span>    |
| <span data-ttu-id="17d5d-117">usedWeb</span><span class="sxs-lookup"><span data-stu-id="17d5d-117">usedWeb</span></span>           | <span data-ttu-id="17d5d-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="17d5d-118">Boolean</span></span> |
| <span data-ttu-id="17d5d-119">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="17d5d-119">usedWindowsPhone</span></span>  | <span data-ttu-id="17d5d-120">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="17d5d-120">Boolean</span></span> |
| <span data-ttu-id="17d5d-121">usediOS</span><span class="sxs-lookup"><span data-stu-id="17d5d-121">usediOS</span></span>           | <span data-ttu-id="17d5d-122">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="17d5d-122">Boolean</span></span> |
| <span data-ttu-id="17d5d-123">usedMac</span><span class="sxs-lookup"><span data-stu-id="17d5d-123">usedMac</span></span>           | <span data-ttu-id="17d5d-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="17d5d-124">Boolean</span></span> |
| <span data-ttu-id="17d5d-125">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="17d5d-125">usedAndroidPhone</span></span>  | <span data-ttu-id="17d5d-126">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="17d5d-126">Boolean</span></span> |
| <span data-ttu-id="17d5d-127">usedWindows</span><span class="sxs-lookup"><span data-stu-id="17d5d-127">usedWindows</span></span>       | <span data-ttu-id="17d5d-128">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="17d5d-128">Boolean</span></span> |
| <span data-ttu-id="17d5d-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="17d5d-129">reportPeriod</span></span>      | <span data-ttu-id="17d5d-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17d5d-130">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="17d5d-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="17d5d-131">JSON representation</span></span>

<span data-ttu-id="17d5d-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="17d5d-132">The following is a JSON representation of the resource.</span></span>

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
