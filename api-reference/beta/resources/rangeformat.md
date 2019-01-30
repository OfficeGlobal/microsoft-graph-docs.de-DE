---
title: RangeFormat-Ressourcentyp
description: Gibt ein Formatobjekt zurück, das die Schriftart des Bereichs, Füllung, Rahmen, die Ausrichtung und andere Eigenschaften verschachtelt.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 58ed56b11b571237211307c8fb0dd1abaf27761f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643930"
---
# <a name="rangeformat-resource-type"></a><span data-ttu-id="52cda-103">RangeFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="52cda-103">RangeFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52cda-104">Gibt ein Formatobjekt zurück, das die Schriftart des Bereichs, Füllung, Rahmen, die Ausrichtung und andere Eigenschaften verschachtelt.</span><span class="sxs-lookup"><span data-stu-id="52cda-104">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="52cda-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="52cda-105">Methods</span></span>

| <span data-ttu-id="52cda-106">Methode</span><span class="sxs-lookup"><span data-stu-id="52cda-106">Method</span></span>           | <span data-ttu-id="52cda-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="52cda-107">Return Type</span></span>    |<span data-ttu-id="52cda-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52cda-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52cda-109">RangeFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="52cda-109">Get RangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="52cda-110">RangeFormat</span><span class="sxs-lookup"><span data-stu-id="52cda-110">RangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="52cda-111">Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="52cda-111">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="52cda-112">RangeBorder erstellen</span><span class="sxs-lookup"><span data-stu-id="52cda-112">Create RangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="52cda-113">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="52cda-113">RangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="52cda-114">Dient zum Erstellen eines neues RangeBorder durch Veröffentlichen in der Rahmensammlung.</span><span class="sxs-lookup"><span data-stu-id="52cda-114">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="52cda-115">Rahmen auflisten</span><span class="sxs-lookup"><span data-stu-id="52cda-115">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="52cda-116">[RangeBorder-Sammlung](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="52cda-116">[RangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="52cda-117">Dient zum Abrufen einer RangeBorder-Objeksammlung.</span><span class="sxs-lookup"><span data-stu-id="52cda-117">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="52cda-118">Update</span><span class="sxs-lookup"><span data-stu-id="52cda-118">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="52cda-119">RangeFormat</span><span class="sxs-lookup"><span data-stu-id="52cda-119">RangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="52cda-120">Dient zum Aktualisieren des RangeFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="52cda-120">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="52cda-121">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="52cda-121">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="52cda-122">Keine</span><span class="sxs-lookup"><span data-stu-id="52cda-122">None</span></span>|<span data-ttu-id="52cda-123">Ändert die Breite der Spalten des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Spalten die optimale Breite zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="52cda-123">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="52cda-124">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="52cda-124">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="52cda-125">Keine</span><span class="sxs-lookup"><span data-stu-id="52cda-125">None</span></span>|<span data-ttu-id="52cda-126">Ändert die Höhe der Zeilen des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Zeilen die optimale Höhe zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="52cda-126">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="52cda-127">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="52cda-127">Properties</span></span>
| <span data-ttu-id="52cda-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="52cda-128">Property</span></span>     | <span data-ttu-id="52cda-129">Typ</span><span class="sxs-lookup"><span data-stu-id="52cda-129">Type</span></span>   |<span data-ttu-id="52cda-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52cda-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52cda-131">columnWidth</span><span class="sxs-lookup"><span data-stu-id="52cda-131">columnWidth</span></span>|<span data-ttu-id="52cda-132">double</span><span class="sxs-lookup"><span data-stu-id="52cda-132">double</span></span>|<span data-ttu-id="52cda-p101">Ruft die Breite aller Spalten innerhalb des Bereichs ab oder legt diese fest. Wenn die Breite der Spalten nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="52cda-p101">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="52cda-135">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="52cda-135">horizontalAlignment</span></span>|<span data-ttu-id="52cda-136">string</span><span class="sxs-lookup"><span data-stu-id="52cda-136">string</span></span>|<span data-ttu-id="52cda-p102">Stellt die horizontale Ausrichtung für das angegebene Objekt dar. Mögliche Werte: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="52cda-p102">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="52cda-139">rowHeight</span><span class="sxs-lookup"><span data-stu-id="52cda-139">rowHeight</span></span>|<span data-ttu-id="52cda-140">double</span><span class="sxs-lookup"><span data-stu-id="52cda-140">double</span></span>|<span data-ttu-id="52cda-p103">Ruft die Höhe aller Zeilen des Bereichs ab oder legt diese fest. Wenn die Höhe der Zeilen nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="52cda-p103">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="52cda-143">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="52cda-143">verticalAlignment</span></span>|<span data-ttu-id="52cda-144">string</span><span class="sxs-lookup"><span data-stu-id="52cda-144">string</span></span>|<span data-ttu-id="52cda-p104">Stellt die vertikale Ausrichtung für das angegebene Objekt dar. Mögliche Werte: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="52cda-p104">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="52cda-147">wrapText</span><span class="sxs-lookup"><span data-stu-id="52cda-147">wrapText</span></span>|<span data-ttu-id="52cda-148">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="52cda-148">boolean</span></span>|<span data-ttu-id="52cda-p105">Gibt an, ob Excel den Text im Objekt umbricht. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Textumbruch-Einstellung hat</span><span class="sxs-lookup"><span data-stu-id="52cda-p105">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="52cda-151">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="52cda-151">Relationships</span></span>
| <span data-ttu-id="52cda-152">Beziehung</span><span class="sxs-lookup"><span data-stu-id="52cda-152">Relationship</span></span> | <span data-ttu-id="52cda-153">Typ</span><span class="sxs-lookup"><span data-stu-id="52cda-153">Type</span></span>   |<span data-ttu-id="52cda-154">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52cda-154">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52cda-155">Borders</span><span class="sxs-lookup"><span data-stu-id="52cda-155">borders</span></span>|<span data-ttu-id="52cda-156">[RangeBorder-Sammlung](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="52cda-156">[RangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="52cda-157">Auflistung von Border-Objekten, die für den gesamten ausgewählten Bereich gelten, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="52cda-157">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="52cda-158">fill</span><span class="sxs-lookup"><span data-stu-id="52cda-158">fill</span></span>|[<span data-ttu-id="52cda-159">RangeFill</span><span class="sxs-lookup"><span data-stu-id="52cda-159">RangeFill</span></span>](rangefill.md)|<span data-ttu-id="52cda-p106">Gibt das Fill-Objekt an, das für den gesamten Bereich definiert ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="52cda-p106">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="52cda-162">Schriftart</span><span class="sxs-lookup"><span data-stu-id="52cda-162">font</span></span>|[<span data-ttu-id="52cda-163">RangeFont</span><span class="sxs-lookup"><span data-stu-id="52cda-163">RangeFont</span></span>](rangefont.md)|<span data-ttu-id="52cda-164">Gibt das Font-Objekt zurück, das für den gesamten ausgewählten Bereich definiert ist, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="52cda-164">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="52cda-165">protection</span><span class="sxs-lookup"><span data-stu-id="52cda-165">protection</span></span>|[<span data-ttu-id="52cda-166">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="52cda-166">FormatProtection</span></span>](formatprotection.md)|<span data-ttu-id="52cda-p107">Gibt das Formatschutz-Objekt für einen Bereich zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="52cda-p107">Returns the format protection object for a range. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52cda-169">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="52cda-169">JSON representation</span></span>

<span data-ttu-id="52cda-170">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="52cda-170">Here is a JSON representation of the resource.</span></span>

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
