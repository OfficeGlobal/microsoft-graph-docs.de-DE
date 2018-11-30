---
title: Ressourcentyp rangeView
description: RangeView stellt einen Satz von sichtbaren Zellen des übergeordneten Bereichs dar.
ms.openlocfilehash: e7a19464e52f694705f2e22795513110ae7cbd89
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016116"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="35213-103">Ressourcentyp rangeView</span><span class="sxs-lookup"><span data-stu-id="35213-103">rangeView resource type</span></span>
<span data-ttu-id="35213-104">RangeView stellt einen Satz von sichtbaren Zellen des übergeordneten Bereichs dar.</span><span class="sxs-lookup"><span data-stu-id="35213-104">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="35213-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="35213-105">Methods</span></span>

| <span data-ttu-id="35213-106">Methode</span><span class="sxs-lookup"><span data-stu-id="35213-106">Method</span></span>           | <span data-ttu-id="35213-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="35213-107">Return Type</span></span>    |<span data-ttu-id="35213-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35213-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="35213-109">Zeilen auflisten</span><span class="sxs-lookup"><span data-stu-id="35213-109">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="35213-110">[workbookRangeView](workbookrangeview.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="35213-110">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="35213-111">Rufen Sie eine workbookRangeView-Objektsammlung ab.</span><span class="sxs-lookup"><span data-stu-id="35213-111">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="35213-112">Itemat</span><span class="sxs-lookup"><span data-stu-id="35213-112">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="35213-113">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="35213-113">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="35213-114">Rufen Sie ein im Index basiertes RangeView-Element ab.</span><span class="sxs-lookup"><span data-stu-id="35213-114">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="35213-115">Range</span><span class="sxs-lookup"><span data-stu-id="35213-115">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="35213-116">workbookRange</span><span class="sxs-lookup"><span data-stu-id="35213-116">workbookRange</span></span>](range.md)|<span data-ttu-id="35213-117">Rufen Sie das Range-Objekt ab, das mit der Bereichsansicht verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="35213-117">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="35213-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="35213-118">Properties</span></span>
| <span data-ttu-id="35213-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="35213-119">Property</span></span>     | <span data-ttu-id="35213-120">Typ</span><span class="sxs-lookup"><span data-stu-id="35213-120">Type</span></span>   |<span data-ttu-id="35213-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35213-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35213-122">cellAddresses</span><span class="sxs-lookup"><span data-stu-id="35213-122">cellAddresses</span></span>|<span data-ttu-id="35213-123">Json</span><span class="sxs-lookup"><span data-stu-id="35213-123">Json</span></span>|<span data-ttu-id="35213-124">Stellt die Zelle Adressen</span><span class="sxs-lookup"><span data-stu-id="35213-124">Represents the cell addresses</span></span>
|<span data-ttu-id="35213-125">columnCount</span><span class="sxs-lookup"><span data-stu-id="35213-125">columnCount</span></span>|<span data-ttu-id="35213-126">Int32</span><span class="sxs-lookup"><span data-stu-id="35213-126">Int32</span></span>|<span data-ttu-id="35213-p101">Gibt die Anzahl der sichtbaren Spalten zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="35213-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="35213-129">formulas</span><span class="sxs-lookup"><span data-stu-id="35213-129">formulas</span></span>|<span data-ttu-id="35213-130">Json</span><span class="sxs-lookup"><span data-stu-id="35213-130">Json</span></span>|<span data-ttu-id="35213-131">Stellt die Formel in der A1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="35213-131">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="35213-132">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="35213-132">formulasLocal</span></span>|<span data-ttu-id="35213-133">Json</span><span class="sxs-lookup"><span data-stu-id="35213-133">Json</span></span>|<span data-ttu-id="35213-p102">Stellt die Formel in der A1-Schreibweise, Sprache des Benutzers und im Gebietsschema der Zahlenformatierung dar. Beispielsweise würde die englische Formel "= SUM(A1, 1.5)" in Deutsch "= SUMME(A1; 1,5) " werden.</span><span class="sxs-lookup"><span data-stu-id="35213-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="35213-136">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="35213-136">formulasR1C1</span></span>|<span data-ttu-id="35213-137">Json</span><span class="sxs-lookup"><span data-stu-id="35213-137">Json</span></span>|<span data-ttu-id="35213-138">Stellt die Formel in der R1C1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="35213-138">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="35213-139">Index</span><span class="sxs-lookup"><span data-stu-id="35213-139">index</span></span>|<span data-ttu-id="35213-140">Int32</span><span class="sxs-lookup"><span data-stu-id="35213-140">Int32</span></span>|<span data-ttu-id="35213-141">Der Index des Bereichs.</span><span class="sxs-lookup"><span data-stu-id="35213-141">Index of the range.</span></span>|
|<span data-ttu-id="35213-142">numberFormat</span><span class="sxs-lookup"><span data-stu-id="35213-142">numberFormat</span></span>|<span data-ttu-id="35213-143">Json</span><span class="sxs-lookup"><span data-stu-id="35213-143">Json</span></span>|<span data-ttu-id="35213-p103">Stellt den Excel-Zahlenformatcode für die angegebene Zelle dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="35213-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="35213-146">rowCount</span><span class="sxs-lookup"><span data-stu-id="35213-146">rowCount</span></span>|<span data-ttu-id="35213-147">Int32</span><span class="sxs-lookup"><span data-stu-id="35213-147">Int32</span></span>|<span data-ttu-id="35213-p104">Gibt die Anzahl der sichtbaren Zeilen zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="35213-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="35213-150">text</span><span class="sxs-lookup"><span data-stu-id="35213-150">text</span></span>|<span data-ttu-id="35213-151">Json</span><span class="sxs-lookup"><span data-stu-id="35213-151">Json</span></span>|<span data-ttu-id="35213-p105">Textwerte des angegebenen Bereichs. Der Textwert hängt nicht von der Zellenbreite ab. Die Ersetzung des #-Zeichens, die in der Excel-Benutzeroberfläche passiert, wirkt sich nicht auf den von der API zurückgegebenen Textwert aus. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="35213-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="35213-156">valueTypes</span><span class="sxs-lookup"><span data-stu-id="35213-156">valueTypes</span></span>|<span data-ttu-id="35213-157">Json</span><span class="sxs-lookup"><span data-stu-id="35213-157">Json</span></span>|<span data-ttu-id="35213-158">Stellt den Typ der Daten, die jeder Zelle an.</span><span class="sxs-lookup"><span data-stu-id="35213-158">Represents the type of data of each cell.</span></span> <span data-ttu-id="35213-159">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="35213-159">Read-only.</span></span> <span data-ttu-id="35213-160">Die möglichen Werte sind: unbekannt, leer, String, Integer, Double, Boolean, Fehler.</span><span class="sxs-lookup"><span data-stu-id="35213-160">The possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="35213-161">values</span><span class="sxs-lookup"><span data-stu-id="35213-161">values</span></span>|<span data-ttu-id="35213-162">Json</span><span class="sxs-lookup"><span data-stu-id="35213-162">Json</span></span>|<span data-ttu-id="35213-p107">Stellt die Rohwerte der angegebenen Bereichsansicht dar. Die zurückgegebenen Daten können vom Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zellen, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.</span><span class="sxs-lookup"><span data-stu-id="35213-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="35213-166">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="35213-166">Relationships</span></span>
| <span data-ttu-id="35213-167">Beziehung</span><span class="sxs-lookup"><span data-stu-id="35213-167">Relationship</span></span> | <span data-ttu-id="35213-168">Typ</span><span class="sxs-lookup"><span data-stu-id="35213-168">Type</span></span>   |<span data-ttu-id="35213-169">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="35213-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35213-170">Rows</span><span class="sxs-lookup"><span data-stu-id="35213-170">rows</span></span>|<span data-ttu-id="35213-171">[workbookRangeView](workbookrangeview.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="35213-171">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="35213-p108">Stellt eine Sammlung der mit dem Bereich verknüpften Bereichsansichten dar. Schreibgeschützt.    Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="35213-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35213-175">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="35213-175">JSON representation</span></span>
<span data-ttu-id="35213-176">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="35213-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookRangeView"
}-->
```json
{
  "cellAddresses": "Json",
  "columnCount": 1024,
  "formulas": "Json",
  "formulasLocal": "Json",
  "formulasR1C1": "Json",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```
