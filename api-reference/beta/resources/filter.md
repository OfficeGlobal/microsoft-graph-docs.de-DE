---
title: Filter-Ressourcentyp
description: Verwaltet das Filtern der Spalte einer Tabelle.
ms.openlocfilehash: df896d10b1e8734015d38b92b5824e3e3652e3a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062736"
---
# <a name="filter-resource-type"></a><span data-ttu-id="8eb22-103">Filter-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8eb22-103">Filter resource type</span></span>

> <span data-ttu-id="8eb22-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8eb22-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8eb22-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8eb22-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8eb22-106">Verwaltet das Filtern der Spalte einer Tabelle.</span><span class="sxs-lookup"><span data-stu-id="8eb22-106">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="8eb22-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="8eb22-107">Methods</span></span>

| <span data-ttu-id="8eb22-108">Methode</span><span class="sxs-lookup"><span data-stu-id="8eb22-108">Method</span></span>           | <span data-ttu-id="8eb22-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8eb22-109">Return Type</span></span>    |<span data-ttu-id="8eb22-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8eb22-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8eb22-111">Apply</span><span class="sxs-lookup"><span data-stu-id="8eb22-111">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="8eb22-112">Keine</span><span class="sxs-lookup"><span data-stu-id="8eb22-112">None</span></span>|<span data-ttu-id="8eb22-113">Wendet die angegebenen Filterkriterien in der angegebenen Spalte an.</span><span class="sxs-lookup"><span data-stu-id="8eb22-113">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="8eb22-114">Löschen</span><span class="sxs-lookup"><span data-stu-id="8eb22-114">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="8eb22-115">Keine</span><span class="sxs-lookup"><span data-stu-id="8eb22-115">None</span></span>|<span data-ttu-id="8eb22-116">Deaktiviert den Filter für die angegebene Spalte.</span><span class="sxs-lookup"><span data-stu-id="8eb22-116">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="8eb22-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8eb22-117">Properties</span></span>
<span data-ttu-id="8eb22-118">Keine</span><span class="sxs-lookup"><span data-stu-id="8eb22-118">None</span></span>

## <a name="relationships"></a><span data-ttu-id="8eb22-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8eb22-119">Relationships</span></span>
| <span data-ttu-id="8eb22-120">Beziehung</span><span class="sxs-lookup"><span data-stu-id="8eb22-120">Relationship</span></span> | <span data-ttu-id="8eb22-121">Typ</span><span class="sxs-lookup"><span data-stu-id="8eb22-121">Type</span></span>   |<span data-ttu-id="8eb22-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8eb22-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8eb22-123">criteria</span><span class="sxs-lookup"><span data-stu-id="8eb22-123">criteria</span></span>|[<span data-ttu-id="8eb22-124">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="8eb22-124">FilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="8eb22-p102">Der aktuell angewendete Filter in der angegebenen Spalte. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="8eb22-p102">The currently applied filter on the given column. Read-only.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->