---
title: Ressourcentyp office365ActivationsUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3dc497e516f95f1e05167703f2b9f8aea6363a64
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917720"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="a05fe-103">Ressourcentyp office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="a05fe-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a05fe-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a05fe-104">Properties</span></span>

| <span data-ttu-id="a05fe-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a05fe-105">Property</span></span>                 | <span data-ttu-id="a05fe-106">Typ</span><span class="sxs-lookup"><span data-stu-id="a05fe-106">Type</span></span>   | <span data-ttu-id="a05fe-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a05fe-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="a05fe-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a05fe-108">reportRefreshDate</span></span>        | <span data-ttu-id="a05fe-109">Datum</span><span class="sxs-lookup"><span data-stu-id="a05fe-109">Date</span></span>   | <span data-ttu-id="a05fe-110">Das aktuelle Datum des Inhalts.</span><span class="sxs-lookup"><span data-stu-id="a05fe-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="a05fe-111">productType</span><span class="sxs-lookup"><span data-stu-id="a05fe-111">productType</span></span>              | <span data-ttu-id="a05fe-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a05fe-112">String</span></span> | <span data-ttu-id="a05fe-113">Der Produkttyp wie "Office 365 ProPlus", "Project-Client" oder "Visio Pro für Office 365".</span><span class="sxs-lookup"><span data-stu-id="a05fe-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="a05fe-114">zugewiesen</span><span class="sxs-lookup"><span data-stu-id="a05fe-114">assigned</span></span>                 | <span data-ttu-id="a05fe-115">Int64</span><span class="sxs-lookup"><span data-stu-id="a05fe-115">Int64</span></span>  | <span data-ttu-id="a05fe-116">Die Anzahl der Benutzer ist für die Produktlizenz zugewiesen worden.</span><span class="sxs-lookup"><span data-stu-id="a05fe-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="a05fe-117">aktiviert</span><span class="sxs-lookup"><span data-stu-id="a05fe-117">activated</span></span>                | <span data-ttu-id="a05fe-118">Int64</span><span class="sxs-lookup"><span data-stu-id="a05fe-118">Int64</span></span>  | <span data-ttu-id="a05fe-119">Die Anzahl der Benutzer, die das Produkt aktiviert haben.</span><span class="sxs-lookup"><span data-stu-id="a05fe-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="a05fe-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="a05fe-120">sharedComputerActivation</span></span> | <span data-ttu-id="a05fe-121">Int64</span><span class="sxs-lookup"><span data-stu-id="a05fe-121">Int64</span></span>  | <span data-ttu-id="a05fe-122">Die Anzahl der Benutzer, die das Produkt auf einem freigegebenen Computer verwendet haben.</span><span class="sxs-lookup"><span data-stu-id="a05fe-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a05fe-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a05fe-123">JSON representation</span></span>

<span data-ttu-id="a05fe-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a05fe-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "assigned": 1024, 
  "activated": 1024,
  "sharedComputerActivation": 1024
}
```
