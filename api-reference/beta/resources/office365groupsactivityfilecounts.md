---
title: Ressourcentyp office365GroupsActivityFileCounts
description: Es folgt eine JSON-Darstellung der Ressource.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: adff009d9047aa147c8042059fbdab8491288fb7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972558"
---
# <a name="office365groupsactivityfilecounts-resource-type"></a><span data-ttu-id="9d567-103">Ressourcentyp office365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="9d567-103">office365GroupsActivityFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="9d567-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9d567-104">Properties</span></span>

| <span data-ttu-id="9d567-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9d567-105">Property</span></span>          | <span data-ttu-id="9d567-106">Typ</span><span class="sxs-lookup"><span data-stu-id="9d567-106">Type</span></span>   | <span data-ttu-id="9d567-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d567-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="9d567-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9d567-108">reportRefreshDate</span></span> | <span data-ttu-id="9d567-109">Datum</span><span class="sxs-lookup"><span data-stu-id="9d567-109">Date</span></span>   | <span data-ttu-id="9d567-110">Das aktuelle Datum des Inhalts.</span><span class="sxs-lookup"><span data-stu-id="9d567-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="9d567-111">gesamt</span><span class="sxs-lookup"><span data-stu-id="9d567-111">total</span></span>             | <span data-ttu-id="9d567-112">Int64</span><span class="sxs-lookup"><span data-stu-id="9d567-112">Int64</span></span>  | <span data-ttu-id="9d567-113">Die Gesamtzahl der Dateien in der Gruppe SharePoint-Dokumentbibliothek.</span><span class="sxs-lookup"><span data-stu-id="9d567-113">The total number of files in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="9d567-114">aktive</span><span class="sxs-lookup"><span data-stu-id="9d567-114">active</span></span>            | <span data-ttu-id="9d567-115">Int64</span><span class="sxs-lookup"><span data-stu-id="9d567-115">Int64</span></span>  | <span data-ttu-id="9d567-116">Die Anzahl der Dateien, die angezeigt wurden, bearbeitet, freigegebene oder in der Gruppe SharePoint-Dokumentbibliothek synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="9d567-116">The number of files that were viewed, edited, shared, or synced in the group's SharePoint document library.</span></span> |
| <span data-ttu-id="9d567-117">reportDate</span><span class="sxs-lookup"><span data-stu-id="9d567-117">reportDate</span></span>        | <span data-ttu-id="9d567-118">Datum</span><span class="sxs-lookup"><span data-stu-id="9d567-118">Date</span></span>   | <span data-ttu-id="9d567-119">Das Datum, an dem eine Reihe von Dateien in der Gruppe SharePoint-Website aktiv waren.</span><span class="sxs-lookup"><span data-stu-id="9d567-119">The date on which a number of files were active in the group's SharePoint site.</span></span> |
| <span data-ttu-id="9d567-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="9d567-120">reportPeriod</span></span>      | <span data-ttu-id="9d567-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9d567-121">String</span></span> | <span data-ttu-id="9d567-122">Die Anzahl der Tage, die der Bericht wird behandelt.</span><span class="sxs-lookup"><span data-stu-id="9d567-122">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="9d567-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9d567-123">JSON representation</span></span>

<span data-ttu-id="9d567-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9d567-124">The following is a JSON representation of the resource.</span></span>

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
