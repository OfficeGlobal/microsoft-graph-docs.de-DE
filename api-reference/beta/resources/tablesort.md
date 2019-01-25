---
title: TableSort-Ressourcentyp
description: Verwaltet Sortiervorgänge für Table-Objekte.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 612e0cb7d59011f04ae992f80119fc1da572b582
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511744"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="78a4f-103">TableSort-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="78a4f-103">TableSort resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78a4f-104">Verwaltet Sortiervorgänge für Table-Objekte.</span><span class="sxs-lookup"><span data-stu-id="78a4f-104">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="78a4f-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="78a4f-105">Methods</span></span>

| <span data-ttu-id="78a4f-106">Methode</span><span class="sxs-lookup"><span data-stu-id="78a4f-106">Method</span></span>           | <span data-ttu-id="78a4f-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="78a4f-107">Return Type</span></span>    |<span data-ttu-id="78a4f-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78a4f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78a4f-109">Get TableSort</span><span class="sxs-lookup"><span data-stu-id="78a4f-109">[Get TableSort](../api/tablesort-get.md)</span></span> | [<span data-ttu-id="78a4f-110">TableSort</span><span class="sxs-lookup"><span data-stu-id="78a4f-110">TableSort</span></span>](tablesort.md) |<span data-ttu-id="78a4f-111">Dient zum Lesen der Eigenschaften und der Beziehungen des tableSort-Objekts.</span><span class="sxs-lookup"><span data-stu-id="78a4f-111">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="78a4f-112">Apply</span><span class="sxs-lookup"><span data-stu-id="78a4f-112">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="78a4f-113">Keine</span><span class="sxs-lookup"><span data-stu-id="78a4f-113">None</span></span>|<span data-ttu-id="78a4f-114">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="78a4f-114">Perform a sort operation.</span></span>|
|[<span data-ttu-id="78a4f-115">Clear</span><span class="sxs-lookup"><span data-stu-id="78a4f-115">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="78a4f-116">Keine</span><span class="sxs-lookup"><span data-stu-id="78a4f-116">None</span></span>|<span data-ttu-id="78a4f-p101">Löscht die Sortierung, die derzeit in der Tabelle enthalten ist. Dies ändert nicht die Sortierung der Tabelle, löscht jedoch den Zustand der Kopfzeilen-Schaltflächen.</span><span class="sxs-lookup"><span data-stu-id="78a4f-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="78a4f-119">Reapply</span><span class="sxs-lookup"><span data-stu-id="78a4f-119">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="78a4f-120">Keine</span><span class="sxs-lookup"><span data-stu-id="78a4f-120">None</span></span>|<span data-ttu-id="78a4f-121">Wendet die aktuellen Sortierparameter erneut auf die Tabelle an.</span><span class="sxs-lookup"><span data-stu-id="78a4f-121">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="78a4f-122">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="78a4f-122">Properties</span></span>
| <span data-ttu-id="78a4f-123">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="78a4f-123">Property</span></span>     | <span data-ttu-id="78a4f-124">Typ</span><span class="sxs-lookup"><span data-stu-id="78a4f-124">Type</span></span>   |<span data-ttu-id="78a4f-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78a4f-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78a4f-126">matchCase</span><span class="sxs-lookup"><span data-stu-id="78a4f-126">matchCase</span></span>|<span data-ttu-id="78a4f-127">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="78a4f-127">boolean</span></span>|<span data-ttu-id="78a4f-p102">Stellt dar, ob die Groß-/Kleinschreibung den letzten Sortiervorgang der Tabelle beeinflusst hat. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="78a4f-p102">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="78a4f-130">method</span><span class="sxs-lookup"><span data-stu-id="78a4f-130">method</span></span>|<span data-ttu-id="78a4f-131">string</span><span class="sxs-lookup"><span data-stu-id="78a4f-131">string</span></span>|<span data-ttu-id="78a4f-p103">Stellt die chinesische Zeichensortiermethode dar, mit der die Tabelle zuletzt sortiert wurde. Die folgenden Werte sind möglich: `PinYin`, `StrokeCount`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="78a4f-p103">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78a4f-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="78a4f-135">Relationships</span></span>
| <span data-ttu-id="78a4f-136">Beziehung</span><span class="sxs-lookup"><span data-stu-id="78a4f-136">Relationship</span></span> | <span data-ttu-id="78a4f-137">Typ</span><span class="sxs-lookup"><span data-stu-id="78a4f-137">Type</span></span>   |<span data-ttu-id="78a4f-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="78a4f-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78a4f-139">fields</span><span class="sxs-lookup"><span data-stu-id="78a4f-139">fields</span></span>|[<span data-ttu-id="78a4f-140">SortField</span><span class="sxs-lookup"><span data-stu-id="78a4f-140">SortField</span></span>](sortfield.md)|<span data-ttu-id="78a4f-p104">Stellt die aktuellen Bedingungen dar, die zuletzt zum Sortieren der Tabelle verwendet wurden. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="78a4f-p104">Represents the current conditions used to last sort the table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78a4f-143">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="78a4f-143">JSON representation</span></span>

<span data-ttu-id="78a4f-144">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="78a4f-144">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/tablesort.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
