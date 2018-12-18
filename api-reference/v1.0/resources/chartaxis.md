---
title: ChartAxis-Ressourcentyp
description: Stellt eine einzelne Achse in einem Diagramm dar.
author: lumine2008
ms.openlocfilehash: 39c71e9fa832ffb967a1ef147ccd7e07d6b9aaec
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344366"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="f89b2-103">ChartAxis-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f89b2-103">ChartAxis resource type</span></span>

<span data-ttu-id="f89b2-104">Stellt eine einzelne Achse in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="f89b2-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="f89b2-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="f89b2-105">Methods</span></span>

| <span data-ttu-id="f89b2-106">Methode</span><span class="sxs-lookup"><span data-stu-id="f89b2-106">Method</span></span>           | <span data-ttu-id="f89b2-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f89b2-107">Return Type</span></span>    |<span data-ttu-id="f89b2-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f89b2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f89b2-109">ChartAxis abrufen</span><span class="sxs-lookup"><span data-stu-id="f89b2-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="f89b2-110">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="f89b2-110">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="f89b2-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chartAxis-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f89b2-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="f89b2-112">Update</span><span class="sxs-lookup"><span data-stu-id="f89b2-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="f89b2-113">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="f89b2-113">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="f89b2-114">Dient zum Aktualisieren des ChartAxis-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f89b2-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f89b2-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f89b2-115">Properties</span></span>
| <span data-ttu-id="f89b2-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f89b2-116">Property</span></span>     | <span data-ttu-id="f89b2-117">Typ</span><span class="sxs-lookup"><span data-stu-id="f89b2-117">Type</span></span>   |<span data-ttu-id="f89b2-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f89b2-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f89b2-119">id</span><span class="sxs-lookup"><span data-stu-id="f89b2-119">id</span></span>       |<span data-ttu-id="f89b2-120">string</span><span class="sxs-lookup"><span data-stu-id="f89b2-120">string</span></span>   | <span data-ttu-id="f89b2-121">Eindeutiger Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="f89b2-121">Unique identifier.</span></span> <span data-ttu-id="f89b2-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f89b2-122">Read-only.</span></span>|
|<span data-ttu-id="f89b2-123">majorUnit</span><span class="sxs-lookup"><span data-stu-id="f89b2-123">majorUnit</span></span>|<span data-ttu-id="f89b2-124">Json</span><span class="sxs-lookup"><span data-stu-id="f89b2-124">Json</span></span>|<span data-ttu-id="f89b2-p102">Stellt das Intervall zwischen zwei Hauptteilstrichen dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden.  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="f89b2-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="f89b2-128">maximum</span><span class="sxs-lookup"><span data-stu-id="f89b2-128">maximum</span></span>|<span data-ttu-id="f89b2-129">Json</span><span class="sxs-lookup"><span data-stu-id="f89b2-129">Json</span></span>|<span data-ttu-id="f89b2-p103">Stellt den Maximalwert auf der Größenachse dar.  Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte).  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="f89b2-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="f89b2-133">minimum</span><span class="sxs-lookup"><span data-stu-id="f89b2-133">minimum</span></span>|<span data-ttu-id="f89b2-134">Json</span><span class="sxs-lookup"><span data-stu-id="f89b2-134">Json</span></span>|<span data-ttu-id="f89b2-p104">Stellt den Mindestwert auf der Größenachse dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte).  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="f89b2-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="f89b2-138">minorUnit</span><span class="sxs-lookup"><span data-stu-id="f89b2-138">minorUnit</span></span>|<span data-ttu-id="f89b2-139">Json</span><span class="sxs-lookup"><span data-stu-id="f89b2-139">Json</span></span>|<span data-ttu-id="f89b2-p105">Stellt das Intervall zwischen zwei Hilfsteilstrichen dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte). Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="f89b2-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f89b2-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f89b2-143">Relationships</span></span>
| <span data-ttu-id="f89b2-144">Beziehung</span><span class="sxs-lookup"><span data-stu-id="f89b2-144">Relationship</span></span> | <span data-ttu-id="f89b2-145">Typ</span><span class="sxs-lookup"><span data-stu-id="f89b2-145">Type</span></span>   |<span data-ttu-id="f89b2-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f89b2-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f89b2-147">Format</span><span class="sxs-lookup"><span data-stu-id="f89b2-147">format</span></span>|[<span data-ttu-id="f89b2-148">WorkbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="f89b2-148">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="f89b2-p106">Stellt die Formatierung für ein Diagrammobjekt dar, einschließlich Linien- und Schriftartformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f89b2-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="f89b2-151">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="f89b2-151">majorGridlines</span></span>|[<span data-ttu-id="f89b2-152">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="f89b2-152">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="f89b2-p107">Gibt ein Gitternetzlinien-Objekt zurück, das die Hauptgitternetzlinien für die angegebene Achse darstellt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f89b2-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="f89b2-155">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="f89b2-155">minorGridlines</span></span>|[<span data-ttu-id="f89b2-156">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="f89b2-156">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="f89b2-p108">Gibt ein Gitternetzlinien-Objekt zurück, das die Hilfsgitternetzlinien für die angegebene Achse darstellt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f89b2-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="f89b2-159">title</span><span class="sxs-lookup"><span data-stu-id="f89b2-159">title</span></span>|[<span data-ttu-id="f89b2-160">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="f89b2-160">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="f89b2-p109">Stellt den Achsentitel dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f89b2-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f89b2-163">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f89b2-163">JSON representation</span></span>

<span data-ttu-id="f89b2-164">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f89b2-164">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxis"
}-->

```json
{
  "id": "string",
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string",
   "format": {"@odata.type": "microsoft.graph.workbookChartAxisFormat"},
  "majorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "minorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "title": {"@odata.type": "microsoft.graph.workbookChartAxisTitle"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->