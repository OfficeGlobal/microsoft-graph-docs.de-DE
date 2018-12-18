---
title: TableSort-Ressourcentyp
description: Verwaltet Sortiervorgänge für Table-Objekte.
author: lumine2008
ms.openlocfilehash: 52ee5288698b236f7ee4d29eb75fdac5ad14fa0f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339823"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="0338d-103">TableSort-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0338d-103">TableSort resource type</span></span>

> <span data-ttu-id="0338d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0338d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0338d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0338d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0338d-106">Verwaltet Sortiervorgänge für Table-Objekte.</span><span class="sxs-lookup"><span data-stu-id="0338d-106">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="0338d-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="0338d-107">Methods</span></span>

| <span data-ttu-id="0338d-108">Methode</span><span class="sxs-lookup"><span data-stu-id="0338d-108">Method</span></span>           | <span data-ttu-id="0338d-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0338d-109">Return Type</span></span>    |<span data-ttu-id="0338d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0338d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0338d-111">Get TableSort</span><span class="sxs-lookup"><span data-stu-id="0338d-111">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="0338d-112">TableSort</span><span class="sxs-lookup"><span data-stu-id="0338d-112">TableSort</span></span>](tablesort.md) |<span data-ttu-id="0338d-113">Dient zum Lesen der Eigenschaften und der Beziehungen des tableSort-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0338d-113">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="0338d-114">Apply</span><span class="sxs-lookup"><span data-stu-id="0338d-114">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="0338d-115">Keine</span><span class="sxs-lookup"><span data-stu-id="0338d-115">None</span></span>|<span data-ttu-id="0338d-116">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="0338d-116">Perform a sort operation.</span></span>|
|[<span data-ttu-id="0338d-117">Löschen</span><span class="sxs-lookup"><span data-stu-id="0338d-117">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="0338d-118">Keine</span><span class="sxs-lookup"><span data-stu-id="0338d-118">None</span></span>|<span data-ttu-id="0338d-p102">Löscht die Sortierung, die derzeit in der Tabelle enthalten ist. Dies ändert nicht die Sortierung der Tabelle, löscht jedoch den Zustand der Kopfzeilen-Schaltflächen.</span><span class="sxs-lookup"><span data-stu-id="0338d-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="0338d-121">Reapply</span><span class="sxs-lookup"><span data-stu-id="0338d-121">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="0338d-122">Keine</span><span class="sxs-lookup"><span data-stu-id="0338d-122">None</span></span>|<span data-ttu-id="0338d-123">Wendet die aktuellen Sortierparameter erneut auf die Tabelle an.</span><span class="sxs-lookup"><span data-stu-id="0338d-123">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="0338d-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0338d-124">Properties</span></span>
| <span data-ttu-id="0338d-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0338d-125">Property</span></span>     | <span data-ttu-id="0338d-126">Typ</span><span class="sxs-lookup"><span data-stu-id="0338d-126">Type</span></span>   |<span data-ttu-id="0338d-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0338d-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0338d-128">matchCase</span><span class="sxs-lookup"><span data-stu-id="0338d-128">matchCase</span></span>|<span data-ttu-id="0338d-129">boolean</span><span class="sxs-lookup"><span data-stu-id="0338d-129">boolean</span></span>|<span data-ttu-id="0338d-p103">Stellt dar, ob die Groß-/Kleinschreibung den letzten Sortiervorgang der Tabelle beeinflusst hat. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0338d-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="0338d-132">method</span><span class="sxs-lookup"><span data-stu-id="0338d-132">method</span></span>|<span data-ttu-id="0338d-133">string</span><span class="sxs-lookup"><span data-stu-id="0338d-133">string</span></span>|<span data-ttu-id="0338d-p104">Stellt die chinesische Zeichensortiermethode dar, mit der die Tabelle zuletzt sortiert wurde. Die folgenden Werte sind möglich: `PinYin`, `StrokeCount`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0338d-p104">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0338d-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0338d-137">Relationships</span></span>
| <span data-ttu-id="0338d-138">Beziehung</span><span class="sxs-lookup"><span data-stu-id="0338d-138">Relationship</span></span> | <span data-ttu-id="0338d-139">Typ</span><span class="sxs-lookup"><span data-stu-id="0338d-139">Type</span></span>   |<span data-ttu-id="0338d-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0338d-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0338d-141">fields</span><span class="sxs-lookup"><span data-stu-id="0338d-141">fields</span></span>|[<span data-ttu-id="0338d-142">SortField</span><span class="sxs-lookup"><span data-stu-id="0338d-142">SortField</span></span>](sortfield.md)|<span data-ttu-id="0338d-p105">Stellt die aktuellen Bedingungen dar, die zuletzt zum Sortieren der Tabelle verwendet wurden. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0338d-p105">Represents the current conditions used to last sort the table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0338d-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0338d-145">JSON representation</span></span>

<span data-ttu-id="0338d-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0338d-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->