---
title: Ressourcentyp skypeForBusinessPeerToPeerActivityUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: ad3b409f3abc4cc9e7476825f9dbf5b7c2120d92
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063143"
---
# <a name="skypeforbusinesspeertopeeractivityusercounts-resource-type"></a><span data-ttu-id="121a5-103">Ressourcentyp skypeForBusinessPeerToPeerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="121a5-103">skypeForBusinessPeerToPeerActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="121a5-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="121a5-104">Properties</span></span>

| <span data-ttu-id="121a5-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="121a5-105">Property</span></span>          | <span data-ttu-id="121a5-106">Typ</span><span class="sxs-lookup"><span data-stu-id="121a5-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="121a5-107">Instant Messaging</span><span class="sxs-lookup"><span data-stu-id="121a5-107">im</span></span>                | <span data-ttu-id="121a5-108">Int64</span><span class="sxs-lookup"><span data-stu-id="121a5-108">Int64</span></span>  |
| <span data-ttu-id="121a5-109">audio</span><span class="sxs-lookup"><span data-stu-id="121a5-109">audio</span></span>             | <span data-ttu-id="121a5-110">Int64</span><span class="sxs-lookup"><span data-stu-id="121a5-110">Int64</span></span>  |
| <span data-ttu-id="121a5-111">video</span><span class="sxs-lookup"><span data-stu-id="121a5-111">video</span></span>             | <span data-ttu-id="121a5-112">Int64</span><span class="sxs-lookup"><span data-stu-id="121a5-112">Int64</span></span>  |
| <span data-ttu-id="121a5-113">appSharing</span><span class="sxs-lookup"><span data-stu-id="121a5-113">appSharing</span></span>        | <span data-ttu-id="121a5-114">Int64</span><span class="sxs-lookup"><span data-stu-id="121a5-114">Int64</span></span>  |
| <span data-ttu-id="121a5-115">fileTransfer</span><span class="sxs-lookup"><span data-stu-id="121a5-115">fileTransfer</span></span>      | <span data-ttu-id="121a5-116">Int64</span><span class="sxs-lookup"><span data-stu-id="121a5-116">Int64</span></span>  |
| <span data-ttu-id="121a5-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="121a5-117">reportRefreshDate</span></span> | <span data-ttu-id="121a5-118">Datum</span><span class="sxs-lookup"><span data-stu-id="121a5-118">Date</span></span>   |
| <span data-ttu-id="121a5-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="121a5-119">reportDate</span></span>        | <span data-ttu-id="121a5-120">Datum</span><span class="sxs-lookup"><span data-stu-id="121a5-120">Date</span></span>   |
| <span data-ttu-id="121a5-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="121a5-121">reportPeriod</span></span>      | <span data-ttu-id="121a5-122">String</span><span class="sxs-lookup"><span data-stu-id="121a5-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="121a5-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="121a5-123">JSON representation</span></span>

<span data-ttu-id="121a5-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="121a5-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts"
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
