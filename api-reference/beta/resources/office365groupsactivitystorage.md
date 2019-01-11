---
title: Ressourcentyp office365GroupsActivityStorage
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 9824d3d172a8578f8a25a049c2d0d3b407bbc47e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862251"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="d62c8-103">Ressourcentyp office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="d62c8-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d62c8-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d62c8-104">Properties</span></span>

| <span data-ttu-id="d62c8-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d62c8-105">Property</span></span>                  | <span data-ttu-id="d62c8-106">Typ</span><span class="sxs-lookup"><span data-stu-id="d62c8-106">Type</span></span>   | <span data-ttu-id="d62c8-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d62c8-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="d62c8-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d62c8-108">reportRefreshDate</span></span>         | <span data-ttu-id="d62c8-109">Datum</span><span class="sxs-lookup"><span data-stu-id="d62c8-109">Date</span></span>   | <span data-ttu-id="d62c8-110">Das aktuelle Datum des Inhalts.</span><span class="sxs-lookup"><span data-stu-id="d62c8-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="d62c8-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="d62c8-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="d62c8-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d62c8-112">Int64</span></span>  | <span data-ttu-id="d62c8-113">Der Speicher, die in der Gruppenpostfach verwendet.</span><span class="sxs-lookup"><span data-stu-id="d62c8-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="d62c8-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="d62c8-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="d62c8-115">Int64</span><span class="sxs-lookup"><span data-stu-id="d62c8-115">Int64</span></span>  | <span data-ttu-id="d62c8-116">Der Speicher in SharePoint-Dokumentbibliothek verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="d62c8-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="d62c8-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="d62c8-117">reportDate</span></span>                | <span data-ttu-id="d62c8-118">Datum</span><span class="sxs-lookup"><span data-stu-id="d62c8-118">Date</span></span>   | <span data-ttu-id="d62c8-119">Das Datum Snapshot für Exchange und SharePoint verwendet Speicher.</span><span class="sxs-lookup"><span data-stu-id="d62c8-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="d62c8-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d62c8-120">reportPeriod</span></span>              | <span data-ttu-id="d62c8-121">String</span><span class="sxs-lookup"><span data-stu-id="d62c8-121">String</span></span> | <span data-ttu-id="d62c8-122">Die Anzahl der Tage, die der Bericht wird behandelt.</span><span class="sxs-lookup"><span data-stu-id="d62c8-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="d62c8-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d62c8-123">JSON representation</span></span>

<span data-ttu-id="d62c8-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d62c8-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailboxStorageUsedInBytes": 1024, 
  "siteStorageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
