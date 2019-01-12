---
title: Ressourcentyp siteActivitySummary
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a49b8e47ca2a6efcc5c5c87702fdea0122b208e1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957137"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="52a4b-103">Ressourcentyp siteActivitySummary</span><span class="sxs-lookup"><span data-stu-id="52a4b-103">siteActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="52a4b-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="52a4b-104">Properties</span></span>

| <span data-ttu-id="52a4b-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="52a4b-105">Property</span></span>          | <span data-ttu-id="52a4b-106">Typ</span><span class="sxs-lookup"><span data-stu-id="52a4b-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="52a4b-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="52a4b-107">reportRefreshDate</span></span> | <span data-ttu-id="52a4b-108">Datum</span><span class="sxs-lookup"><span data-stu-id="52a4b-108">Date</span></span>   |
| <span data-ttu-id="52a4b-109">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="52a4b-109">viewedOrEdited</span></span>    | <span data-ttu-id="52a4b-110">Int64</span><span class="sxs-lookup"><span data-stu-id="52a4b-110">Int64</span></span>  |
| <span data-ttu-id="52a4b-111">synchronisiert</span><span class="sxs-lookup"><span data-stu-id="52a4b-111">synced</span></span>            | <span data-ttu-id="52a4b-112">Int64</span><span class="sxs-lookup"><span data-stu-id="52a4b-112">Int64</span></span>  |
| <span data-ttu-id="52a4b-113">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="52a4b-113">sharedInternally</span></span>  | <span data-ttu-id="52a4b-114">Int64</span><span class="sxs-lookup"><span data-stu-id="52a4b-114">Int64</span></span>  |
| <span data-ttu-id="52a4b-115">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="52a4b-115">sharedExternally</span></span>  | <span data-ttu-id="52a4b-116">Int64</span><span class="sxs-lookup"><span data-stu-id="52a4b-116">Int64</span></span>  |
| <span data-ttu-id="52a4b-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="52a4b-117">reportDate</span></span>        | <span data-ttu-id="52a4b-118">Datum</span><span class="sxs-lookup"><span data-stu-id="52a4b-118">Date</span></span>   |
| <span data-ttu-id="52a4b-119">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="52a4b-119">reportPeriod</span></span>      | <span data-ttu-id="52a4b-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52a4b-120">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="52a4b-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="52a4b-121">JSON representation</span></span>

<span data-ttu-id="52a4b-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="52a4b-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "viewedOrEdited": 1024, 
  "synced": 1024, 
  "sharedInternally": 1024, 
  "sharedExternally": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
