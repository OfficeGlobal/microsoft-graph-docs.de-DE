---
title: Ressourcentyp rangeFormat
description: Gibt ein Formatobjekt zurück, das die Schriftart des Bereichs, Füllung, Rahmen, die Ausrichtung und andere Eigenschaften verschachtelt.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 1394153a09a30c273280dab5469a40e2e0c2c4ad
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572423"
---
# <a name="rangeformat-resource-type"></a><span data-ttu-id="56127-103">RangeFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="56127-103">RangeFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56127-104">Gibt ein Formatobjekt zurück, das die Schriftart des Bereichs, Füllung, Rahmen, die Ausrichtung und andere Eigenschaften verschachtelt.</span><span class="sxs-lookup"><span data-stu-id="56127-104">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="56127-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="56127-105">Methods</span></span>

| <span data-ttu-id="56127-106">Methode</span><span class="sxs-lookup"><span data-stu-id="56127-106">Method</span></span>           | <span data-ttu-id="56127-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="56127-107">Return Type</span></span>    |<span data-ttu-id="56127-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56127-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="56127-109">RangeFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="56127-109">Get RangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="56127-110">RangeFormat</span><span class="sxs-lookup"><span data-stu-id="56127-110">RangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="56127-111">Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="56127-111">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="56127-112">RangeBorder erstellen</span><span class="sxs-lookup"><span data-stu-id="56127-112">Create RangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="56127-113">rangeBorder</span><span class="sxs-lookup"><span data-stu-id="56127-113">rangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="56127-114">Dient zum Erstellen eines neues RangeBorder durch Veröffentlichen in der Rahmensammlung.</span><span class="sxs-lookup"><span data-stu-id="56127-114">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="56127-115">Rahmen auflisten</span><span class="sxs-lookup"><span data-stu-id="56127-115">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="56127-116">[RangeBorder](rangeborder.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="56127-116">[rangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="56127-117">Dient zum Abrufen einer RangeBorder-Objeksammlung.</span><span class="sxs-lookup"><span data-stu-id="56127-117">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="56127-118">Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="56127-118">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="56127-119">rangeFormat</span><span class="sxs-lookup"><span data-stu-id="56127-119">rangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="56127-120">Dient zum Aktualisieren des RangeFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="56127-120">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="56127-121">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="56127-121">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="56127-122">Keine</span><span class="sxs-lookup"><span data-stu-id="56127-122">None</span></span>|<span data-ttu-id="56127-123">Ändert die Breite der Spalten des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Spalten die optimale Breite zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="56127-123">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="56127-124">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="56127-124">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="56127-125">Keine</span><span class="sxs-lookup"><span data-stu-id="56127-125">None</span></span>|<span data-ttu-id="56127-126">Ändert die Höhe der Zeilen des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Zeilen die optimale Höhe zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="56127-126">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="56127-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="56127-127">Properties</span></span>
| <span data-ttu-id="56127-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="56127-128">Property</span></span>     | <span data-ttu-id="56127-129">Typ</span><span class="sxs-lookup"><span data-stu-id="56127-129">Type</span></span>   |<span data-ttu-id="56127-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56127-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56127-131">columnWidth</span><span class="sxs-lookup"><span data-stu-id="56127-131">columnWidth</span></span>|<span data-ttu-id="56127-132">double</span><span class="sxs-lookup"><span data-stu-id="56127-132">double</span></span>|<span data-ttu-id="56127-p101">Ruft die Breite aller Spalten innerhalb des Bereichs ab oder legt diese fest. Wenn die Breite der Spalten nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56127-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="56127-135">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="56127-135">horizontalAlignment</span></span>|<span data-ttu-id="56127-136">string</span><span class="sxs-lookup"><span data-stu-id="56127-136">string</span></span>|<span data-ttu-id="56127-p102">Stellt die horizontale Ausrichtung für das angegebene Objekt dar. Mögliche Werte: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="56127-p102">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="56127-139">rowHeight</span><span class="sxs-lookup"><span data-stu-id="56127-139">rowHeight</span></span>|<span data-ttu-id="56127-140">double</span><span class="sxs-lookup"><span data-stu-id="56127-140">double</span></span>|<span data-ttu-id="56127-p103">Ruft die Höhe aller Zeilen des Bereichs ab oder legt diese fest. Wenn die Höhe der Zeilen nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56127-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="56127-143">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="56127-143">verticalAlignment</span></span>|<span data-ttu-id="56127-144">string</span><span class="sxs-lookup"><span data-stu-id="56127-144">string</span></span>|<span data-ttu-id="56127-p104">Stellt die vertikale Ausrichtung für das angegebene Objekt dar. Mögliche Werte: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="56127-p104">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="56127-147">wrapText</span><span class="sxs-lookup"><span data-stu-id="56127-147">wrapText</span></span>|<span data-ttu-id="56127-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="56127-148">boolean</span></span>|<span data-ttu-id="56127-p105">Gibt an, ob Excel den Text im Objekt umbricht. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Textumbruch-Einstellung hat</span><span class="sxs-lookup"><span data-stu-id="56127-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="56127-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="56127-151">Relationships</span></span>
| <span data-ttu-id="56127-152">Beziehung</span><span class="sxs-lookup"><span data-stu-id="56127-152">Relationship</span></span> | <span data-ttu-id="56127-153">Typ</span><span class="sxs-lookup"><span data-stu-id="56127-153">Type</span></span>   |<span data-ttu-id="56127-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56127-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56127-155">Borders</span><span class="sxs-lookup"><span data-stu-id="56127-155">borders</span></span>|<span data-ttu-id="56127-156">[RangeBorder](rangeborder.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="56127-156">[rangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="56127-157">Auflistung von Border-Objekten, die für den gesamten ausgewählten Bereich gelten, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="56127-157">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="56127-158">fill</span><span class="sxs-lookup"><span data-stu-id="56127-158">fill</span></span>|[<span data-ttu-id="56127-159">rangeFill</span><span class="sxs-lookup"><span data-stu-id="56127-159">rangeFill</span></span>](rangefill.md)|<span data-ttu-id="56127-p106">Gibt das Fill-Objekt an, das für den gesamten Bereich definiert ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="56127-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="56127-162">Schriftart</span><span class="sxs-lookup"><span data-stu-id="56127-162">font</span></span>|[<span data-ttu-id="56127-163">rangeFont</span><span class="sxs-lookup"><span data-stu-id="56127-163">rangeFont</span></span>](rangefont.md)|<span data-ttu-id="56127-164">Gibt das Font-Objekt zurück, das für den gesamten ausgewählten Bereich definiert ist, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="56127-164">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="56127-165">protection</span><span class="sxs-lookup"><span data-stu-id="56127-165">protection</span></span>|[<span data-ttu-id="56127-166">formatProtection</span><span class="sxs-lookup"><span data-stu-id="56127-166">formatProtection</span></span>](formatprotection.md)|<span data-ttu-id="56127-p107">Gibt das Formatschutz-Objekt für einen Bereich zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="56127-p107">Returns the format protection object for a range. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56127-169">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="56127-169">JSON representation</span></span>

<span data-ttu-id="56127-170">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="56127-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFormat"
}-->

```json
{
  "columnWidth": 1024,
  "horizontalAlignment": "string",
  "rowHeight": 1024,
  "verticalAlignment": "string",
  "wrapText": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rangeformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
