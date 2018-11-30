---
title: Ressourcentyp skypeForBusinessPeerToPeerActivityCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: cdc8ec2a63c4a03ac8b77bedba06c6addfba4584
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061468"
---
# <a name="skypeforbusinesspeertopeeractivitycounts-resource-type"></a><span data-ttu-id="70140-103">Ressourcentyp skypeForBusinessPeerToPeerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="70140-103">skypeForBusinessPeerToPeerActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="70140-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="70140-104">Properties</span></span>

| <span data-ttu-id="70140-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="70140-105">Property</span></span>          | <span data-ttu-id="70140-106">Typ</span><span class="sxs-lookup"><span data-stu-id="70140-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="70140-107">Instant Messaging</span><span class="sxs-lookup"><span data-stu-id="70140-107">im</span></span>                | <span data-ttu-id="70140-108">Int64</span><span class="sxs-lookup"><span data-stu-id="70140-108">Int64</span></span>  |
| <span data-ttu-id="70140-109">audio</span><span class="sxs-lookup"><span data-stu-id="70140-109">audio</span></span>             | <span data-ttu-id="70140-110">Int64</span><span class="sxs-lookup"><span data-stu-id="70140-110">Int64</span></span>  |
| <span data-ttu-id="70140-111">video</span><span class="sxs-lookup"><span data-stu-id="70140-111">video</span></span>             | <span data-ttu-id="70140-112">Int64</span><span class="sxs-lookup"><span data-stu-id="70140-112">Int64</span></span>  |
| <span data-ttu-id="70140-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="70140-113">appSharing</span></span>        | <span data-ttu-id="70140-114">Int64</span><span class="sxs-lookup"><span data-stu-id="70140-114">Int64</span></span>  |
| <span data-ttu-id="70140-115">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="70140-115">fileTransfer</span></span>      | <span data-ttu-id="70140-116">Int64</span><span class="sxs-lookup"><span data-stu-id="70140-116">Int64</span></span>  |
| <span data-ttu-id="70140-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="70140-117">reportRefreshDate</span></span> | <span data-ttu-id="70140-118">Datum</span><span class="sxs-lookup"><span data-stu-id="70140-118">Date</span></span>   |
| <span data-ttu-id="70140-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="70140-119">reportDate</span></span>        | <span data-ttu-id="70140-120">Datum</span><span class="sxs-lookup"><span data-stu-id="70140-120">Date</span></span>   |
| <span data-ttu-id="70140-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="70140-121">reportPeriod</span></span>      | <span data-ttu-id="70140-122">String</span><span class="sxs-lookup"><span data-stu-id="70140-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="70140-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="70140-123">JSON representation</span></span>

<span data-ttu-id="70140-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="70140-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audio": 1024, 
  "video": 1024, 
  "appSharing": 1024, 
  "fileTransfer": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
