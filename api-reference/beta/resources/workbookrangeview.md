---
title: Ressourcentyp rangeView
description: RangeView stellt einen Satz von sichtbaren Zellen des übergeordneten Bereichs dar.
ms.openlocfilehash: 84ff9d315a6bfa8c4b03fad1b8f05670cb2b155c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064947"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="992e6-103">Ressourcentyp rangeView</span><span class="sxs-lookup"><span data-stu-id="992e6-103">rangeView resource type</span></span>

> <span data-ttu-id="992e6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="992e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="992e6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="992e6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="992e6-106">RangeView stellt einen Satz von sichtbaren Zellen des übergeordneten Bereichs dar.</span><span class="sxs-lookup"><span data-stu-id="992e6-106">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="992e6-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="992e6-107">Methods</span></span>

| <span data-ttu-id="992e6-108">Methode</span><span class="sxs-lookup"><span data-stu-id="992e6-108">Method</span></span>           | <span data-ttu-id="992e6-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="992e6-109">Return Type</span></span>    |<span data-ttu-id="992e6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="992e6-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="992e6-111">Zeilen auflisten</span><span class="sxs-lookup"><span data-stu-id="992e6-111">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="992e6-112">[workbookRangeView](workbookrangeview.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="992e6-112">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="992e6-113">Rufen Sie eine workbookRangeView-Objektsammlung ab.</span><span class="sxs-lookup"><span data-stu-id="992e6-113">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="992e6-114">Itemat</span><span class="sxs-lookup"><span data-stu-id="992e6-114">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="992e6-115">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="992e6-115">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="992e6-116">Rufen Sie ein im Index basiertes RangeView-Element ab.</span><span class="sxs-lookup"><span data-stu-id="992e6-116">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="992e6-117">Range</span><span class="sxs-lookup"><span data-stu-id="992e6-117">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="992e6-118">workbookRange</span><span class="sxs-lookup"><span data-stu-id="992e6-118">workbookRange</span></span>](range.md)|<span data-ttu-id="992e6-119">Rufen Sie das Range-Objekt ab, das mit der Bereichsansicht verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="992e6-119">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="992e6-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="992e6-120">Properties</span></span>
| <span data-ttu-id="992e6-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="992e6-121">Property</span></span>     | <span data-ttu-id="992e6-122">Typ</span><span class="sxs-lookup"><span data-stu-id="992e6-122">Type</span></span>   |<span data-ttu-id="992e6-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="992e6-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="992e6-124">columnCount</span><span class="sxs-lookup"><span data-stu-id="992e6-124">columnCount</span></span>|<span data-ttu-id="992e6-125">Int32</span><span class="sxs-lookup"><span data-stu-id="992e6-125">Int32</span></span>|<span data-ttu-id="992e6-p102">Gibt die Anzahl der sichtbaren Spalten zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="992e6-p102">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="992e6-128">formulas</span><span class="sxs-lookup"><span data-stu-id="992e6-128">formulas</span></span>|<span data-ttu-id="992e6-129">Json</span><span class="sxs-lookup"><span data-stu-id="992e6-129">Json</span></span>|<span data-ttu-id="992e6-130">Stellt die Formel in der A1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="992e6-130">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="992e6-131">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="992e6-131">formulasLocal</span></span>|<span data-ttu-id="992e6-132">Json</span><span class="sxs-lookup"><span data-stu-id="992e6-132">Json</span></span>|<span data-ttu-id="992e6-p103">Stellt die Formel in der A1-Schreibweise, Sprache des Benutzers und im Gebietsschema der Zahlenformatierung dar. Beispielsweise würde die englische Formel "= SUM(A1, 1.5)" in Deutsch "= SUMME(A1; 1,5) " werden.</span><span class="sxs-lookup"><span data-stu-id="992e6-p103">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="992e6-135">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="992e6-135">formulasR1C1</span></span>|<span data-ttu-id="992e6-136">Json</span><span class="sxs-lookup"><span data-stu-id="992e6-136">Json</span></span>|<span data-ttu-id="992e6-137">Stellt die Formel in der R1C1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="992e6-137">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="992e6-138">Index</span><span class="sxs-lookup"><span data-stu-id="992e6-138">index</span></span>|<span data-ttu-id="992e6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="992e6-139">Int32</span></span>|<span data-ttu-id="992e6-140">Der Index des Bereichs.</span><span class="sxs-lookup"><span data-stu-id="992e6-140">Index of the range.</span></span>|
|<span data-ttu-id="992e6-141">numberFormat</span><span class="sxs-lookup"><span data-stu-id="992e6-141">numberFormat</span></span>|<span data-ttu-id="992e6-142">Json</span><span class="sxs-lookup"><span data-stu-id="992e6-142">Json</span></span>|<span data-ttu-id="992e6-p104">Stellt den Excel-Zahlenformatcode für die angegebene Zelle dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="992e6-p104">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="992e6-145">rowCount</span><span class="sxs-lookup"><span data-stu-id="992e6-145">rowCount</span></span>|<span data-ttu-id="992e6-146">Int32</span><span class="sxs-lookup"><span data-stu-id="992e6-146">Int32</span></span>|<span data-ttu-id="992e6-p105">Gibt die Anzahl der sichtbaren Zeilen zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="992e6-p105">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="992e6-149">text</span><span class="sxs-lookup"><span data-stu-id="992e6-149">text</span></span>|<span data-ttu-id="992e6-150">Json</span><span class="sxs-lookup"><span data-stu-id="992e6-150">Json</span></span>|<span data-ttu-id="992e6-p106">Textwerte des angegebenen Bereichs. Der Textwert hängt nicht von der Zellenbreite ab. Die Ersetzung des #-Zeichens, die in der Excel-Benutzeroberfläche passiert, wirkt sich nicht auf den von der API zurückgegebenen Textwert aus. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="992e6-p106">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="992e6-155">valueTypes</span><span class="sxs-lookup"><span data-stu-id="992e6-155">valueTypes</span></span>|<span data-ttu-id="992e6-156">Json</span><span class="sxs-lookup"><span data-stu-id="992e6-156">Json</span></span>|<span data-ttu-id="992e6-p107">Stellt den Datentyp in jeder Zelle dar. Schreibgeschützt. Die folgenden Werte sind möglich: Unbekannt, leer, Zeichenfolge, Ganzzahl, Doppelwort, Boolesch, Fehler.</span><span class="sxs-lookup"><span data-stu-id="992e6-p107">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="992e6-160">values</span><span class="sxs-lookup"><span data-stu-id="992e6-160">values</span></span>|<span data-ttu-id="992e6-161">Json</span><span class="sxs-lookup"><span data-stu-id="992e6-161">Json</span></span>|<span data-ttu-id="992e6-p108">Stellt die Rohwerte der angegebenen Bereichsansicht dar. Die zurückgegebenen Daten können vom Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zellen, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.</span><span class="sxs-lookup"><span data-stu-id="992e6-p108">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="992e6-165">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="992e6-165">Relationships</span></span>
| <span data-ttu-id="992e6-166">Beziehung</span><span class="sxs-lookup"><span data-stu-id="992e6-166">Relationship</span></span> | <span data-ttu-id="992e6-167">Typ</span><span class="sxs-lookup"><span data-stu-id="992e6-167">Type</span></span>   |<span data-ttu-id="992e6-168">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="992e6-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="992e6-169">Rows</span><span class="sxs-lookup"><span data-stu-id="992e6-169">rows</span></span>|<span data-ttu-id="992e6-170">[workbookRangeView](workbookrangeview.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="992e6-170">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="992e6-p109">Stellt eine Sammlung der mit dem Bereich verknüpften Bereichsansichten dar. Schreibgeschützt.    Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="992e6-p109">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="992e6-174">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="992e6-174">JSON representation</span></span>
<span data-ttu-id="992e6-175">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="992e6-175">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
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
  "id": "String (identifier)",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```