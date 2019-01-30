---
title: Ressourcentyp rangeView
description: RangeView stellt einen Satz von sichtbaren Zellen des übergeordneten Bereichs dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ace424d12e38e4bb907923ea542ebd7330130d06
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643979"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="11ca2-103">Ressourcentyp rangeView</span><span class="sxs-lookup"><span data-stu-id="11ca2-103">rangeView resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11ca2-104">RangeView stellt einen Satz von sichtbaren Zellen des übergeordneten Bereichs dar.</span><span class="sxs-lookup"><span data-stu-id="11ca2-104">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="11ca2-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="11ca2-105">Methods</span></span>

| <span data-ttu-id="11ca2-106">Methode</span><span class="sxs-lookup"><span data-stu-id="11ca2-106">Method</span></span>           | <span data-ttu-id="11ca2-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="11ca2-107">Return Type</span></span>    |<span data-ttu-id="11ca2-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11ca2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="11ca2-109">Zeilen auflisten</span><span class="sxs-lookup"><span data-stu-id="11ca2-109">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="11ca2-110">[workbookRangeView](workbookrangeview.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="11ca2-110">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="11ca2-111">Rufen Sie eine workbookRangeView-Objektsammlung ab.</span><span class="sxs-lookup"><span data-stu-id="11ca2-111">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="11ca2-112">Itemat</span><span class="sxs-lookup"><span data-stu-id="11ca2-112">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="11ca2-113">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="11ca2-113">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="11ca2-114">Rufen Sie ein im Index basiertes RangeView-Element ab.</span><span class="sxs-lookup"><span data-stu-id="11ca2-114">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="11ca2-115">Range</span><span class="sxs-lookup"><span data-stu-id="11ca2-115">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="11ca2-116">workbookRange</span><span class="sxs-lookup"><span data-stu-id="11ca2-116">workbookRange</span></span>](range.md)|<span data-ttu-id="11ca2-117">Rufen Sie das Range-Objekt ab, das mit der Bereichsansicht verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="11ca2-117">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="11ca2-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="11ca2-118">Properties</span></span>
| <span data-ttu-id="11ca2-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="11ca2-119">Property</span></span>     | <span data-ttu-id="11ca2-120">Typ</span><span class="sxs-lookup"><span data-stu-id="11ca2-120">Type</span></span>   |<span data-ttu-id="11ca2-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11ca2-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11ca2-122">columnCount</span><span class="sxs-lookup"><span data-stu-id="11ca2-122">columnCount</span></span>|<span data-ttu-id="11ca2-123">Int32</span><span class="sxs-lookup"><span data-stu-id="11ca2-123">Int32</span></span>|<span data-ttu-id="11ca2-p101">Gibt die Anzahl der sichtbaren Spalten zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="11ca2-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="11ca2-126">formulas</span><span class="sxs-lookup"><span data-stu-id="11ca2-126">formulas</span></span>|<span data-ttu-id="11ca2-127">Json</span><span class="sxs-lookup"><span data-stu-id="11ca2-127">Json</span></span>|<span data-ttu-id="11ca2-128">Stellt die Formel in der A1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="11ca2-128">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="11ca2-129">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="11ca2-129">formulasLocal</span></span>|<span data-ttu-id="11ca2-130">Json</span><span class="sxs-lookup"><span data-stu-id="11ca2-130">Json</span></span>|<span data-ttu-id="11ca2-p102">Stellt die Formel in der A1-Schreibweise, Sprache des Benutzers und im Gebietsschema der Zahlenformatierung dar. Beispielsweise würde die englische Formel "= SUM(A1, 1.5)" in Deutsch "= SUMME(A1; 1,5) " werden.</span><span class="sxs-lookup"><span data-stu-id="11ca2-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="11ca2-133">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="11ca2-133">formulasR1C1</span></span>|<span data-ttu-id="11ca2-134">Json</span><span class="sxs-lookup"><span data-stu-id="11ca2-134">Json</span></span>|<span data-ttu-id="11ca2-135">Stellt die Formel in der R1C1-Schreibweise dar.</span><span class="sxs-lookup"><span data-stu-id="11ca2-135">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="11ca2-136">Index</span><span class="sxs-lookup"><span data-stu-id="11ca2-136">index</span></span>|<span data-ttu-id="11ca2-137">Int32</span><span class="sxs-lookup"><span data-stu-id="11ca2-137">Int32</span></span>|<span data-ttu-id="11ca2-138">Der Index des Bereichs.</span><span class="sxs-lookup"><span data-stu-id="11ca2-138">Index of the range.</span></span>|
|<span data-ttu-id="11ca2-139">numberFormat</span><span class="sxs-lookup"><span data-stu-id="11ca2-139">numberFormat</span></span>|<span data-ttu-id="11ca2-140">Json</span><span class="sxs-lookup"><span data-stu-id="11ca2-140">Json</span></span>|<span data-ttu-id="11ca2-p103">Stellt den Excel-Zahlenformatcode für die angegebene Zelle dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="11ca2-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="11ca2-143">rowCount</span><span class="sxs-lookup"><span data-stu-id="11ca2-143">rowCount</span></span>|<span data-ttu-id="11ca2-144">Int32</span><span class="sxs-lookup"><span data-stu-id="11ca2-144">Int32</span></span>|<span data-ttu-id="11ca2-p104">Gibt die Anzahl der sichtbaren Zeilen zurück. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="11ca2-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="11ca2-147">text</span><span class="sxs-lookup"><span data-stu-id="11ca2-147">text</span></span>|<span data-ttu-id="11ca2-148">Json</span><span class="sxs-lookup"><span data-stu-id="11ca2-148">Json</span></span>|<span data-ttu-id="11ca2-p105">Textwerte des angegebenen Bereichs. Der Textwert hängt nicht von der Zellenbreite ab. Die Ersetzung des #-Zeichens, die in der Excel-Benutzeroberfläche passiert, wirkt sich nicht auf den von der API zurückgegebenen Textwert aus. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="11ca2-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="11ca2-153">valueTypes</span><span class="sxs-lookup"><span data-stu-id="11ca2-153">valueTypes</span></span>|<span data-ttu-id="11ca2-154">Json</span><span class="sxs-lookup"><span data-stu-id="11ca2-154">Json</span></span>|<span data-ttu-id="11ca2-p106">Stellt den Datentyp in jeder Zelle dar. Schreibgeschützt. Die folgenden Werte sind möglich: Unbekannt, leer, Zeichenfolge, Ganzzahl, Doppelwort, Boolesch, Fehler.</span><span class="sxs-lookup"><span data-stu-id="11ca2-p106">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="11ca2-158">values</span><span class="sxs-lookup"><span data-stu-id="11ca2-158">values</span></span>|<span data-ttu-id="11ca2-159">Json</span><span class="sxs-lookup"><span data-stu-id="11ca2-159">Json</span></span>|<span data-ttu-id="11ca2-p107">Stellt die Rohwerte der angegebenen Bereichsansicht dar. Die zurückgegebenen Daten können vom Typ Zeichenfolge, Zahl oder ein boolescher Wert sein. Zellen, die einen Fehler enthalten, geben die Fehlerzeichenfolge zurück.</span><span class="sxs-lookup"><span data-stu-id="11ca2-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="11ca2-163">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="11ca2-163">Relationships</span></span>
| <span data-ttu-id="11ca2-164">Beziehung</span><span class="sxs-lookup"><span data-stu-id="11ca2-164">Relationship</span></span> | <span data-ttu-id="11ca2-165">Typ</span><span class="sxs-lookup"><span data-stu-id="11ca2-165">Type</span></span>   |<span data-ttu-id="11ca2-166">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11ca2-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11ca2-167">Rows</span><span class="sxs-lookup"><span data-stu-id="11ca2-167">rows</span></span>|<span data-ttu-id="11ca2-168">[workbookRangeView](workbookrangeview.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="11ca2-168">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="11ca2-p108">Stellt eine Sammlung der mit dem Bereich verknüpften Bereichsansichten dar. Schreibgeschützt.    Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="11ca2-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11ca2-172">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="11ca2-172">JSON representation</span></span>
<span data-ttu-id="11ca2-173">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="11ca2-173">Here is a JSON representation of the resource.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/workbookrangeview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
