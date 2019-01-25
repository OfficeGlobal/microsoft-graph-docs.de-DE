---
title: Filter-Ressourcentyp
description: Verwaltet das Filtern der Spalte einer Tabelle.
localization_priority: Normal
ms.openlocfilehash: 6adc4e378b47bcb134a640e77bf54c32a35b3be2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518891"
---
# <a name="filter-resource-type"></a><span data-ttu-id="d1d64-103">Filter-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d1d64-103">Filter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1d64-104">Verwaltet das Filtern der Spalte einer Tabelle.</span><span class="sxs-lookup"><span data-stu-id="d1d64-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="d1d64-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="d1d64-105">Methods</span></span>

| <span data-ttu-id="d1d64-106">Methode</span><span class="sxs-lookup"><span data-stu-id="d1d64-106">Method</span></span>           | <span data-ttu-id="d1d64-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d1d64-107">Return Type</span></span>    |<span data-ttu-id="d1d64-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1d64-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d1d64-109">Apply</span><span class="sxs-lookup"><span data-stu-id="d1d64-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="d1d64-110">Keine</span><span class="sxs-lookup"><span data-stu-id="d1d64-110">None</span></span>|<span data-ttu-id="d1d64-111">Wendet die angegebenen Filterkriterien in der angegebenen Spalte an.</span><span class="sxs-lookup"><span data-stu-id="d1d64-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="d1d64-112">Clear</span><span class="sxs-lookup"><span data-stu-id="d1d64-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="d1d64-113">Keine</span><span class="sxs-lookup"><span data-stu-id="d1d64-113">None</span></span>|<span data-ttu-id="d1d64-114">Deaktiviert den Filter für die angegebene Spalte.</span><span class="sxs-lookup"><span data-stu-id="d1d64-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="d1d64-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d1d64-115">Properties</span></span>
<span data-ttu-id="d1d64-116">Keine</span><span class="sxs-lookup"><span data-stu-id="d1d64-116">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d1d64-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d1d64-117">Relationships</span></span>
| <span data-ttu-id="d1d64-118">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d1d64-118">Relationship</span></span> | <span data-ttu-id="d1d64-119">Typ</span><span class="sxs-lookup"><span data-stu-id="d1d64-119">Type</span></span>   |<span data-ttu-id="d1d64-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1d64-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d1d64-121">criteria</span><span class="sxs-lookup"><span data-stu-id="d1d64-121">criteria</span></span>|[<span data-ttu-id="d1d64-122">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="d1d64-122">FilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="d1d64-p101">Der aktuell angewendete Filter in der angegebenen Spalte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d1d64-p101">The currently applied filter on the given column. Read-only.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/filter.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
