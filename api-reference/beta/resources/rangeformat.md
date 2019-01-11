---
title: RangeFormat-Ressourcentyp
description: Gibt ein Formatobjekt zurück, das die Schriftart des Bereichs, Füllung, Rahmen, die Ausrichtung und andere Eigenschaften verschachtelt.
localization_priority: Normal
ms.openlocfilehash: 38844e2f43dcb56021e25ad189529b36cc8eb456
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880766"
---
# <a name="rangeformat-resource-type"></a><span data-ttu-id="43054-103">RangeFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="43054-103">RangeFormat resource type</span></span>

> <span data-ttu-id="43054-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="43054-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43054-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="43054-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="43054-106">Gibt ein Formatobjekt zurück, das die Schriftart des Bereichs, Füllung, Rahmen, die Ausrichtung und andere Eigenschaften verschachtelt.</span><span class="sxs-lookup"><span data-stu-id="43054-106">A format object encapsulating the range's font, fill, borders, alignment, and other properties.</span></span>


## <a name="methods"></a><span data-ttu-id="43054-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="43054-107">Methods</span></span>

| <span data-ttu-id="43054-108">Methode</span><span class="sxs-lookup"><span data-stu-id="43054-108">Method</span></span>           | <span data-ttu-id="43054-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="43054-109">Return Type</span></span>    |<span data-ttu-id="43054-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43054-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="43054-111">RangeFormat abrufen</span><span class="sxs-lookup"><span data-stu-id="43054-111">Get RangeFormat</span></span>](../api/rangeformat-get.md) | [<span data-ttu-id="43054-112">RangeFormat</span><span class="sxs-lookup"><span data-stu-id="43054-112">RangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="43054-113">Dient zum Lesen der Eigenschaften und der Beziehungen des rangeFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="43054-113">Read properties and relationships of rangeFormat object.</span></span>|
|[<span data-ttu-id="43054-114">RangeBorder erstellen</span><span class="sxs-lookup"><span data-stu-id="43054-114">Create RangeBorder</span></span>](../api/rangeformat-post-borders.md) |[<span data-ttu-id="43054-115">RangeBorder</span><span class="sxs-lookup"><span data-stu-id="43054-115">RangeBorder</span></span>](rangeborder.md)| <span data-ttu-id="43054-116">Dient zum Erstellen eines neues RangeBorder durch Veröffentlichen in der Rahmensammlung.</span><span class="sxs-lookup"><span data-stu-id="43054-116">Create a new RangeBorder by posting to the borders collection.</span></span>|
|[<span data-ttu-id="43054-117">Rahmen auflisten</span><span class="sxs-lookup"><span data-stu-id="43054-117">List borders</span></span>](../api/rangeformat-list-borders.md) |<span data-ttu-id="43054-118">[RangeBorder-Sammlung](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="43054-118">[RangeBorder](rangeborder.md) collection</span></span>| <span data-ttu-id="43054-119">Dient zum Abrufen einer RangeBorder-Objeksammlung.</span><span class="sxs-lookup"><span data-stu-id="43054-119">Get a RangeBorder object collection.</span></span>|
|[<span data-ttu-id="43054-120">Update</span><span class="sxs-lookup"><span data-stu-id="43054-120">Update</span></span>](../api/rangeformat-update.md) | [<span data-ttu-id="43054-121">RangeFormat</span><span class="sxs-lookup"><span data-stu-id="43054-121">RangeFormat</span></span>](rangeformat.md) |<span data-ttu-id="43054-122">Dient zum Aktualisieren des RangeFormat-Objekts.</span><span class="sxs-lookup"><span data-stu-id="43054-122">Update RangeFormat object.</span></span> |
|[<span data-ttu-id="43054-123">Autofitcolumns</span><span class="sxs-lookup"><span data-stu-id="43054-123">Autofitcolumns</span></span>](../api/rangeformat-autofitcolumns.md)|<span data-ttu-id="43054-124">Keine</span><span class="sxs-lookup"><span data-stu-id="43054-124">None</span></span>|<span data-ttu-id="43054-125">Ändert die Breite der Spalten des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Spalten die optimale Breite zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="43054-125">Changes the width of the columns of the current range to achieve the best fit, based on the current data in the columns.</span></span>|
|[<span data-ttu-id="43054-126">Autofitrows</span><span class="sxs-lookup"><span data-stu-id="43054-126">Autofitrows</span></span>](../api/rangeformat-autofitrows.md)|<span data-ttu-id="43054-127">Keine</span><span class="sxs-lookup"><span data-stu-id="43054-127">None</span></span>|<span data-ttu-id="43054-128">Ändert die Höhe der Zeilen des aktuellen Bereichs, um basierend auf den aktuellen Daten in den Zeilen die optimale Höhe zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="43054-128">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>|

## <a name="properties"></a><span data-ttu-id="43054-129">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="43054-129">Properties</span></span>
| <span data-ttu-id="43054-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="43054-130">Property</span></span>     | <span data-ttu-id="43054-131">Typ</span><span class="sxs-lookup"><span data-stu-id="43054-131">Type</span></span>   |<span data-ttu-id="43054-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43054-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43054-133">columnWidth</span><span class="sxs-lookup"><span data-stu-id="43054-133">columnWidth</span></span>|<span data-ttu-id="43054-134">double</span><span class="sxs-lookup"><span data-stu-id="43054-134">double</span></span>|<span data-ttu-id="43054-p102">Ruft die Breite aller Spalten innerhalb des Bereichs ab oder legt diese fest. Wenn die Breite der Spalten nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43054-p102">Gets or sets the width of all colums within the range. If the column widths are not uniform, null will be returned.</span></span>|
|<span data-ttu-id="43054-137">horizontalAlignment</span><span class="sxs-lookup"><span data-stu-id="43054-137">horizontalAlignment</span></span>|<span data-ttu-id="43054-138">string</span><span class="sxs-lookup"><span data-stu-id="43054-138">string</span></span>|<span data-ttu-id="43054-p103">Stellt die horizontale Ausrichtung für das angegebene Objekt dar. Mögliche Werte: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="43054-p103">Represents the horizontal alignment for the specified object. Possible values are: `General`, `Left`, `Center`, `Right`, `Fill`, `Justify`, `CenterAcrossSelection`, `Distributed`.</span></span>|
|<span data-ttu-id="43054-141">rowHeight</span><span class="sxs-lookup"><span data-stu-id="43054-141">rowHeight</span></span>|<span data-ttu-id="43054-142">double</span><span class="sxs-lookup"><span data-stu-id="43054-142">double</span></span>|<span data-ttu-id="43054-p104">Ruft die Höhe aller Zeilen des Bereichs ab oder legt diese fest. Wenn die Höhe der Zeilen nicht gleichmäßig ist, wird Null zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="43054-p104">Gets or sets the height of all rows in the range. If the row heights are not uniform null will be returned.</span></span>|
|<span data-ttu-id="43054-145">verticalAlignment</span><span class="sxs-lookup"><span data-stu-id="43054-145">verticalAlignment</span></span>|<span data-ttu-id="43054-146">string</span><span class="sxs-lookup"><span data-stu-id="43054-146">string</span></span>|<span data-ttu-id="43054-p105">Stellt die vertikale Ausrichtung für das angegebene Objekt dar. Mögliche Werte: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span><span class="sxs-lookup"><span data-stu-id="43054-p105">Represents the vertical alignment for the specified object. Possible values are: `Top`, `Center`, `Bottom`, `Justify`, `Distributed`.</span></span>|
|<span data-ttu-id="43054-149">wrapText</span><span class="sxs-lookup"><span data-stu-id="43054-149">wrapText</span></span>|<span data-ttu-id="43054-150">boolean</span><span class="sxs-lookup"><span data-stu-id="43054-150">boolean</span></span>|<span data-ttu-id="43054-p106">Gibt an, ob Excel den Text im Objekt umbricht. Ein Nullwert gibt an, dass der gesamte Bereich keine einheitliche Textumbruch-Einstellung hat</span><span class="sxs-lookup"><span data-stu-id="43054-p106">Indicates if Excel wraps the text in the object. A null value indicates that the entire range doesn't have uniform wrap setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="43054-153">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="43054-153">Relationships</span></span>
| <span data-ttu-id="43054-154">Beziehung</span><span class="sxs-lookup"><span data-stu-id="43054-154">Relationship</span></span> | <span data-ttu-id="43054-155">Typ</span><span class="sxs-lookup"><span data-stu-id="43054-155">Type</span></span>   |<span data-ttu-id="43054-156">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="43054-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43054-157">Borders</span><span class="sxs-lookup"><span data-stu-id="43054-157">borders</span></span>|<span data-ttu-id="43054-158">[RangeBorder-Sammlung](rangeborder.md)</span><span class="sxs-lookup"><span data-stu-id="43054-158">[RangeBorder](rangeborder.md) collection</span></span>|<span data-ttu-id="43054-159">Auflistung von Border-Objekten, die für den gesamten ausgewählten Bereich gelten, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="43054-159">Collection of border objects that apply to the overall range selected Read-only.</span></span>|
|<span data-ttu-id="43054-160">fill</span><span class="sxs-lookup"><span data-stu-id="43054-160">fill</span></span>|[<span data-ttu-id="43054-161">RangeFill</span><span class="sxs-lookup"><span data-stu-id="43054-161">RangeFill</span></span>](rangefill.md)|<span data-ttu-id="43054-p107">Gibt das Fill-Objekt an, das für den gesamten Bereich definiert ist. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="43054-p107">Returns the fill object defined on the overall range. Read-only.</span></span>|
|<span data-ttu-id="43054-164">Schriftart</span><span class="sxs-lookup"><span data-stu-id="43054-164">font</span></span>|[<span data-ttu-id="43054-165">RangeFont</span><span class="sxs-lookup"><span data-stu-id="43054-165">RangeFont</span></span>](rangefont.md)|<span data-ttu-id="43054-166">Gibt das Font-Objekt zurück, das für den gesamten ausgewählten Bereich definiert ist, schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="43054-166">Returns the font object defined on the overall range selected Read-only.</span></span>|
|<span data-ttu-id="43054-167">protection</span><span class="sxs-lookup"><span data-stu-id="43054-167">protection</span></span>|[<span data-ttu-id="43054-168">FormatProtection</span><span class="sxs-lookup"><span data-stu-id="43054-168">FormatProtection</span></span>](formatprotection.md)|<span data-ttu-id="43054-p108">Gibt das Formatschutz-Objekt für einen Bereich zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="43054-p108">Returns the format protection object for a range. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43054-171">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="43054-171">JSON representation</span></span>

<span data-ttu-id="43054-172">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="43054-172">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
