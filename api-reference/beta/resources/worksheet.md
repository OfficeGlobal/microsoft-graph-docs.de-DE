---
title: Worksheet-Ressourcentyp
description: Ein Excel-Arbeitsblatt ist ein Raster von Zellen. Es kann Daten, Tabellen, Diagramme usw. enthalten.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: d04ebafda64f9a081096fbf0fd94461b9765a6db
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926526"
---
# <a name="worksheet-resource-type"></a><span data-ttu-id="82504-104">Worksheet-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="82504-104">Worksheet resource type</span></span>

> <span data-ttu-id="82504-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="82504-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82504-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="82504-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="82504-p103">Ein Excel-Arbeitsblatt ist ein Raster von Zellen. Es kann Daten, Tabellen, Diagramme usw. enthalten.</span><span class="sxs-lookup"><span data-stu-id="82504-p103">An Excel worksheet is a grid of cells. It can contain data, tables, charts, etc.</span></span>


## <a name="methods"></a><span data-ttu-id="82504-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="82504-109">Methods</span></span>

| <span data-ttu-id="82504-110">Methode</span><span class="sxs-lookup"><span data-stu-id="82504-110">Method</span></span>           | <span data-ttu-id="82504-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="82504-111">Return Type</span></span>    |<span data-ttu-id="82504-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82504-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="82504-113">Arbeitsblatt abrufen</span><span class="sxs-lookup"><span data-stu-id="82504-113">Get Worksheet</span></span>](../api/worksheet-get.md) | [<span data-ttu-id="82504-114">Worksheet</span><span class="sxs-lookup"><span data-stu-id="82504-114">Worksheet</span></span>](worksheet.md) |<span data-ttu-id="82504-115">Dient zum Lesen der Eigenschaften und der Beziehungen des worksheet-Objekts.</span><span class="sxs-lookup"><span data-stu-id="82504-115">Read properties and relationships of worksheet object.</span></span>|
|[<span data-ttu-id="82504-116">Diagramm erstellen</span><span class="sxs-lookup"><span data-stu-id="82504-116">Create Chart</span></span>](../api/worksheet-post-charts.md) |[<span data-ttu-id="82504-117">Chart</span><span class="sxs-lookup"><span data-stu-id="82504-117">Chart</span></span>](chart.md)| <span data-ttu-id="82504-118">Dient zum Erstellen eines neuen Diagramms durch Veröffentlichen in der Diagrammsammlung.</span><span class="sxs-lookup"><span data-stu-id="82504-118">Create a new Chart by posting to the charts collection.</span></span>|
|[<span data-ttu-id="82504-119">Namen auflisten</span><span class="sxs-lookup"><span data-stu-id="82504-119">List names</span></span>](../api/worksheet-list-names.md) |<span data-ttu-id="82504-120">[NamedItem](nameditem.md) collection</span><span class="sxs-lookup"><span data-stu-id="82504-120">[NamedItem](nameditem.md) collection</span></span>| <span data-ttu-id="82504-121">Dient zum Abrufen der benannten Elementsammlung, die mit dem Arbeitsblatt verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="82504-121">Get named item collection associated with the worksheet.</span></span>|
|[<span data-ttu-id="82504-122">Diagramme auflisten</span><span class="sxs-lookup"><span data-stu-id="82504-122">List charts</span></span>](../api/worksheet-list-charts.md) |<span data-ttu-id="82504-123">[Diagrammsammlung](chart.md)</span><span class="sxs-lookup"><span data-stu-id="82504-123">[Chart](chart.md) collection</span></span>| <span data-ttu-id="82504-124">Dient zum Abrufen einer Diagrammobjeksammlung.</span><span class="sxs-lookup"><span data-stu-id="82504-124">Get a Chart object collection.</span></span>|
|[<span data-ttu-id="82504-125">Tabelle erstellen</span><span class="sxs-lookup"><span data-stu-id="82504-125">Create Table</span></span>](../api/worksheet-post-tables.md) |[<span data-ttu-id="82504-126">Table</span><span class="sxs-lookup"><span data-stu-id="82504-126">Table</span></span>](table.md)| <span data-ttu-id="82504-127">Dient zum Erstellen einer neuen Tabelle durch Veröffentlichen in der Diagrammsammlung.</span><span class="sxs-lookup"><span data-stu-id="82504-127">Create a new Table by posting to the tables collection.</span></span>|
|[<span data-ttu-id="82504-128">Tabellen auflisten</span><span class="sxs-lookup"><span data-stu-id="82504-128">List tables</span></span>](../api/worksheet-list-tables.md) |<span data-ttu-id="82504-129">[Tabellensammlung](table.md)</span><span class="sxs-lookup"><span data-stu-id="82504-129">[Table](table.md) collection</span></span>| <span data-ttu-id="82504-130">Dient zum Abrufen einer Tabellenobjeksammlung.</span><span class="sxs-lookup"><span data-stu-id="82504-130">Get a Table object collection.</span></span>|
|[<span data-ttu-id="82504-131">Update</span><span class="sxs-lookup"><span data-stu-id="82504-131">Update</span></span>](../api/worksheet-update.md) | [<span data-ttu-id="82504-132">Worksheet</span><span class="sxs-lookup"><span data-stu-id="82504-132">Worksheet</span></span>](worksheet.md)   |<span data-ttu-id="82504-133">Dient zum Aktualisieren des Worksheet-Objekts.</span><span class="sxs-lookup"><span data-stu-id="82504-133">Update Worksheet object.</span></span> |
|[<span data-ttu-id="82504-134">Cell</span><span class="sxs-lookup"><span data-stu-id="82504-134">Cell</span></span>](../api/worksheet-cell.md)|[<span data-ttu-id="82504-135">Range</span><span class="sxs-lookup"><span data-stu-id="82504-135">Range</span></span>](range.md)|<span data-ttu-id="82504-p104">Ruft das Bereichsobjekt ab, das die einzelne Zelle basierend auf Zeilen- und Spaltenanzahl enthält. Die Zelle kann sich außerhalb ihres übergeordneten Bereichs befinden, solange sie im Arbeitsblattraster bleibt.</span><span class="sxs-lookup"><span data-stu-id="82504-p104">Gets the range object containing the single cell based on row and column numbers. The cell can be outside the bounds of its parent range, so long as it's stays within the worksheet grid.</span></span>|
|[<span data-ttu-id="82504-138">Range</span><span class="sxs-lookup"><span data-stu-id="82504-138">Range</span></span>](../api/worksheet-range.md)|[<span data-ttu-id="82504-139">Range</span><span class="sxs-lookup"><span data-stu-id="82504-139">Range</span></span>](range.md)|<span data-ttu-id="82504-140">Ruft das durch die Adresse oder den Namen angegebene Bereichsobjekt ab.</span><span class="sxs-lookup"><span data-stu-id="82504-140">Gets the range object specified by the address or name.</span></span>|
|[<span data-ttu-id="82504-141">Usedrange</span><span class="sxs-lookup"><span data-stu-id="82504-141">Usedrange</span></span>](../api/worksheet-usedrange.md)|[<span data-ttu-id="82504-142">Range</span><span class="sxs-lookup"><span data-stu-id="82504-142">Range</span></span>](range.md)|<span data-ttu-id="82504-p105">Der verwendete Bereich ist der kleinste Bereich, der mindestens eine der Zellen umfasst, die einen Wert enthalten oder denen eine Formatierung zugewiesen wurde. Wenn das Arbeitsblatt leer ist, gibt diese Funktion die oberste linke Zelle zurück.</span><span class="sxs-lookup"><span data-stu-id="82504-p105">The used range is the smallest range that encompasses any cells that have a value or formatting assigned to them. If the worksheet is blank, this function will return the top left cell.</span></span>|
|[<span data-ttu-id="82504-145">Delete</span><span class="sxs-lookup"><span data-stu-id="82504-145">Delete</span></span>](../api/worksheet-delete.md)|<span data-ttu-id="82504-146">Keine</span><span class="sxs-lookup"><span data-stu-id="82504-146">None</span></span>|<span data-ttu-id="82504-147">Löscht das Arbeitsblatt aus der Arbeitsmappe.</span><span class="sxs-lookup"><span data-stu-id="82504-147">Deletes the worksheet from the workbook.</span></span>|
|[<span data-ttu-id="82504-148">List</span><span class="sxs-lookup"><span data-stu-id="82504-148">List</span></span>](../api/worksheet-list.md) | <span data-ttu-id="82504-149">[Worksheet](worksheet.md) collection</span><span class="sxs-lookup"><span data-stu-id="82504-149">[Worksheet](worksheet.md) collection</span></span> |<span data-ttu-id="82504-150">Dient zum Abrufen der Arbeitsblatt-Objektsammlung.</span><span class="sxs-lookup"><span data-stu-id="82504-150">Get worksheet object collection.</span></span> |
|[<span data-ttu-id="82504-151">Add</span><span class="sxs-lookup"><span data-stu-id="82504-151">Add</span></span>](../api/worksheetcollection-add.md)|[<span data-ttu-id="82504-152">Worksheet</span><span class="sxs-lookup"><span data-stu-id="82504-152">Worksheet</span></span>](worksheet.md)|<span data-ttu-id="82504-p106">Fügt der Arbeitsmappe ein neues Arbeitsblatt hinzu. Das Arbeitsblatt wird automatisch am Ende der vorhandenen Arbeitsblätter hinzugefügt.</span><span class="sxs-lookup"><span data-stu-id="82504-p106">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets.</span></span> |
|[<span data-ttu-id="82504-155">pivotTables auflisten</span><span class="sxs-lookup"><span data-stu-id="82504-155">List pivotTables</span></span>](../api/workbookworksheet-list-pivottables.md) |<span data-ttu-id="82504-156">[workbookPivotTable](workbookpivottable.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="82504-156">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="82504-157">Rufen Sie eine workbookPivotTable-Objektsammlung ab.</span><span class="sxs-lookup"><span data-stu-id="82504-157">Get a workbookPivotTable object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="82504-158">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="82504-158">Properties</span></span>
| <span data-ttu-id="82504-159">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="82504-159">Property</span></span>     | <span data-ttu-id="82504-160">Typ</span><span class="sxs-lookup"><span data-stu-id="82504-160">Type</span></span>   |<span data-ttu-id="82504-161">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82504-161">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82504-162">id</span><span class="sxs-lookup"><span data-stu-id="82504-162">id</span></span>|<span data-ttu-id="82504-163">string</span><span class="sxs-lookup"><span data-stu-id="82504-163">string</span></span>|<span data-ttu-id="82504-p107">Gibt einen Wert zurück, der das Arbeitsblatt in einer bestimmten Arbeitsmappe eindeutig identifiziert. Der Wert des Bezeichners bleibt unverändert, auch wenn das Arbeitsblatt umbenannt oder verschoben wird. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="82504-p107">Returns a value that uniquely identifies the worksheet in a given workbook. The value of the identifier remains the same even when the worksheet is renamed or moved. Read-only.</span></span>|
|<span data-ttu-id="82504-167">name</span><span class="sxs-lookup"><span data-stu-id="82504-167">name</span></span>|<span data-ttu-id="82504-168">string</span><span class="sxs-lookup"><span data-stu-id="82504-168">string</span></span>|<span data-ttu-id="82504-169">Der Anzeigename des Arbeitsblatts.</span><span class="sxs-lookup"><span data-stu-id="82504-169">The display name of the worksheet.</span></span>|
|<span data-ttu-id="82504-170">position</span><span class="sxs-lookup"><span data-stu-id="82504-170">position</span></span>|<span data-ttu-id="82504-171">int</span><span class="sxs-lookup"><span data-stu-id="82504-171">int</span></span>|<span data-ttu-id="82504-172">Die nullbasiert Position des Arbeitsblatts in der Arbeitsmappe.</span><span class="sxs-lookup"><span data-stu-id="82504-172">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="82504-173">visibility</span><span class="sxs-lookup"><span data-stu-id="82504-173">visibility</span></span>|<span data-ttu-id="82504-174">string</span><span class="sxs-lookup"><span data-stu-id="82504-174">string</span></span>|<span data-ttu-id="82504-p108">Die Sichtbarkeit des Arbeitsblatts. Mögliche Werte: `Visible`, `Hidden`, `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="82504-p108">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82504-177">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="82504-177">Relationships</span></span>
| <span data-ttu-id="82504-178">Beziehung</span><span class="sxs-lookup"><span data-stu-id="82504-178">Relationship</span></span> | <span data-ttu-id="82504-179">Typ</span><span class="sxs-lookup"><span data-stu-id="82504-179">Type</span></span>   |<span data-ttu-id="82504-180">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="82504-180">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82504-181">charts</span><span class="sxs-lookup"><span data-stu-id="82504-181">charts</span></span>|<span data-ttu-id="82504-182">[Diagrammsammlung](chart.md)</span><span class="sxs-lookup"><span data-stu-id="82504-182">[Chart](chart.md) collection</span></span>|<span data-ttu-id="82504-p109">Gibt die Sammlung von Diagrammen zurück, die Teil des Arbeitsblatts sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="82504-p109">Returns collection of charts that are part of the worksheet. Read-only.</span></span>|
|<span data-ttu-id="82504-185">names</span><span class="sxs-lookup"><span data-stu-id="82504-185">names</span></span>|<span data-ttu-id="82504-186">[NamedItem](nameditem.md) collection</span><span class="sxs-lookup"><span data-stu-id="82504-186">[NamedItem](nameditem.md) collection</span></span>|<span data-ttu-id="82504-p110">Gibt die Sammlung von Namen zurück, die mit dem Arbeitsblatt verknüpft sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="82504-p110">Returns collection of names that are associated with the worksheet. Read-only.</span></span>|
|<span data-ttu-id="82504-189">pivotTables</span><span class="sxs-lookup"><span data-stu-id="82504-189">pivotTables</span></span>|<span data-ttu-id="82504-190">[workbookPivotTable](workbookpivottable.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="82504-190">[workbookPivotTable](workbookpivottable.md) collection</span></span>| <span data-ttu-id="82504-191">Die Sammlung von PivotTables, die Teil des Arbeitsblatts sind.</span><span class="sxs-lookup"><span data-stu-id="82504-191">Collection of PivotTables that are part of the worksheet.</span></span> |
|<span data-ttu-id="82504-192">Schutz</span><span class="sxs-lookup"><span data-stu-id="82504-192">protection</span></span>|[<span data-ttu-id="82504-193">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="82504-193">WorksheetProtection</span></span>](worksheetprotection.md)|<span data-ttu-id="82504-p111">Gibt das Arbeitsblattschutz-Objekt für ein Arbeitsblatt zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="82504-p111">Returns sheet protection object for a worksheet. Read-only.</span></span>|
|<span data-ttu-id="82504-196">Tabellen</span><span class="sxs-lookup"><span data-stu-id="82504-196">tables</span></span>|<span data-ttu-id="82504-197">[Table](table.md) collection</span><span class="sxs-lookup"><span data-stu-id="82504-197">[Table](table.md) collection</span></span>|<span data-ttu-id="82504-p112">Gibt die Sammlung von Tabellen zurück, die Teil des Arbeitsblatts sind. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="82504-p112">Collection of tables that are part of the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="82504-200">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="82504-200">JSON representation</span></span>

<span data-ttu-id="82504-201">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="82504-201">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheet"
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
