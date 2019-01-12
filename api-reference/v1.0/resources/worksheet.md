---
title: Worksheet-Ressourcentyp
description: Ein Excel-Arbeitsblatt ist ein Raster von Zellen. Es kann Daten, Tabellen, Diagramme usw. enthalten.
localization_priority: Priority
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 60e31738329943d96e1a4f3ea8293851e759eaff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983870"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="73a21-104">Worksheet-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="73a21-104">Worksheet resource type</span></span>

<span data-ttu-id="73a21-p102">Ein Excel-Arbeitsblatt ist ein Raster von Zellen. Es kann Daten, Tabellen, Diagramme usw. enthalten.</span><span class="sxs-lookup"><span data-stu-id="73a21-p102">An Excel worksheet is a grid of cells. It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="73a21-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="73a21-107">Methods</span></span>

| <span data-ttu-id="73a21-108">Methode</span><span class="sxs-lookup"><span data-stu-id="73a21-108">Method</span></span>           | <span data-ttu-id="73a21-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="73a21-109">Return Type</span></span>    |<span data-ttu-id="73a21-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73a21-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="73a21-111">Arbeitsblatt abrufen</span><span class="sxs-lookup"><span data-stu-id="73a21-111">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="73a21-112">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="73a21-112">WorkbookWorksheet</span></span>](worksheet.md) |<span data-ttu-id="73a21-113">Dient zum Lesen der Eigenschaften und der Beziehungen des worksheet-Objekts.</span><span class="sxs-lookup"><span data-stu-id="73a21-113">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="73a21-114">Diagramm erstellen</span><span class="sxs-lookup"><span data-stu-id="73a21-114">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="73a21-115">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="73a21-115">WorkbookChart</span></span>](chart.md)| <span data-ttu-id="73a21-116">Dient zum Erstellen eines neuen Diagramms durch Veröffentlichen in der Diagrammsammlung.</span><span class="sxs-lookup"><span data-stu-id="73a21-116">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="73a21-117">Namen auflisten</span><span class="sxs-lookup"><span data-stu-id="73a21-117">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="73a21-118">[WorkbookNamedItem](nameditem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="73a21-118">[WorkbookNamedItem](nameditem.md) collection</span></span>| <span data-ttu-id="73a21-119">Dient zum Abrufen der benannten Elementsammlung, die mit dem Arbeitsblatt verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="73a21-119">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="73a21-120">Diagramme auflisten</span><span class="sxs-lookup"><span data-stu-id="73a21-120">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="73a21-121">[WorkbookChart](chart.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="73a21-121">[WorkbookChart](chart.md) collection</span></span>| <span data-ttu-id="73a21-122">Dient zum Abrufen einer Diagrammobjeksammlung.</span><span class="sxs-lookup"><span data-stu-id="73a21-122">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="73a21-123">Tabelle erstellen</span><span class="sxs-lookup"><span data-stu-id="73a21-123">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="73a21-124">WorkbookTable</span><span class="sxs-lookup"><span data-stu-id="73a21-124">WorkbookTable</span></span>](table.md)| <span data-ttu-id="73a21-125">Dient zum Erstellen einer neuen Tabelle durch Veröffentlichen in der Diagrammsammlung.</span><span class="sxs-lookup"><span data-stu-id="73a21-125">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="73a21-126">Tabellen auflisten</span><span class="sxs-lookup"><span data-stu-id="73a21-126">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="73a21-127">[WorkbookTable](table.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="73a21-127">[WorkbookTable](table.md) collection</span></span>| <span data-ttu-id="73a21-128">Dient zum Abrufen einer Tabellenobjeksammlung.</span><span class="sxs-lookup"><span data-stu-id="73a21-128">Get a Table object collection.</span></span>|
|[<span data-ttu-id="73a21-129">Update</span><span class="sxs-lookup"><span data-stu-id="73a21-129">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="73a21-130">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="73a21-130">WorkbookWorksheet</span></span>](worksheet.md)   |<span data-ttu-id="73a21-131">Dient zum Aktualisieren des Worksheet-Objekts.</span><span class="sxs-lookup"><span data-stu-id="73a21-131">Update Worksheet object.</span></span> |
|[<span data-ttu-id="73a21-132">Cell</span><span class="sxs-lookup"><span data-stu-id="73a21-132">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="73a21-133">Range</span><span class="sxs-lookup"><span data-stu-id="73a21-133">Range</span></span>](range.md)|<span data-ttu-id="73a21-p103">Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb ihres übergeordneten Bereichs befinden, solange sie im Arbeitsblattraster bleibt.</span><span class="sxs-lookup"><span data-stu-id="73a21-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="73a21-136">Range</span><span class="sxs-lookup"><span data-stu-id="73a21-136">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="73a21-137">Range</span><span class="sxs-lookup"><span data-stu-id="73a21-137">Range</span></span>](range.md)|<span data-ttu-id="73a21-138">Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.</span><span class="sxs-lookup"><span data-stu-id="73a21-138">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="73a21-139">Usedrange</span><span class="sxs-lookup"><span data-stu-id="73a21-139">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="73a21-140">Range</span><span class="sxs-lookup"><span data-stu-id="73a21-140">Range</span></span>](range.md)|<span data-ttu-id="73a21-p104">Der verwendete Bereich ist der kleinste Bereich, der mindestens eine der Zellen umfasst, die einen Wert enthalten oder denen eine Formatierung zugewiesen wurde. Wenn das Arbeitsblatt leer ist, gibt diese Funktion die oberste linke Zelle zurück.</span><span class="sxs-lookup"><span data-stu-id="73a21-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="73a21-143">Delete</span><span class="sxs-lookup"><span data-stu-id="73a21-143">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="73a21-144">Keine</span><span class="sxs-lookup"><span data-stu-id="73a21-144">None</span></span>|<span data-ttu-id="73a21-145">Löscht das Arbeitsblatt aus der Arbeitsmappe.</span><span class="sxs-lookup"><span data-stu-id="73a21-145">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="73a21-146">List</span><span class="sxs-lookup"><span data-stu-id="73a21-146">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="73a21-147">[WorkbookWorksheet](worksheet.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="73a21-147">[WorkbookWorksheet](worksheet.md) collection</span></span> |<span data-ttu-id="73a21-148">Dient zum Abrufen der Arbeitsblatt-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="73a21-148">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="73a21-149">Add</span><span class="sxs-lookup"><span data-stu-id="73a21-149">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="73a21-150">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="73a21-150">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="73a21-p105">Fügt der Arbeitsmappe ein neues Arbeitsblatt hinzu. Das Arbeitsblatt wird automatisch am Ende der vorhandenen Arbeitsblätter hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="73a21-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="73a21-153">pivotTables auflisten</span><span class="sxs-lookup"><span data-stu-id="73a21-153">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="73a21-154">[workbookPivotTable](workbookpivottable.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="73a21-154">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="73a21-155">Rufen Sie eine workbookPivotTable-Objektsammlung ab.</span><span class="sxs-lookup"><span data-stu-id="73a21-155">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="73a21-156">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="73a21-156">Properties</span></span>
| <span data-ttu-id="73a21-157">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="73a21-157">Property</span></span>     | <span data-ttu-id="73a21-158">Typ</span><span class="sxs-lookup"><span data-stu-id="73a21-158">Type</span></span>   |<span data-ttu-id="73a21-159">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73a21-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73a21-160">id</span><span class="sxs-lookup"><span data-stu-id="73a21-160">id</span></span>|<span data-ttu-id="73a21-161">string</span><span class="sxs-lookup"><span data-stu-id="73a21-161">string</span></span>|<span data-ttu-id="73a21-p106">Gibt einen Wert zurück, der das Arbeitsblatt in einer bestimmten Arbeitsmappe eindeutig identifiziert. Der Wert des Bezeichners bleibt unverändert, auch wenn das Arbeitsblatt umbenannt oder verschoben wird. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="73a21-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="73a21-165">name</span><span class="sxs-lookup"><span data-stu-id="73a21-165">name</span></span>|<span data-ttu-id="73a21-166">string</span><span class="sxs-lookup"><span data-stu-id="73a21-166">string</span></span>|<span data-ttu-id="73a21-167">Der Anzeigename des Arbeitsblatts.</span><span class="sxs-lookup"><span data-stu-id="73a21-167">The display name of the worksheet.</span></span>|
|<span data-ttu-id="73a21-168">position</span><span class="sxs-lookup"><span data-stu-id="73a21-168">position</span></span>|<span data-ttu-id="73a21-169">int</span><span class="sxs-lookup"><span data-stu-id="73a21-169">int</span></span>|<span data-ttu-id="73a21-170">Die nullbasiert Position des Arbeitsblatts in der Arbeitsmappe.</span><span class="sxs-lookup"><span data-stu-id="73a21-170">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="73a21-171">visibility</span><span class="sxs-lookup"><span data-stu-id="73a21-171">visibility</span></span>|<span data-ttu-id="73a21-172">string</span><span class="sxs-lookup"><span data-stu-id="73a21-172">string</span></span>|<span data-ttu-id="73a21-173">Die Sichtbarkeit des Arbeitsblatts ein.</span><span class="sxs-lookup"><span data-stu-id="73a21-173">The Visibility of the worksheet.</span></span> <span data-ttu-id="73a21-174">Die möglichen Werte sind: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="73a21-174">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73a21-175">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="73a21-175">Relationships</span></span>
| <span data-ttu-id="73a21-176">Beziehung</span><span class="sxs-lookup"><span data-stu-id="73a21-176">Relationship</span></span> | <span data-ttu-id="73a21-177">Typ</span><span class="sxs-lookup"><span data-stu-id="73a21-177">Type</span></span>   |<span data-ttu-id="73a21-178">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73a21-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73a21-179">charts</span><span class="sxs-lookup"><span data-stu-id="73a21-179">charts</span></span>|<span data-ttu-id="73a21-180">[WorkbookChart](chart.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="73a21-180">[WorkbookChart](chart.md) collection</span></span>|<span data-ttu-id="73a21-p108">Gibt die Sammlung von Diagrammen zurück, die Teil des Arbeitsblatts sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="73a21-p108">Returns collection of charts that are part of the worksheet. Read-only.</span></span>|
|<span data-ttu-id="73a21-183">names</span><span class="sxs-lookup"><span data-stu-id="73a21-183">names</span></span>|<span data-ttu-id="73a21-184">[WorkbookNamedItem](nameditem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="73a21-184">[WorkbookNamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="73a21-p109">Gibt die Sammlung von Namen zurück, die mit dem Arbeitsblatt verknüpft sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="73a21-p109">Returns collection of names that are associated with the worksheet. Read-only.</span></span>|
|<span data-ttu-id="73a21-187">pivotTables</span><span class="sxs-lookup"><span data-stu-id="73a21-187">pivotTables</span></span>|<span data-ttu-id="73a21-188">[workbookPivotTable](workbookpivottable.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="73a21-188">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="73a21-189">Die Sammlung von PivotTables, die Teil des Arbeitsblatts sind.</span><span class="sxs-lookup"><span data-stu-id="73a21-189">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="73a21-190">Schutz</span><span class="sxs-lookup"><span data-stu-id="73a21-190">protection</span></span>|[<span data-ttu-id="73a21-191">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="73a21-191">WorkbookWorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="73a21-p110">Gibt das Arbeitsblattschutz-Objekt für ein Arbeitsblatt zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="73a21-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="73a21-194">Tabellen</span><span class="sxs-lookup"><span data-stu-id="73a21-194">tables</span></span>|<span data-ttu-id="73a21-195">[WorkbookTable](table.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="73a21-195">[WorkbookTable](table.md) collection</span></span>|<span data-ttu-id="73a21-p111">Gibt die Sammlung von Tabellen zurück, die Teil des Arbeitsblatts sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="73a21-p111">Collection of tables that are part of the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73a21-198">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="73a21-198">JSON representation</span></span>

<span data-ttu-id="73a21-199">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="73a21-199">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheet"
}-->

```json
{
  "id": "string",
  "name": "string",
  "position": 1024,
  "visibility": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
