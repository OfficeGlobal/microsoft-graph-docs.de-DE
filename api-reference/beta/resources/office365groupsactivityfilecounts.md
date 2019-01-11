---
title: Ressourcentyp office365GroupsActivityFileCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.openlocfilehash: 856bb4c74c8af35775b6fe71cb75d89935440bdb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819186"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="ada29-103">Ressourcentyp office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="ada29-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ada29-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ada29-104">Properties</span></span>

| <span data-ttu-id="ada29-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ada29-105">Property</span></span>          | <span data-ttu-id="ada29-106">Typ</span><span class="sxs-lookup"><span data-stu-id="ada29-106">Type</span></span>   | <span data-ttu-id="ada29-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ada29-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="ada29-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ada29-108">reportRefreshDate</span></span> | <span data-ttu-id="ada29-109">Datum</span><span class="sxs-lookup"><span data-stu-id="ada29-109">Date</span></span>   | <span data-ttu-id="ada29-110">Das aktuelle Datum des Inhalts.</span><span class="sxs-lookup"><span data-stu-id="ada29-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="ada29-111">gesamt</span><span class="sxs-lookup"><span data-stu-id="ada29-111">total</span></span>             | <span data-ttu-id="ada29-112">Int64</span><span class="sxs-lookup"><span data-stu-id="ada29-112">Int64</span></span>  | <span data-ttu-id="ada29-113">Die Gesamtzahl der Dateien in der Gruppe SharePoint-Dokumentbibliothek.</span><span class="sxs-lookup"><span data-stu-id="ada29-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="ada29-114">aktive</span><span class="sxs-lookup"><span data-stu-id="ada29-114">active</span></span>            | <span data-ttu-id="ada29-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ada29-115">Int64</span></span>  | <span data-ttu-id="ada29-116">Die Anzahl der Dateien, die angezeigt wurden, bearbeitet, freigegebene oder in der Gruppe SharePoint-Dokumentbibliothek synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="ada29-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="ada29-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="ada29-117">reportDate</span></span>        | <span data-ttu-id="ada29-118">Datum</span><span class="sxs-lookup"><span data-stu-id="ada29-118">Date</span></span>   | <span data-ttu-id="ada29-119">Das Datum, an dem eine Reihe von Dateien in der Gruppe SharePoint-Website aktiv waren.</span><span class="sxs-lookup"><span data-stu-id="ada29-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="ada29-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ada29-120">reportPeriod</span></span>      | <span data-ttu-id="ada29-121">String</span><span class="sxs-lookup"><span data-stu-id="ada29-121">String</span></span> | <span data-ttu-id="ada29-122">Die Anzahl der Tage, die der Bericht wird behandelt.</span><span class="sxs-lookup"><span data-stu-id="ada29-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="ada29-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ada29-123">JSON representation</span></span>

<span data-ttu-id="ada29-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ada29-124">The following is a JSON representation of the resource.</span></span>

<!-- {

  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityFileCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
