---
title: Ressourcentyp office365GroupsActivityStorage
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0485fd95046bc83350983bc1333dba83c79139d6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576381"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="8495d-103">Ressourcentyp office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="8495d-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8495d-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8495d-104">Properties</span></span>

| <span data-ttu-id="8495d-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8495d-105">Property</span></span>                  | <span data-ttu-id="8495d-106">Typ</span><span class="sxs-lookup"><span data-stu-id="8495d-106">Type</span></span>   | <span data-ttu-id="8495d-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8495d-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="8495d-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8495d-108">reportRefreshDate</span></span>         | <span data-ttu-id="8495d-109">Date</span><span class="sxs-lookup"><span data-stu-id="8495d-109">Date</span></span>   | <span data-ttu-id="8495d-110">Das aktuelle Datum des Inhalts.</span><span class="sxs-lookup"><span data-stu-id="8495d-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="8495d-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="8495d-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="8495d-112">Int64</span><span class="sxs-lookup"><span data-stu-id="8495d-112">Int64</span></span>  | <span data-ttu-id="8495d-113">Der Speicher, die in der Gruppenpostfach verwendet.</span><span class="sxs-lookup"><span data-stu-id="8495d-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="8495d-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="8495d-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="8495d-115">Int64</span><span class="sxs-lookup"><span data-stu-id="8495d-115">Int64</span></span>  | <span data-ttu-id="8495d-116">Der Speicher in SharePoint-Dokumentbibliothek verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="8495d-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="8495d-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="8495d-117">reportDate</span></span>                | <span data-ttu-id="8495d-118">Date</span><span class="sxs-lookup"><span data-stu-id="8495d-118">Date</span></span>   | <span data-ttu-id="8495d-119">Das Datum Snapshot für Exchange und SharePoint verwendet Speicher.</span><span class="sxs-lookup"><span data-stu-id="8495d-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="8495d-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8495d-120">reportPeriod</span></span>              | <span data-ttu-id="8495d-121">String</span><span class="sxs-lookup"><span data-stu-id="8495d-121">String</span></span> | <span data-ttu-id="8495d-122">Die Anzahl der Tage, die der Bericht wird behandelt.</span><span class="sxs-lookup"><span data-stu-id="8495d-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="8495d-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8495d-123">JSON representation</span></span>

<span data-ttu-id="8495d-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8495d-124">The following is a JSON representation of the resource.</span></span>

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
