---
title: TableColumn-Ressourcentyp
description: Stellt eine Spalte in einer Tabelle dar.
ms.openlocfilehash: 0195bde59ee2116b064b47b9659f682877efc16b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061685"
---
# <a name="tablecolumn-resource-type"></a><span data-ttu-id="d8243-103">TableColumn-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d8243-103">TableColumn resource type</span></span>

> <span data-ttu-id="d8243-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d8243-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8243-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d8243-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d8243-106">Stellt eine Spalte in einer Tabelle dar.</span><span class="sxs-lookup"><span data-stu-id="d8243-106">Represents a column in a table.</span></span>


## <a name="methods"></a><span data-ttu-id="d8243-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="d8243-107">Methods</span></span>

| <span data-ttu-id="d8243-108">Methode</span><span class="sxs-lookup"><span data-stu-id="d8243-108">Method</span></span>           | <span data-ttu-id="d8243-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d8243-109">Return Type</span></span>    |<span data-ttu-id="d8243-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d8243-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8243-111">TableColumn abrufen</span><span class="sxs-lookup"><span data-stu-id="d8243-111">Get TableColumn</span></span>](../api/tablecolumn-get.md) | [<span data-ttu-id="d8243-112">TableColumn</span><span class="sxs-lookup"><span data-stu-id="d8243-112">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="d8243-113">Dient zum Lesen der Eigenschaften und der Beziehungen des tableColumn-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d8243-113">Read properties and relationships of tableColumn object.</span></span>|
|[<span data-ttu-id="d8243-114">Update</span><span class="sxs-lookup"><span data-stu-id="d8243-114">Update</span></span>](../api/tablecolumn-update.md) | [<span data-ttu-id="d8243-115">TableColumn</span><span class="sxs-lookup"><span data-stu-id="d8243-115">TableColumn</span></span>](tablecolumn.md) |<span data-ttu-id="d8243-116">Dient zum Aktualisieren des TableColumn-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d8243-116">Update TableColumn object.</span></span> |
|[<span data-ttu-id="d8243-117">Databodyrange</span><span class="sxs-lookup"><span data-stu-id="d8243-117">Databodyrange</span></span>](../api/tablecolumn-databodyrange.md)|[<span data-ttu-id="d8243-118">Range</span><span class="sxs-lookup"><span data-stu-id="d8243-118">Range</span></span>](range.md)|<span data-ttu-id="d8243-119">Ruft das Bereichsobjekt ab, das mit dem Datenteil der Spalte verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="d8243-119">Gets the range object associated with the data body of the column.</span></span>|
|[<span data-ttu-id="d8243-120">Headerrowrange</span><span class="sxs-lookup"><span data-stu-id="d8243-120">Headerrowrange</span></span>](../api/tablecolumn-headerrowrange.md)|[<span data-ttu-id="d8243-121">Range</span><span class="sxs-lookup"><span data-stu-id="d8243-121">Range</span></span>](range.md)|<span data-ttu-id="d8243-122">Ruft das Bereichsobjekt ab, das mit der Überschriftenzeile der Spalte verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="d8243-122">Gets the range object associated with the header row of the column.</span></span>|
|[<span data-ttu-id="d8243-123">Range</span><span class="sxs-lookup"><span data-stu-id="d8243-123">Range</span></span>](../api/tablecolumn-range.md)|[<span data-ttu-id="d8243-124">Range</span><span class="sxs-lookup"><span data-stu-id="d8243-124">Range</span></span>](range.md)|<span data-ttu-id="d8243-125">Ruft das Bereichsobjekt ab, das mit der gesamten Spalte verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="d8243-125">Gets the range object associated with the entire column.</span></span>|
|[<span data-ttu-id="d8243-126">Totalrowrange</span><span class="sxs-lookup"><span data-stu-id="d8243-126">Totalrowrange</span></span>](../api/tablecolumn-totalrowrange.md)|[<span data-ttu-id="d8243-127">Range</span><span class="sxs-lookup"><span data-stu-id="d8243-127">Range</span></span>](range.md)|<span data-ttu-id="d8243-128">Ruft das Bereichsobjekt ab, das mit der Ergebniszeile der Spalte verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="d8243-128">Gets the range object associated with the totals row of the column.</span></span>|
|[<span data-ttu-id="d8243-129">Delete</span><span class="sxs-lookup"><span data-stu-id="d8243-129">Delete</span></span>](../api/tablecolumn-delete.md)|<span data-ttu-id="d8243-130">Keine</span><span class="sxs-lookup"><span data-stu-id="d8243-130">None</span></span>|<span data-ttu-id="d8243-131">Löscht die Spalte aus der Tabelle.</span><span class="sxs-lookup"><span data-stu-id="d8243-131">Deletes the column from the table.</span></span>|
|[<span data-ttu-id="d8243-132">List</span><span class="sxs-lookup"><span data-stu-id="d8243-132">List</span></span>](../api/tablecolumn-list.md) | <span data-ttu-id="d8243-133">[TableColumn](tablecolumn.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d8243-133">[TableColumn](tablecolumn.md) collection</span></span> |<span data-ttu-id="d8243-134">Dient zum Abrufen der tableColumn-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="d8243-134">Get tableColumn object collection.</span></span> |
|[<span data-ttu-id="d8243-135">Itemat</span><span class="sxs-lookup"><span data-stu-id="d8243-135">Itemat</span></span>](../api/tablecolumncollection-itemat.md)|[<span data-ttu-id="d8243-136">TableColumn</span><span class="sxs-lookup"><span data-stu-id="d8243-136">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="d8243-137">Ruft eine Spalte anhand ihrer Position in der Auflistung ab.</span><span class="sxs-lookup"><span data-stu-id="d8243-137">Gets a column based on its position in the collection.</span></span>|
|[<span data-ttu-id="d8243-138">Add</span><span class="sxs-lookup"><span data-stu-id="d8243-138">Add</span></span>](../api/tablecolumncollection-add.md)|[<span data-ttu-id="d8243-139">TableColumn</span><span class="sxs-lookup"><span data-stu-id="d8243-139">TableColumn</span></span>](tablecolumn.md)|<span data-ttu-id="d8243-140">Fügt der Tabelle eine neue Spalte hinzu.</span><span class="sxs-lookup"><span data-stu-id="d8243-140">Adds a new column to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8243-141">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d8243-141">Properties</span></span>
| <span data-ttu-id="d8243-142">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d8243-142">Property</span></span>     | <span data-ttu-id="d8243-143">Typ</span><span class="sxs-lookup"><span data-stu-id="d8243-143">Type</span></span>   |<span data-ttu-id="d8243-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d8243-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8243-145">id</span><span class="sxs-lookup"><span data-stu-id="d8243-145">id</span></span>|<span data-ttu-id="d8243-146">int</span><span class="sxs-lookup"><span data-stu-id="d8243-146">int</span></span>|<span data-ttu-id="d8243-p102">Gibt einen eindeutigen Schlüssel an, der die Spalte in der Tabelle angibt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d8243-p102">Returns a unique key that identifies the column within the table. Read-only.</span></span>|
|<span data-ttu-id="d8243-149">Index</span><span class="sxs-lookup"><span data-stu-id="d8243-149">index</span></span>|<span data-ttu-id="d8243-150">int</span><span class="sxs-lookup"><span data-stu-id="d8243-150">int</span></span>|<span data-ttu-id="d8243-p103">Gibt die Indexnummer der Spalte in der Spaltenauflistung der Tabelle zurück. Nullindiziert. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d8243-p103">Returns the index number of the column within the columns collection of the table. Zero-indexed. Read-only.</span></span>|
|<span data-ttu-id="d8243-154">name</span><span class="sxs-lookup"><span data-stu-id="d8243-154">name</span></span>|<span data-ttu-id="d8243-155">string</span><span class="sxs-lookup"><span data-stu-id="d8243-155">string</span></span>|<span data-ttu-id="d8243-p104">Gibt den Namen der Tabellenspalte zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d8243-p104">Returns the name of the table column. Read-only.</span></span>|
|<span data-ttu-id="d8243-158">values</span><span class="sxs-lookup"><span data-stu-id="d8243-158">values</span></span>|<span data-ttu-id="d8243-159">json</span><span class="sxs-lookup"><span data-stu-id="d8243-159">json</span></span>|<span data-ttu-id="d8243-p105">Stellt die Rohwerte des angegebenen Bereichs dar. Die zurückgegebenen Daten können den Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zelle, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.</span><span class="sxs-lookup"><span data-stu-id="d8243-p105">Represents the raw values of the specified range. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8243-163">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d8243-163">Relationships</span></span>
| <span data-ttu-id="d8243-164">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d8243-164">Relationship</span></span> | <span data-ttu-id="d8243-165">Typ</span><span class="sxs-lookup"><span data-stu-id="d8243-165">Type</span></span>   |<span data-ttu-id="d8243-166">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d8243-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8243-167">Filter</span><span class="sxs-lookup"><span data-stu-id="d8243-167">filter</span></span>|[<span data-ttu-id="d8243-168">Filter</span><span class="sxs-lookup"><span data-stu-id="d8243-168">Filter</span></span>](filter.md)|<span data-ttu-id="d8243-p106">Ruft den auf die Salte angewendeten Filter ab. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d8243-p106">Retrieve the filter applied to the column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8243-171">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d8243-171">JSON representation</span></span>

<span data-ttu-id="d8243-172">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d8243-172">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableColumn"
}-->

```json
{
  "id": 1024,
  "index": 1024,
  "name": "string",
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableColumn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->