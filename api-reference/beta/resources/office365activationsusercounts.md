---
title: Ressourcentyp office365ActivationsUserCounts
description: Es folgt eine JSON-Darstellung der Ressource.
ms.openlocfilehash: 90d9d2d8616f166eb9d8b87967898daa0468db54
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064738"
---
# <a name="office365activationsusercounts-resource-type"></a><span data-ttu-id="f1934-103">Ressourcentyp office365ActivationsUserCounts</span><span class="sxs-lookup"><span data-stu-id="f1934-103">office365ActivationsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f1934-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f1934-104">Properties</span></span>

| <span data-ttu-id="f1934-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f1934-105">Property</span></span>                 | <span data-ttu-id="f1934-106">Typ</span><span class="sxs-lookup"><span data-stu-id="f1934-106">Type</span></span>   | <span data-ttu-id="f1934-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1934-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="f1934-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f1934-108">reportRefreshDate</span></span>        | <span data-ttu-id="f1934-109">Datum</span><span class="sxs-lookup"><span data-stu-id="f1934-109">Date</span></span>   | <span data-ttu-id="f1934-110">Das aktuelle Datum des Inhalts.</span><span class="sxs-lookup"><span data-stu-id="f1934-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="f1934-111">productType</span><span class="sxs-lookup"><span data-stu-id="f1934-111">productType</span></span>              | <span data-ttu-id="f1934-112">String</span><span class="sxs-lookup"><span data-stu-id="f1934-112">String</span></span> | <span data-ttu-id="f1934-113">Der Produkttyp wie "Office 365 ProPlus", "Project-Client" oder "Visio Pro für Office 365".</span><span class="sxs-lookup"><span data-stu-id="f1934-113">The product type such as "Office 365 ProPlus", "Project Client", or "Visio Pro for Office 365".</span></span> |
| <span data-ttu-id="f1934-114">zugewiesen</span><span class="sxs-lookup"><span data-stu-id="f1934-114">assigned</span></span>                 | <span data-ttu-id="f1934-115">Int64</span><span class="sxs-lookup"><span data-stu-id="f1934-115">Int64</span></span>  | <span data-ttu-id="f1934-116">Die Anzahl der Benutzer ist für die Produktlizenz zugewiesen worden.</span><span class="sxs-lookup"><span data-stu-id="f1934-116">The number of users have been assigned for the product license.</span></span> |
| <span data-ttu-id="f1934-117">aktiviert</span><span class="sxs-lookup"><span data-stu-id="f1934-117">activated</span></span>                | <span data-ttu-id="f1934-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f1934-118">Int64</span></span>  | <span data-ttu-id="f1934-119">Die Anzahl der Benutzer, die das Produkt aktiviert haben.</span><span class="sxs-lookup"><span data-stu-id="f1934-119">The number of users who have activated the product.</span></span> |
| <span data-ttu-id="f1934-120">sharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="f1934-120">sharedComputerActivation</span></span> | <span data-ttu-id="f1934-121">Int64</span><span class="sxs-lookup"><span data-stu-id="f1934-121">Int64</span></span>  | <span data-ttu-id="f1934-122">Die Anzahl der Benutzer, die das Produkt auf einem freigegebenen Computer verwendet haben.</span><span class="sxs-lookup"><span data-stu-id="f1934-122">The number of users who have used the product on a shared computer.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f1934-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f1934-123">JSON representation</span></span>

<span data-ttu-id="f1934-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f1934-124">The following is a JSON representation of the resource.</span></span>

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
