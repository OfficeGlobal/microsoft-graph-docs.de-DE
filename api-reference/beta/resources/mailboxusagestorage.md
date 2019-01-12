---
title: Ressourcentyp mailboxUsageStorage
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 44b97c7b18264e01c86b34bfd8265246f80ab031
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917867"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="cbb10-103">Ressourcentyp mailboxUsageStorage</span><span class="sxs-lookup"><span data-stu-id="cbb10-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="cbb10-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cbb10-104">Properties</span></span>

| <span data-ttu-id="cbb10-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cbb10-105">Property</span></span>           | <span data-ttu-id="cbb10-106">Typ</span><span class="sxs-lookup"><span data-stu-id="cbb10-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="cbb10-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="cbb10-107">reportRefreshDate</span></span>  | <span data-ttu-id="cbb10-108">Datum</span><span class="sxs-lookup"><span data-stu-id="cbb10-108">Date</span></span>   |
| <span data-ttu-id="cbb10-109">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="cbb10-109">storageUsedInBytes</span></span> | <span data-ttu-id="cbb10-110">Int64</span><span class="sxs-lookup"><span data-stu-id="cbb10-110">Int64</span></span>  |
| <span data-ttu-id="cbb10-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="cbb10-111">reportDate</span></span>         | <span data-ttu-id="cbb10-112">Datum</span><span class="sxs-lookup"><span data-stu-id="cbb10-112">Date</span></span>   |
| <span data-ttu-id="cbb10-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="cbb10-113">reportPeriod</span></span>       | <span data-ttu-id="cbb10-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cbb10-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cbb10-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cbb10-115">JSON representation</span></span>

<span data-ttu-id="cbb10-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cbb10-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
