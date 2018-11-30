---
title: TableSort-Ressourcentyp
description: Verwaltet Sortiervorgänge für Table-Objekte.
ms.openlocfilehash: 02ee1f72bc53a3097c76cf9bab62a165fe3c56f8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066062"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="327cd-103">TableSort-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="327cd-103">TableSort resource type</span></span>

> <span data-ttu-id="327cd-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="327cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="327cd-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="327cd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="327cd-106">Verwaltet Sortiervorgänge für Table-Objekte.</span><span class="sxs-lookup"><span data-stu-id="327cd-106">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="327cd-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="327cd-107">Methods</span></span>

| <span data-ttu-id="327cd-108">Methode</span><span class="sxs-lookup"><span data-stu-id="327cd-108">Method</span></span>           | <span data-ttu-id="327cd-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="327cd-109">Return Type</span></span>    |<span data-ttu-id="327cd-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="327cd-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="327cd-111">Get TableSort</span><span class="sxs-lookup"><span data-stu-id="327cd-111">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="327cd-112">TableSort</span><span class="sxs-lookup"><span data-stu-id="327cd-112">TableSort</span></span>](tablesort.md) |<span data-ttu-id="327cd-113">Dient zum Lesen der Eigenschaften und der Beziehungen des tableSort-Objekts.</span><span class="sxs-lookup"><span data-stu-id="327cd-113">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="327cd-114">Apply</span><span class="sxs-lookup"><span data-stu-id="327cd-114">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="327cd-115">Keine</span><span class="sxs-lookup"><span data-stu-id="327cd-115">None</span></span>|<span data-ttu-id="327cd-116">Führt einen Sortiervorgang aus.</span><span class="sxs-lookup"><span data-stu-id="327cd-116">Perform a sort operation.</span></span>|
|[<span data-ttu-id="327cd-117">Löschen</span><span class="sxs-lookup"><span data-stu-id="327cd-117">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="327cd-118">Keine</span><span class="sxs-lookup"><span data-stu-id="327cd-118">None</span></span>|<span data-ttu-id="327cd-p102">Löscht die Sortierung, die derzeit in der Tabelle enthalten ist. Dies ändert nicht die Sortierung der Tabelle, löscht jedoch den Zustand der Kopfzeilen-Schaltflächen.</span><span class="sxs-lookup"><span data-stu-id="327cd-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="327cd-121">Reapply</span><span class="sxs-lookup"><span data-stu-id="327cd-121">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="327cd-122">Keine</span><span class="sxs-lookup"><span data-stu-id="327cd-122">None</span></span>|<span data-ttu-id="327cd-123">Wendet die aktuellen Sortierparameter erneut auf die Tabelle an.</span><span class="sxs-lookup"><span data-stu-id="327cd-123">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="327cd-124">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="327cd-124">Properties</span></span>
| <span data-ttu-id="327cd-125">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="327cd-125">Property</span></span>     | <span data-ttu-id="327cd-126">Typ</span><span class="sxs-lookup"><span data-stu-id="327cd-126">Type</span></span>   |<span data-ttu-id="327cd-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="327cd-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="327cd-128">matchCase</span><span class="sxs-lookup"><span data-stu-id="327cd-128">matchCase</span></span>|<span data-ttu-id="327cd-129">boolean</span><span class="sxs-lookup"><span data-stu-id="327cd-129">boolean</span></span>|<span data-ttu-id="327cd-p103">Stellt dar, ob die Groß-/Kleinschreibung den letzten Sortiervorgang der Tabelle beeinflusst hat. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="327cd-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="327cd-132">method</span><span class="sxs-lookup"><span data-stu-id="327cd-132">method</span></span>|<span data-ttu-id="327cd-133">string</span><span class="sxs-lookup"><span data-stu-id="327cd-133">string</span></span>|<span data-ttu-id="327cd-p104">Stellt die chinesische Zeichensortiermethode dar, mit der die Tabelle zuletzt sortiert wurde. Die folgenden Werte sind möglich: `PinYin`, `StrokeCount`. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="327cd-p104">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="327cd-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="327cd-137">Relationships</span></span>
| <span data-ttu-id="327cd-138">Beziehung</span><span class="sxs-lookup"><span data-stu-id="327cd-138">Relationship</span></span> | <span data-ttu-id="327cd-139">Typ</span><span class="sxs-lookup"><span data-stu-id="327cd-139">Type</span></span>   |<span data-ttu-id="327cd-140">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="327cd-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="327cd-141">fields</span><span class="sxs-lookup"><span data-stu-id="327cd-141">fields</span></span>|[<span data-ttu-id="327cd-142">SortField</span><span class="sxs-lookup"><span data-stu-id="327cd-142">SortField</span></span>](sortfield.md)|<span data-ttu-id="327cd-p105">Stellt die aktuellen Bedingungen dar, die zuletzt zum Sortieren der Tabelle verwendet wurden. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="327cd-p105">Represents the current conditions used to last sort the table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="327cd-145">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="327cd-145">JSON representation</span></span>

<span data-ttu-id="327cd-146">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="327cd-146">Here is a JSON representation of the resource.</span></span>

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