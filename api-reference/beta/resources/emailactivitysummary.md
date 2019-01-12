---
title: Ressourcentyp emailActivitySummary
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 84958874af09b31aafed694c1a62d080a5c798ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990089"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="4f093-103">Ressourcentyp emailActivitySummary</span><span class="sxs-lookup"><span data-stu-id="4f093-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4f093-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4f093-104">Properties</span></span>

| <span data-ttu-id="4f093-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4f093-105">Property</span></span>          | <span data-ttu-id="4f093-106">Typ</span><span class="sxs-lookup"><span data-stu-id="4f093-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="4f093-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4f093-107">reportRefreshDate</span></span> | <span data-ttu-id="4f093-108">Datum</span><span class="sxs-lookup"><span data-stu-id="4f093-108">Date</span></span>   |
| <span data-ttu-id="4f093-109">Senden</span><span class="sxs-lookup"><span data-stu-id="4f093-109">send</span></span>              | <span data-ttu-id="4f093-110">Int64</span><span class="sxs-lookup"><span data-stu-id="4f093-110">Int64</span></span>  |
| <span data-ttu-id="4f093-111">empfangen</span><span class="sxs-lookup"><span data-stu-id="4f093-111">receive</span></span>           | <span data-ttu-id="4f093-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4f093-112">Int64</span></span>  |
| <span data-ttu-id="4f093-113">Lesen</span><span class="sxs-lookup"><span data-stu-id="4f093-113">read</span></span>              | <span data-ttu-id="4f093-114">Int64</span><span class="sxs-lookup"><span data-stu-id="4f093-114">Int64</span></span>  |
| <span data-ttu-id="4f093-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="4f093-115">reportDate</span></span>        | <span data-ttu-id="4f093-116">Datum</span><span class="sxs-lookup"><span data-stu-id="4f093-116">Date</span></span>   |
| <span data-ttu-id="4f093-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4f093-117">reportPeriod</span></span>      | <span data-ttu-id="4f093-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4f093-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4f093-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4f093-119">JSON representation</span></span>

<span data-ttu-id="4f093-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4f093-120">The following is a JSON representation of the resource.</span></span>

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
