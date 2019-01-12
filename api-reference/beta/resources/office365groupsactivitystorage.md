---
title: Ressourcentyp office365GroupsActivityStorage
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 180e60a52b397f969aa10cee5bc27bba934ad1e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944453"
---
# <a name="office365groupsactivitystorage-resource-type"></a><span data-ttu-id="91f62-103">Ressourcentyp office365GroupsActivityStorage</span><span class="sxs-lookup"><span data-stu-id="91f62-103">office365GroupsActivityStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="91f62-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="91f62-104">Properties</span></span>

| <span data-ttu-id="91f62-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="91f62-105">Property</span></span>                  | <span data-ttu-id="91f62-106">Typ</span><span class="sxs-lookup"><span data-stu-id="91f62-106">Type</span></span>   | <span data-ttu-id="91f62-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91f62-107">Description</span></span>                              |
| :------------------------ | :----- | ---------------------------------------- |
| <span data-ttu-id="91f62-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="91f62-108">reportRefreshDate</span></span>         | <span data-ttu-id="91f62-109">Datum</span><span class="sxs-lookup"><span data-stu-id="91f62-109">Date</span></span>   | <span data-ttu-id="91f62-110">Das aktuelle Datum des Inhalts.</span><span class="sxs-lookup"><span data-stu-id="91f62-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="91f62-111">mailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="91f62-111">mailboxStorageUsedInBytes</span></span> | <span data-ttu-id="91f62-112">Int64</span><span class="sxs-lookup"><span data-stu-id="91f62-112">Int64</span></span>  | <span data-ttu-id="91f62-113">Der Speicher, die in der Gruppenpostfach verwendet.</span><span class="sxs-lookup"><span data-stu-id="91f62-113">The storage used in group mailbox.</span></span>       |
| <span data-ttu-id="91f62-114">siteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="91f62-114">siteStorageUsedInBytes</span></span>    | <span data-ttu-id="91f62-115">Int64</span><span class="sxs-lookup"><span data-stu-id="91f62-115">Int64</span></span>  | <span data-ttu-id="91f62-116">Der Speicher in SharePoint-Dokumentbibliothek verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="91f62-116">The storage used in SharePoint document library.</span></span> |
| <span data-ttu-id="91f62-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="91f62-117">reportDate</span></span>                | <span data-ttu-id="91f62-118">Datum</span><span class="sxs-lookup"><span data-stu-id="91f62-118">Date</span></span>   | <span data-ttu-id="91f62-119">Das Datum Snapshot für Exchange und SharePoint verwendet Speicher.</span><span class="sxs-lookup"><span data-stu-id="91f62-119">The snapshot date for Exchange and SharePoint used storage.</span></span> |
| <span data-ttu-id="91f62-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="91f62-120">reportPeriod</span></span>              | <span data-ttu-id="91f62-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="91f62-121">String</span></span> | <span data-ttu-id="91f62-122">Die Anzahl der Tage, die der Bericht wird behandelt.</span><span class="sxs-lookup"><span data-stu-id="91f62-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="91f62-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="91f62-123">JSON representation</span></span>

<span data-ttu-id="91f62-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="91f62-124">The following is a JSON representation of the resource.</span></span>

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
