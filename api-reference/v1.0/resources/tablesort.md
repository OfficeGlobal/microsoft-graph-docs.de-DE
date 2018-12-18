---
title: TableSort-Ressourcentyp
description: Verwaltet Sortiervorgänge für Table-Objekte.
author: lumine2008
ms.openlocfilehash: 1d40182fbd92da0022136cb694928397e468d7ac
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346977"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="da835-103">TableSort-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="da835-103">TableSort resource type</span></span>

<span data-ttu-id="da835-104">Verwaltet Sortiervorgänge für Table-Objekte.</span><span class="sxs-lookup"><span data-stu-id="da835-104">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="da835-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="da835-105">Methods</span></span>

| <span data-ttu-id="da835-106">Methode</span><span class="sxs-lookup"><span data-stu-id="da835-106">Method</span></span>           | <span data-ttu-id="da835-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="da835-107">Return Type</span></span>    |<span data-ttu-id="da835-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da835-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="da835-109">Get TableSort</span><span class="sxs-lookup"><span data-stu-id="da835-109">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="da835-110">WorkbookTableSort</span><span class="sxs-lookup"><span data-stu-id="da835-110">WorkbookTableSort</span></span>](tablesort.md) |<span data-ttu-id="da835-111">Dient zum Lesen der Eigenschaften und der Beziehungen des tableSort-Objekts.</span><span class="sxs-lookup"><span data-stu-id="da835-111">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="da835-112">Apply</span><span class="sxs-lookup"><span data-stu-id="da835-112">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="da835-113">Keine</span><span class="sxs-lookup"><span data-stu-id="da835-113">None</span></span>|<span data-ttu-id="da835-114">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="da835-114">Perform a sort operation.</span></span>|
|[<span data-ttu-id="da835-115">Löschen</span><span class="sxs-lookup"><span data-stu-id="da835-115">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="da835-116">Keine</span><span class="sxs-lookup"><span data-stu-id="da835-116">None</span></span>|<span data-ttu-id="da835-p101">Löscht die Sortierung, die derzeit in der Tabelle enthalten ist. Dies ändert nicht die Sortierung der Tabelle, löscht jedoch den Zustand der Kopfzeilen-Schaltflächen.</span><span class="sxs-lookup"><span data-stu-id="da835-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="da835-119">Reapply</span><span class="sxs-lookup"><span data-stu-id="da835-119">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="da835-120">Keine</span><span class="sxs-lookup"><span data-stu-id="da835-120">None</span></span>|<span data-ttu-id="da835-121">Wendet die aktuellen Sortierparameter erneut auf die Tabelle an.</span><span class="sxs-lookup"><span data-stu-id="da835-121">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="da835-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="da835-122">Properties</span></span>
| <span data-ttu-id="da835-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="da835-123">Property</span></span>     | <span data-ttu-id="da835-124">Typ</span><span class="sxs-lookup"><span data-stu-id="da835-124">Type</span></span>   |<span data-ttu-id="da835-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da835-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da835-126">fields</span><span class="sxs-lookup"><span data-stu-id="da835-126">fields</span></span>|<span data-ttu-id="da835-127">[WorkbookSortField](sortfield.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="da835-127">[WorkbookSortField](sortfield.md) collection</span></span>|<span data-ttu-id="da835-p102">Stellt die aktuellen Bedingungen dar, die zuletzt zum Sortieren der Tabelle verwendet wurden. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="da835-p102">Represents the current conditions used to last sort the table. Read-only.</span></span>|
|<span data-ttu-id="da835-130">matchCase</span><span class="sxs-lookup"><span data-stu-id="da835-130">matchCase</span></span>|<span data-ttu-id="da835-131">boolean</span><span class="sxs-lookup"><span data-stu-id="da835-131">boolean</span></span>|<span data-ttu-id="da835-p103">Stellt dar, ob die Groß-/Kleinschreibung den letzten Sortiervorgang der Tabelle beeinflusst hat. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="da835-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="da835-134">method</span><span class="sxs-lookup"><span data-stu-id="da835-134">method</span></span>|<span data-ttu-id="da835-135">string</span><span class="sxs-lookup"><span data-stu-id="da835-135">string</span></span>|<span data-ttu-id="da835-136">Stellt Chinesisches Zeichen Sortierung Methode zuletzt verwendet, um die Tabelle zu sortieren.</span><span class="sxs-lookup"><span data-stu-id="da835-136">Represents Chinese character ordering method last used to sort the table.</span></span> <span data-ttu-id="da835-137">Die möglichen Werte sind: `PinYin`, `StrokeCount`.</span><span class="sxs-lookup"><span data-stu-id="da835-137">The possible values are: `PinYin`, `StrokeCount`.</span></span> <span data-ttu-id="da835-138">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="da835-138">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="da835-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="da835-139">JSON representation</span></span>

<span data-ttu-id="da835-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="da835-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
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