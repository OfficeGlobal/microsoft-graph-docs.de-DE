---
title: Ressourcentyp emailActivitySummary
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 82fbdc2621b9c8746ed3028fe44414edeb7e56db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871344"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="128dd-103">Ressourcentyp emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="128dd-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="128dd-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="128dd-104">Properties</span></span>

| <span data-ttu-id="128dd-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="128dd-105">Property</span></span>          | <span data-ttu-id="128dd-106">Typ</span><span class="sxs-lookup"><span data-stu-id="128dd-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="128dd-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="128dd-107">reportRefreshDate</span></span> | <span data-ttu-id="128dd-108">Datum</span><span class="sxs-lookup"><span data-stu-id="128dd-108">Date</span></span>   |
| <span data-ttu-id="128dd-109">Senden</span><span class="sxs-lookup"><span data-stu-id="128dd-109">send</span></span>              | <span data-ttu-id="128dd-110">Int64</span><span class="sxs-lookup"><span data-stu-id="128dd-110">Int64</span></span>  |
| <span data-ttu-id="128dd-111">empfangen</span><span class="sxs-lookup"><span data-stu-id="128dd-111">receive</span></span>           | <span data-ttu-id="128dd-112">Int64</span><span class="sxs-lookup"><span data-stu-id="128dd-112">Int64</span></span>  |
| <span data-ttu-id="128dd-113">Lesen</span><span class="sxs-lookup"><span data-stu-id="128dd-113">read</span></span>              | <span data-ttu-id="128dd-114">Int64</span><span class="sxs-lookup"><span data-stu-id="128dd-114">Int64</span></span>  |
| <span data-ttu-id="128dd-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="128dd-115">reportDate</span></span>        | <span data-ttu-id="128dd-116">Datum</span><span class="sxs-lookup"><span data-stu-id="128dd-116">Date</span></span>   |
| <span data-ttu-id="128dd-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="128dd-117">reportPeriod</span></span>      | <span data-ttu-id="128dd-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="128dd-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="128dd-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="128dd-119">JSON representation</span></span>

<span data-ttu-id="128dd-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="128dd-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
