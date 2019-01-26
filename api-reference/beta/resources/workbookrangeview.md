---
title: Ressourcentyp rangeView
description: RangeView stellt einen Satz von sichtbaren Zellen des übergeordneten Bereichs dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d01ab0b8b21814a363d838b61fca29aa90357156
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574362"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="abc7f-103">Ressourcentyp rangeView</span><span class="sxs-lookup"><span data-stu-id="abc7f-103">rangeView resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abc7f-104">RangeView stellt einen Satz von sichtbaren Zellen des übergeordneten Bereichs dar.</span><span class="sxs-lookup"><span data-stu-id="abc7f-104">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="abc7f-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="abc7f-105">Methods</span></span>

| <span data-ttu-id="abc7f-106">Methode</span><span class="sxs-lookup"><span data-stu-id="abc7f-106">Method</span></span>           | <span data-ttu-id="abc7f-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="abc7f-107">Return Type</span></span>    |<span data-ttu-id="abc7f-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="abc7f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="abc7f-109">Zeilen auflisten</span><span class="sxs-lookup"><span data-stu-id="abc7f-109">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="abc7f-110">[workbookRangeView](workbookrangeview.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="abc7f-110">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="abc7f-111">Rufen Sie eine workbookRangeView-Objektsammlung ab.</span><span class="sxs-lookup"><span data-stu-id="abc7f-111">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="abc7f-112">Itemat</span><span class="sxs-lookup"><span data-stu-id="abc7f-112">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="abc7f-113">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="abc7f-113">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="abc7f-114">Rufen Sie ein im Index basiertes RangeView-Element ab.</span><span class="sxs-lookup"><span data-stu-id="abc7f-114">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="abc7f-115">Range</span><span class="sxs-lookup"><span data-stu-id="abc7f-115">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="abc7f-116">workbookRange</span><span class="sxs-lookup"><span data-stu-id="abc7f-116">workbookRange</span></span>](range.md)|<span data-ttu-id="abc7f-117">Rufen Sie das Range-Objekt ab, das mit der Bereichsansicht verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="abc7f-117">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="abc7f-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="abc7f-118">Properties</span></span>
| <span data-ttu-id="abc7f-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="abc7f-119">Property</span></span>     | <span data-ttu-id="abc7f-120">Typ</span><span class="sxs-lookup"><span data-stu-id="abc7f-120">Type</span></span>   |<span data-ttu-id="abc7f-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="abc7f-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abc7f-122">cellAddresses</span><span class="sxs-lookup"><span data-stu-id="abc7f-122">cellAddresses</span></span>|<span data-ttu-id="abc7f-123">Json</span><span class="sxs-lookup"><span data-stu-id="abc7f-123">Json</span></span>|<span data-ttu-id="abc7f-124">Stellt die Zelle Adressen</span><span class="sxs-lookup"><span data-stu-id="abc7f-124">Represents the cell addresses</span></span>
|<span data-ttu-id="abc7f-125">columnCount</span><span class="sxs-lookup"><span data-stu-id="abc7f-125">columnCount</span></span>|<span data-ttu-id="abc7f-126">Int32</span><span class="sxs-lookup"><span data-stu-id="abc7f-126">Int32</span></span>|<span data-ttu-id="abc7f-p101">Gibt die Anzahl der sichtbaren Spalten zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="abc7f-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="abc7f-129">formulas</span><span class="sxs-lookup"><span data-stu-id="abc7f-129">formulas</span></span>|<span data-ttu-id="abc7f-130">Json</span><span class="sxs-lookup"><span data-stu-id="abc7f-130">Json</span></span>|<span data-ttu-id="abc7f-131">Stellt die Formel in der A1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="abc7f-131">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="abc7f-132">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="abc7f-132">formulasLocal</span></span>|<span data-ttu-id="abc7f-133">Json</span><span class="sxs-lookup"><span data-stu-id="abc7f-133">Json</span></span>|<span data-ttu-id="abc7f-p102">Stellt die Formel in der A1-Schreibweise, Sprache des Benutzers und im Gebietsschema der Zahlenformatierung dar. Beispielsweise würde die englische Formel "= SUM(A1, 1.5)" in Deutsch "= SUMME(A1; 1,5) " werden.</span><span class="sxs-lookup"><span data-stu-id="abc7f-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="abc7f-136">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="abc7f-136">formulasR1C1</span></span>|<span data-ttu-id="abc7f-137">Json</span><span class="sxs-lookup"><span data-stu-id="abc7f-137">Json</span></span>|<span data-ttu-id="abc7f-138">Stellt die Formel in der R1C1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="abc7f-138">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="abc7f-139">Index</span><span class="sxs-lookup"><span data-stu-id="abc7f-139">index</span></span>|<span data-ttu-id="abc7f-140">Int32</span><span class="sxs-lookup"><span data-stu-id="abc7f-140">Int32</span></span>|<span data-ttu-id="abc7f-141">Der Index des Bereichs.</span><span class="sxs-lookup"><span data-stu-id="abc7f-141">Index of the range.</span></span>|
|<span data-ttu-id="abc7f-142">numberFormat</span><span class="sxs-lookup"><span data-stu-id="abc7f-142">numberFormat</span></span>|<span data-ttu-id="abc7f-143">Json</span><span class="sxs-lookup"><span data-stu-id="abc7f-143">Json</span></span>|<span data-ttu-id="abc7f-p103">Stellt den Excel-Zahlenformatcode für die angegebene Zelle dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="abc7f-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="abc7f-146">rowCount</span><span class="sxs-lookup"><span data-stu-id="abc7f-146">rowCount</span></span>|<span data-ttu-id="abc7f-147">Int32</span><span class="sxs-lookup"><span data-stu-id="abc7f-147">Int32</span></span>|<span data-ttu-id="abc7f-p104">Gibt die Anzahl der sichtbaren Zeilen zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="abc7f-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="abc7f-150">text</span><span class="sxs-lookup"><span data-stu-id="abc7f-150">text</span></span>|<span data-ttu-id="abc7f-151">Json</span><span class="sxs-lookup"><span data-stu-id="abc7f-151">Json</span></span>|<span data-ttu-id="abc7f-p105">Textwerte des angegebenen Bereichs. Der Textwert hängt nicht von der Zellenbreite ab. Die Ersetzung des #-Zeichens, die in der Excel-Benutzeroberfläche passiert, wirkt sich nicht auf den von der API zurückgegebenen Textwert aus. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="abc7f-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="abc7f-156">valueTypes</span><span class="sxs-lookup"><span data-stu-id="abc7f-156">valueTypes</span></span>|<span data-ttu-id="abc7f-157">Json</span><span class="sxs-lookup"><span data-stu-id="abc7f-157">Json</span></span>|<span data-ttu-id="abc7f-158">Stellt den Typ der Daten, die jeder Zelle an.</span><span class="sxs-lookup"><span data-stu-id="abc7f-158">Represents the type of data of each cell.</span></span> <span data-ttu-id="abc7f-159">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="abc7f-159">Read-only.</span></span> <span data-ttu-id="abc7f-160">Die möglichen Werte sind: unbekannt, leer, String, Integer, Double, Boolean, Fehler.</span><span class="sxs-lookup"><span data-stu-id="abc7f-160">The possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="abc7f-161">values</span><span class="sxs-lookup"><span data-stu-id="abc7f-161">values</span></span>|<span data-ttu-id="abc7f-162">Json</span><span class="sxs-lookup"><span data-stu-id="abc7f-162">Json</span></span>|<span data-ttu-id="abc7f-p107">Stellt die Rohwerte der angegebenen Bereichsansicht dar. Die zurückgegebenen Daten können vom Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zellen, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.</span><span class="sxs-lookup"><span data-stu-id="abc7f-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="abc7f-166">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="abc7f-166">Relationships</span></span>
| <span data-ttu-id="abc7f-167">Beziehung</span><span class="sxs-lookup"><span data-stu-id="abc7f-167">Relationship</span></span> | <span data-ttu-id="abc7f-168">Typ</span><span class="sxs-lookup"><span data-stu-id="abc7f-168">Type</span></span>   |<span data-ttu-id="abc7f-169">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="abc7f-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abc7f-170">Rows</span><span class="sxs-lookup"><span data-stu-id="abc7f-170">rows</span></span>|<span data-ttu-id="abc7f-171">[workbookRangeView](workbookrangeview.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="abc7f-171">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="abc7f-p108">Stellt eine Sammlung der mit dem Bereich verknüpften Bereichsansichten dar. Schreibgeschützt.    Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="abc7f-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="abc7f-175">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="abc7f-175">JSON representation</span></span>
<span data-ttu-id="abc7f-176">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="abc7f-176">Here is a JSON representation of the resource.</span></span>
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
  "id": "String (identifier)",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/workbookrangeview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
