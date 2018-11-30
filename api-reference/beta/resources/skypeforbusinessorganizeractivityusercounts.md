---
title: Ressourcentyp skypeForBusinessOrganizerActivityUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 0e0b6838b58b4a3fab9a62351446bf26fc50bfbd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063146"
---
# <a name="skypeforbusinessorganizeractivityusercounts-resource-type"></a><span data-ttu-id="4b533-103">Ressourcentyp skypeForBusinessOrganizerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="4b533-103">skypeForBusinessOrganizerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4b533-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4b533-104">Properties</span></span>

| <span data-ttu-id="4b533-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4b533-105">Property</span></span>           | <span data-ttu-id="4b533-106">Typ</span><span class="sxs-lookup"><span data-stu-id="4b533-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="4b533-107">Instant Messaging</span><span class="sxs-lookup"><span data-stu-id="4b533-107">im</span></span>                 | <span data-ttu-id="4b533-108">Int64</span><span class="sxs-lookup"><span data-stu-id="4b533-108">Int64</span></span>  |
| <span data-ttu-id="4b533-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="4b533-109">audioVideo</span></span>         | <span data-ttu-id="4b533-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4b533-110">Int64</span></span>  |
| <span data-ttu-id="4b533-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="4b533-111">appSharing</span></span>         | <span data-ttu-id="4b533-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4b533-112">Int64</span></span>  |
| <span data-ttu-id="4b533-113">web</span><span class="sxs-lookup"><span data-stu-id="4b533-113">web</span></span>                | <span data-ttu-id="4b533-114">Int64</span><span class="sxs-lookup"><span data-stu-id="4b533-114">Int64</span></span>  |
| <span data-ttu-id="4b533-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="4b533-115">dialInOut3rdParty</span></span>  | <span data-ttu-id="4b533-116">Int64</span><span class="sxs-lookup"><span data-stu-id="4b533-116">Int64</span></span>  |
| <span data-ttu-id="4b533-117">dialInOutMicrosoft</span><span class="sxs-lookup"><span data-stu-id="4b533-117">dialInOutMicrosoft</span></span> | <span data-ttu-id="4b533-118">Int64</span><span class="sxs-lookup"><span data-stu-id="4b533-118">Int64</span></span>  |
| <span data-ttu-id="4b533-119">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4b533-119">reportRefreshDate</span></span>  | <span data-ttu-id="4b533-120">Datum</span><span class="sxs-lookup"><span data-stu-id="4b533-120">Date</span></span>   |
| <span data-ttu-id="4b533-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="4b533-121">reportDate</span></span>         | <span data-ttu-id="4b533-122">Datum</span><span class="sxs-lookup"><span data-stu-id="4b533-122">Date</span></span>   |
| <span data-ttu-id="4b533-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4b533-123">reportPeriod</span></span>       | <span data-ttu-id="4b533-124">String</span><span class="sxs-lookup"><span data-stu-id="4b533-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4b533-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4b533-125">JSON representation</span></span>

<span data-ttu-id="4b533-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4b533-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "dialInOutMicrosoft": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```