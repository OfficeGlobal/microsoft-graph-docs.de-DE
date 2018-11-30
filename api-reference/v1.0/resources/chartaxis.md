---
title: ChartAxis-Ressourcentyp
description: Stellt eine einzelne Achse in einem Diagramm dar.
ms.openlocfilehash: fe29c6820f810158ca4accc864c852b0f00d2dda
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017171"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="71b0c-103">ChartAxis-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="71b0c-103">ChartAxis resource type</span></span>

<span data-ttu-id="71b0c-104">Stellt eine einzelne Achse in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="71b0c-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="71b0c-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="71b0c-105">Methods</span></span>

| <span data-ttu-id="71b0c-106">Methode</span><span class="sxs-lookup"><span data-stu-id="71b0c-106">Method</span></span>           | <span data-ttu-id="71b0c-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="71b0c-107">Return Type</span></span>    |<span data-ttu-id="71b0c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71b0c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="71b0c-109">ChartAxis abrufen</span><span class="sxs-lookup"><span data-stu-id="71b0c-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="71b0c-110">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="71b0c-110">WorkbookChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="71b0c-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chartAxis-Objekts.</span><span class="sxs-lookup"><span data-stu-id="71b0c-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="71b0c-112">Update</span><span class="sxs-lookup"><span data-stu-id="71b0c-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="71b0c-113">WorkbookChartAxis</span><span class="sxs-lookup"><span data-stu-id="71b0c-113">WorkbookChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="71b0c-114">Dient zum Aktualisieren des ChartAxis-Objekts.</span><span class="sxs-lookup"><span data-stu-id="71b0c-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="71b0c-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="71b0c-115">Properties</span></span>
| <span data-ttu-id="71b0c-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71b0c-116">Property</span></span>     | <span data-ttu-id="71b0c-117">Typ</span><span class="sxs-lookup"><span data-stu-id="71b0c-117">Type</span></span>   |<span data-ttu-id="71b0c-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71b0c-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="71b0c-119">id</span><span class="sxs-lookup"><span data-stu-id="71b0c-119">id</span></span>       |<span data-ttu-id="71b0c-120">string</span><span class="sxs-lookup"><span data-stu-id="71b0c-120">string</span></span>   | <span data-ttu-id="71b0c-121">Eindeutiger Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="71b0c-121">Unique identifier.</span></span> <span data-ttu-id="71b0c-122">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="71b0c-122">Read-only.</span></span>|
|<span data-ttu-id="71b0c-123">majorUnit</span><span class="sxs-lookup"><span data-stu-id="71b0c-123">majorUnit</span></span>|<span data-ttu-id="71b0c-124">Json</span><span class="sxs-lookup"><span data-stu-id="71b0c-124">Json</span></span>|<span data-ttu-id="71b0c-p102">Stellt das Intervall zwischen zwei Hauptteilstrichen dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden.  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="71b0c-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="71b0c-128">maximum</span><span class="sxs-lookup"><span data-stu-id="71b0c-128">maximum</span></span>|<span data-ttu-id="71b0c-129">Json</span><span class="sxs-lookup"><span data-stu-id="71b0c-129">Json</span></span>|<span data-ttu-id="71b0c-p103">Stellt den Maximalwert auf der Größenachse dar.  Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte).  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="71b0c-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="71b0c-133">minimum</span><span class="sxs-lookup"><span data-stu-id="71b0c-133">minimum</span></span>|<span data-ttu-id="71b0c-134">Json</span><span class="sxs-lookup"><span data-stu-id="71b0c-134">Json</span></span>|<span data-ttu-id="71b0c-p104">Stellt den Mindestwert auf der Größenachse dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte).  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="71b0c-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="71b0c-138">minorUnit</span><span class="sxs-lookup"><span data-stu-id="71b0c-138">minorUnit</span></span>|<span data-ttu-id="71b0c-139">Json</span><span class="sxs-lookup"><span data-stu-id="71b0c-139">Json</span></span>|<span data-ttu-id="71b0c-p105">Stellt das Intervall zwischen zwei Hilfsteilstrichen dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte). Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="71b0c-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71b0c-143">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="71b0c-143">Relationships</span></span>
| <span data-ttu-id="71b0c-144">Beziehung</span><span class="sxs-lookup"><span data-stu-id="71b0c-144">Relationship</span></span> | <span data-ttu-id="71b0c-145">Typ</span><span class="sxs-lookup"><span data-stu-id="71b0c-145">Type</span></span>   |<span data-ttu-id="71b0c-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71b0c-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71b0c-147">Format</span><span class="sxs-lookup"><span data-stu-id="71b0c-147">format</span></span>|[<span data-ttu-id="71b0c-148">WorkbookChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="71b0c-148">WorkbookChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="71b0c-p106">Stellt die Formatierung für ein Diagrammobjekt dar, einschließlich Linien- und Schriftartformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="71b0c-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="71b0c-151">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="71b0c-151">majorGridlines</span></span>|[<span data-ttu-id="71b0c-152">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="71b0c-152">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="71b0c-p107">Gibt ein Gitternetzlinien-Objekt zurück, das die Hauptgitternetzlinien für die angegebene Achse darstellt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="71b0c-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="71b0c-155">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="71b0c-155">minorGridlines</span></span>|[<span data-ttu-id="71b0c-156">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="71b0c-156">WorkbookChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="71b0c-p108">Gibt ein Gitternetzlinien-Objekt zurück, das die Hilfsgitternetzlinien für die angegebene Achse darstellt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="71b0c-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="71b0c-159">title</span><span class="sxs-lookup"><span data-stu-id="71b0c-159">title</span></span>|[<span data-ttu-id="71b0c-160">WorkbookChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="71b0c-160">WorkbookChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="71b0c-p109">Stellt den Achsentitel dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="71b0c-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71b0c-163">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="71b0c-163">JSON representation</span></span>

<span data-ttu-id="71b0c-164">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="71b0c-164">Here is a JSON representation of the resource.</span></span>

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