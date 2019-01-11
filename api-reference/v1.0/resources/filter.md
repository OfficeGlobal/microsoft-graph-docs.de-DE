---
title: Filter-Ressourcentyp
description: Verwaltet das Filtern der Spalte einer Tabelle.
localization_priority: Normal
ms.openlocfilehash: cc4b1b105c2049b36fa27cb88b41102366648fa8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834664"
---
# <a name="filter-resource-type"></a><span data-ttu-id="4545b-103">Filter-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4545b-103">Filter resource type</span></span>

<span data-ttu-id="4545b-104">Verwaltet das Filtern der Spalte einer Tabelle.</span><span class="sxs-lookup"><span data-stu-id="4545b-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="4545b-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="4545b-105">Methods</span></span>

| <span data-ttu-id="4545b-106">Methode</span><span class="sxs-lookup"><span data-stu-id="4545b-106">Method</span></span>           | <span data-ttu-id="4545b-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="4545b-107">Return Type</span></span>    |<span data-ttu-id="4545b-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4545b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4545b-109">Apply</span><span class="sxs-lookup"><span data-stu-id="4545b-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="4545b-110">Keine</span><span class="sxs-lookup"><span data-stu-id="4545b-110">None</span></span>|<span data-ttu-id="4545b-111">Wendet die angegebenen Filterkriterien in der angegebenen Spalte an.</span><span class="sxs-lookup"><span data-stu-id="4545b-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="4545b-112">Clear</span><span class="sxs-lookup"><span data-stu-id="4545b-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="4545b-113">Keine</span><span class="sxs-lookup"><span data-stu-id="4545b-113">None</span></span>|<span data-ttu-id="4545b-114">Deaktiviert den Filter für die angegebene Spalte.</span><span class="sxs-lookup"><span data-stu-id="4545b-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="4545b-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4545b-115">Properties</span></span>

| <span data-ttu-id="4545b-116">Name</span><span class="sxs-lookup"><span data-stu-id="4545b-116">Name</span></span> | <span data-ttu-id="4545b-117">Typ</span><span class="sxs-lookup"><span data-stu-id="4545b-117">Type</span></span>   |<span data-ttu-id="4545b-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4545b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4545b-119">criteria</span><span class="sxs-lookup"><span data-stu-id="4545b-119">criteria</span></span>|[<span data-ttu-id="4545b-120">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="4545b-120">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="4545b-p101">Der aktuell angewendete Filter in der angegebenen Spalte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="4545b-p101">The currently applied filter on the given column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4545b-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4545b-123">JSON representation</span></span>

<span data-ttu-id="4545b-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4545b-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
  "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
