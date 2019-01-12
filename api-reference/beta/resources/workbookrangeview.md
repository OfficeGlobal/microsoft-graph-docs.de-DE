---
title: Ressourcentyp rangeView
description: RangeView stellt einen Satz von sichtbaren Zellen des übergeordneten Bereichs dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9476b3f4a085f70be51d81a9da667c07db3b9232
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983716"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="87166-103">Ressourcentyp rangeView</span><span class="sxs-lookup"><span data-stu-id="87166-103">rangeView resource type</span></span>

> <span data-ttu-id="87166-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="87166-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87166-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="87166-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="87166-106">RangeView stellt einen Satz von sichtbaren Zellen des übergeordneten Bereichs dar.</span><span class="sxs-lookup"><span data-stu-id="87166-106">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="87166-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="87166-107">Methods</span></span>

| <span data-ttu-id="87166-108">Methode</span><span class="sxs-lookup"><span data-stu-id="87166-108">Method</span></span>           | <span data-ttu-id="87166-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="87166-109">Return Type</span></span>    |<span data-ttu-id="87166-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87166-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="87166-111">Zeilen auflisten</span><span class="sxs-lookup"><span data-stu-id="87166-111">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="87166-112">[workbookRangeView](workbookrangeview.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="87166-112">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="87166-113">Rufen Sie eine workbookRangeView-Objektsammlung ab.</span><span class="sxs-lookup"><span data-stu-id="87166-113">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="87166-114">Itemat</span><span class="sxs-lookup"><span data-stu-id="87166-114">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="87166-115">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="87166-115">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="87166-116">Rufen Sie ein im Index basiertes RangeView-Element ab.</span><span class="sxs-lookup"><span data-stu-id="87166-116">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="87166-117">Range</span><span class="sxs-lookup"><span data-stu-id="87166-117">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="87166-118">workbookRange</span><span class="sxs-lookup"><span data-stu-id="87166-118">workbookRange</span></span>](range.md)|<span data-ttu-id="87166-119">Rufen Sie das Range-Objekt ab, das mit der Bereichsansicht verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="87166-119">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="87166-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="87166-120">Properties</span></span>
| <span data-ttu-id="87166-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="87166-121">Property</span></span>     | <span data-ttu-id="87166-122">Typ</span><span class="sxs-lookup"><span data-stu-id="87166-122">Type</span></span>   |<span data-ttu-id="87166-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87166-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87166-124">columnCount</span><span class="sxs-lookup"><span data-stu-id="87166-124">columnCount</span></span>|<span data-ttu-id="87166-125">Int32</span><span class="sxs-lookup"><span data-stu-id="87166-125">Int32</span></span>|<span data-ttu-id="87166-p102">Gibt die Anzahl der sichtbaren Spalten zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="87166-p102">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="87166-128">formulas</span><span class="sxs-lookup"><span data-stu-id="87166-128">formulas</span></span>|<span data-ttu-id="87166-129">Json</span><span class="sxs-lookup"><span data-stu-id="87166-129">Json</span></span>|<span data-ttu-id="87166-130">Stellt die Formel in der A1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="87166-130">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="87166-131">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="87166-131">formulasLocal</span></span>|<span data-ttu-id="87166-132">Json</span><span class="sxs-lookup"><span data-stu-id="87166-132">Json</span></span>|<span data-ttu-id="87166-p103">Stellt die Formel in der A1-Schreibweise, Sprache des Benutzers und im Gebietsschema der Zahlenformatierung dar. Beispielsweise würde die englische Formel "= SUM(A1, 1.5)" in Deutsch "= SUMME(A1; 1,5) " werden.</span><span class="sxs-lookup"><span data-stu-id="87166-p103">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="87166-135">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="87166-135">formulasR1C1</span></span>|<span data-ttu-id="87166-136">Json</span><span class="sxs-lookup"><span data-stu-id="87166-136">Json</span></span>|<span data-ttu-id="87166-137">Stellt die Formel in der R1C1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="87166-137">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="87166-138">Index</span><span class="sxs-lookup"><span data-stu-id="87166-138">index</span></span>|<span data-ttu-id="87166-139">Int32</span><span class="sxs-lookup"><span data-stu-id="87166-139">Int32</span></span>|<span data-ttu-id="87166-140">Der Index des Bereichs.</span><span class="sxs-lookup"><span data-stu-id="87166-140">Index of the range.</span></span>|
|<span data-ttu-id="87166-141">numberFormat</span><span class="sxs-lookup"><span data-stu-id="87166-141">numberFormat</span></span>|<span data-ttu-id="87166-142">Json</span><span class="sxs-lookup"><span data-stu-id="87166-142">Json</span></span>|<span data-ttu-id="87166-p104">Stellt den Excel-Zahlenformatcode für die angegebene Zelle dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="87166-p104">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="87166-145">rowCount</span><span class="sxs-lookup"><span data-stu-id="87166-145">rowCount</span></span>|<span data-ttu-id="87166-146">Int32</span><span class="sxs-lookup"><span data-stu-id="87166-146">Int32</span></span>|<span data-ttu-id="87166-p105">Gibt die Anzahl der sichtbaren Zeilen zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="87166-p105">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="87166-149">text</span><span class="sxs-lookup"><span data-stu-id="87166-149">text</span></span>|<span data-ttu-id="87166-150">Json</span><span class="sxs-lookup"><span data-stu-id="87166-150">Json</span></span>|<span data-ttu-id="87166-p106">Textwerte des angegebenen Bereichs. Der Textwert hängt nicht von der Zellenbreite ab. Die Ersetzung des #-Zeichens, die in der Excel-Benutzeroberfläche passiert, wirkt sich nicht auf den von der API zurückgegebenen Textwert aus. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="87166-p106">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="87166-155">valueTypes</span><span class="sxs-lookup"><span data-stu-id="87166-155">valueTypes</span></span>|<span data-ttu-id="87166-156">Json</span><span class="sxs-lookup"><span data-stu-id="87166-156">Json</span></span>|<span data-ttu-id="87166-p107">Stellt den Datentyp in jeder Zelle dar. Schreibgeschützt. Die folgenden Werte sind möglich: Unbekannt, leer, Zeichenfolge, Ganzzahl, Doppelwort, Boolesch, Fehler.</span><span class="sxs-lookup"><span data-stu-id="87166-p107">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="87166-160">values</span><span class="sxs-lookup"><span data-stu-id="87166-160">values</span></span>|<span data-ttu-id="87166-161">Json</span><span class="sxs-lookup"><span data-stu-id="87166-161">Json</span></span>|<span data-ttu-id="87166-p108">Stellt die Rohwerte der angegebenen Bereichsansicht dar. Die zurückgegebenen Daten können vom Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zellen, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.</span><span class="sxs-lookup"><span data-stu-id="87166-p108">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="87166-165">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="87166-165">Relationships</span></span>
| <span data-ttu-id="87166-166">Beziehung</span><span class="sxs-lookup"><span data-stu-id="87166-166">Relationship</span></span> | <span data-ttu-id="87166-167">Typ</span><span class="sxs-lookup"><span data-stu-id="87166-167">Type</span></span>   |<span data-ttu-id="87166-168">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87166-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87166-169">Rows</span><span class="sxs-lookup"><span data-stu-id="87166-169">rows</span></span>|<span data-ttu-id="87166-170">[workbookRangeView](workbookrangeview.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="87166-170">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="87166-p109">Stellt eine Sammlung der mit dem Bereich verknüpften Bereichsansichten dar. Schreibgeschützt.    Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="87166-p109">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="87166-174">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="87166-174">JSON representation</span></span>
<span data-ttu-id="87166-175">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="87166-175">Here is a JSON representation of the resource.</span></span>
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
