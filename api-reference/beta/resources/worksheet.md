---
title: Worksheet-Ressourcentyp
description: Ein Excel-Arbeitsblatt ist ein Raster von Zellen. Es kann Daten, Tabellen, Diagramme usw. enthalten.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 6a3a5fbb222c9228b55b2dac2a38b699ed15f213
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574376"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="d4fd8-104">Worksheet-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d4fd8-104">Worksheet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4fd8-p102">Ein Excel-Arbeitsblatt ist ein Raster von Zellen. Es kann Daten, Tabellen, Diagramme usw. enthalten.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-p102">An Excel worksheet is a grid of cells. It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="d4fd8-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="d4fd8-107">Methods</span></span>

| <span data-ttu-id="d4fd8-108">Methode</span><span class="sxs-lookup"><span data-stu-id="d4fd8-108">Method</span></span>           | <span data-ttu-id="d4fd8-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d4fd8-109">Return Type</span></span>    |<span data-ttu-id="d4fd8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4fd8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4fd8-111">Arbeitsblatt abrufen</span><span class="sxs-lookup"><span data-stu-id="d4fd8-111">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="d4fd8-112">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="d4fd8-112">WorkbookWorksheet</span></span>](worksheet.md) |<span data-ttu-id="d4fd8-113">Dient zum Lesen der Eigenschaften und der Beziehungen des worksheet-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-113">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="d4fd8-114">Diagramm erstellen</span><span class="sxs-lookup"><span data-stu-id="d4fd8-114">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="d4fd8-115">WorkbookChart</span><span class="sxs-lookup"><span data-stu-id="d4fd8-115">WorkbookChart</span></span>](chart.md)| <span data-ttu-id="d4fd8-116">Dient zum Erstellen eines neuen Diagramms durch Veröffentlichen in der Diagrammsammlung.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-116">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="d4fd8-117">Namen auflisten</span><span class="sxs-lookup"><span data-stu-id="d4fd8-117">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="d4fd8-118">[WorkbookNamedItem](workbooknameditem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d4fd8-118">[WorkbookNamedItem](workbooknameditem.md) collection</span></span>| <span data-ttu-id="d4fd8-119">Dient zum Abrufen der benannten Elementsammlung, die mit dem Arbeitsblatt verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-119">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="d4fd8-120">Diagramme auflisten</span><span class="sxs-lookup"><span data-stu-id="d4fd8-120">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="d4fd8-121">[WorkbookChart](chart.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d4fd8-121">[WorkbookChart](chart.md) collection</span></span>| <span data-ttu-id="d4fd8-122">Dient zum Abrufen einer Diagrammobjeksammlung.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-122">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="d4fd8-123">Tabelle erstellen</span><span class="sxs-lookup"><span data-stu-id="d4fd8-123">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="d4fd8-124">WorkbookTable</span><span class="sxs-lookup"><span data-stu-id="d4fd8-124">WorkbookTable</span></span>](table.md)| <span data-ttu-id="d4fd8-125">Dient zum Erstellen einer neuen Tabelle durch Veröffentlichen in der Diagrammsammlung.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-125">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="d4fd8-126">Tabellen auflisten</span><span class="sxs-lookup"><span data-stu-id="d4fd8-126">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="d4fd8-127">[WorkbookTable](table.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d4fd8-127">[WorkbookTable](table.md) collection</span></span>| <span data-ttu-id="d4fd8-128">Dient zum Abrufen einer Tabellenobjeksammlung.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-128">Get a Table object collection.</span></span>|
|[<span data-ttu-id="d4fd8-129">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="d4fd8-129">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="d4fd8-130">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="d4fd8-130">WorkbookWorksheet</span></span>](worksheet.md)   |<span data-ttu-id="d4fd8-131">Dient zum Aktualisieren des Worksheet-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-131">Update Worksheet object.</span></span> |
|[<span data-ttu-id="d4fd8-132">Cell</span><span class="sxs-lookup"><span data-stu-id="d4fd8-132">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="d4fd8-133">Range</span><span class="sxs-lookup"><span data-stu-id="d4fd8-133">Range</span></span>](range.md)|<span data-ttu-id="d4fd8-p103">Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb ihres übergeordneten Bereichs befinden, solange sie im Arbeitsblattraster bleibt.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-p103">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="d4fd8-136">Range</span><span class="sxs-lookup"><span data-stu-id="d4fd8-136">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="d4fd8-137">Range</span><span class="sxs-lookup"><span data-stu-id="d4fd8-137">Range</span></span>](range.md)|<span data-ttu-id="d4fd8-138">Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-138">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="d4fd8-139">Usedrange</span><span class="sxs-lookup"><span data-stu-id="d4fd8-139">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="d4fd8-140">Range</span><span class="sxs-lookup"><span data-stu-id="d4fd8-140">Range</span></span>](range.md)|<span data-ttu-id="d4fd8-p104">Der verwendete Bereich ist der kleinste Bereich, der mindestens eine der Zellen umfasst, die einen Wert enthalten oder denen eine Formatierung zugewiesen wurde. Wenn das Arbeitsblatt leer ist, gibt diese Funktion die oberste linke Zelle zurück.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-p104">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="d4fd8-143">Löschen</span><span class="sxs-lookup"><span data-stu-id="d4fd8-143">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="d4fd8-144">Keine</span><span class="sxs-lookup"><span data-stu-id="d4fd8-144">None</span></span>|<span data-ttu-id="d4fd8-145">Löscht das Arbeitsblatt aus der Arbeitsmappe.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-145">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="d4fd8-146">List</span><span class="sxs-lookup"><span data-stu-id="d4fd8-146">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="d4fd8-147">[WorkbookWorksheet](worksheet.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d4fd8-147">[WorkbookWorksheet](worksheet.md) collection</span></span> |<span data-ttu-id="d4fd8-148">Dient zum Abrufen der Arbeitsblatt-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-148">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="d4fd8-149">Add</span><span class="sxs-lookup"><span data-stu-id="d4fd8-149">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="d4fd8-150">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="d4fd8-150">WorkbookWorksheet</span></span>](worksheet.md)|<span data-ttu-id="d4fd8-p105">Fügt der Arbeitsmappe ein neues Arbeitsblatt hinzu. Das Arbeitsblatt wird automatisch am Ende der vorhandenen Arbeitsblätter hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-p105">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="d4fd8-153">pivotTables auflisten</span><span class="sxs-lookup"><span data-stu-id="d4fd8-153">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="d4fd8-154">[workbookPivotTable](workbookpivottable.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d4fd8-154">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="d4fd8-155">Rufen Sie eine workbookPivotTable-Objektsammlung ab.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-155">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="d4fd8-156">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d4fd8-156">Properties</span></span>
| <span data-ttu-id="d4fd8-157">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4fd8-157">Property</span></span>     | <span data-ttu-id="d4fd8-158">Typ</span><span class="sxs-lookup"><span data-stu-id="d4fd8-158">Type</span></span>   |<span data-ttu-id="d4fd8-159">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4fd8-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4fd8-160">id</span><span class="sxs-lookup"><span data-stu-id="d4fd8-160">id</span></span>|<span data-ttu-id="d4fd8-161">string</span><span class="sxs-lookup"><span data-stu-id="d4fd8-161">string</span></span>|<span data-ttu-id="d4fd8-p106">Gibt einen Wert zurück, der das Arbeitsblatt in einer bestimmten Arbeitsmappe eindeutig identifiziert. Der Wert des Bezeichners bleibt unverändert, auch wenn das Arbeitsblatt umbenannt oder verschoben wird. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-p106">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="d4fd8-165">name</span><span class="sxs-lookup"><span data-stu-id="d4fd8-165">name</span></span>|<span data-ttu-id="d4fd8-166">string</span><span class="sxs-lookup"><span data-stu-id="d4fd8-166">string</span></span>|<span data-ttu-id="d4fd8-167">Der Anzeigename des Arbeitsblatts.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-167">The display name of the worksheet.</span></span>|
|<span data-ttu-id="d4fd8-168">position</span><span class="sxs-lookup"><span data-stu-id="d4fd8-168">position</span></span>|<span data-ttu-id="d4fd8-169">int</span><span class="sxs-lookup"><span data-stu-id="d4fd8-169">int</span></span>|<span data-ttu-id="d4fd8-170">Die nullbasiert Position des Arbeitsblatts in der Arbeitsmappe.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-170">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="d4fd8-171">visibility</span><span class="sxs-lookup"><span data-stu-id="d4fd8-171">visibility</span></span>|<span data-ttu-id="d4fd8-172">string</span><span class="sxs-lookup"><span data-stu-id="d4fd8-172">string</span></span>|<span data-ttu-id="d4fd8-173">Die Sichtbarkeit des Arbeitsblatts ein.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-173">The Visibility of the worksheet.</span></span> <span data-ttu-id="d4fd8-174">Die möglichen Werte sind: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-174">The possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4fd8-175">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d4fd8-175">Relationships</span></span>
| <span data-ttu-id="d4fd8-176">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d4fd8-176">Relationship</span></span> | <span data-ttu-id="d4fd8-177">Typ</span><span class="sxs-lookup"><span data-stu-id="d4fd8-177">Type</span></span>   |<span data-ttu-id="d4fd8-178">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4fd8-178">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4fd8-179">charts</span><span class="sxs-lookup"><span data-stu-id="d4fd8-179">charts</span></span>|<span data-ttu-id="d4fd8-180">[WorkbookChart](chart.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d4fd8-180">[WorkbookChart](chart.md) collection</span></span>|<span data-ttu-id="d4fd8-p108">Gibt die Sammlung von Diagrammen zurück, die Teil des Arbeitsblatts sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-p108">Returns collection of charts that are part of the worksheet. Read-only.</span></span>|
|<span data-ttu-id="d4fd8-183">names</span><span class="sxs-lookup"><span data-stu-id="d4fd8-183">names</span></span>|<span data-ttu-id="d4fd8-184">[WorkbookNamedItem](workbooknameditem.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d4fd8-184">[workbookNamedItem](workbooknameditem.md) collection</span></span>|<span data-ttu-id="d4fd8-p109">Gibt die Sammlung von Namen zurück, die mit dem Arbeitsblatt verknüpft sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-p109">Returns collection of names that are associated with the worksheet. Read-only.</span></span>|
|<span data-ttu-id="d4fd8-187">pivotTables</span><span class="sxs-lookup"><span data-stu-id="d4fd8-187">pivotTables</span></span>|<span data-ttu-id="d4fd8-188">[workbookPivotTable](workbookpivottable.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d4fd8-188">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="d4fd8-189">Die Sammlung von PivotTables, die Teil des Arbeitsblatts sind.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-189">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="d4fd8-190">Schutz</span><span class="sxs-lookup"><span data-stu-id="d4fd8-190">protection</span></span>|[<span data-ttu-id="d4fd8-191">WorkbookWorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="d4fd8-191">WorkbookWorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="d4fd8-p110">Gibt das Arbeitsblattschutz-Objekt für ein Arbeitsblatt zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-p110">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="d4fd8-194">Tabellen</span><span class="sxs-lookup"><span data-stu-id="d4fd8-194">tables</span></span>|<span data-ttu-id="d4fd8-195">[WorkbookTable](table.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d4fd8-195">[WorkbookTable](table.md) collection</span></span>|<span data-ttu-id="d4fd8-p111">Gibt die Sammlung von Tabellen zurück, die Teil des Arbeitsblatts sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-p111">Collection of tables that are part of the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4fd8-198">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d4fd8-198">JSON representation</span></span>

<span data-ttu-id="d4fd8-199">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d4fd8-199">Here is a JSON representation of the resource.</span></span>

<!-- {
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
<!--
{
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/worksheet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
