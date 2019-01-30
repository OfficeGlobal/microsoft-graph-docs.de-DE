---
title: ChartAxis-Ressourcentyp
description: Stellt eine einzelne Achse in einem Diagramm dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6cb780272887b6a9b637bbec24b68b37db93657e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640931"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="73d3f-103">ChartAxis-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="73d3f-103">ChartAxis resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73d3f-104">Stellt eine einzelne Achse in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="73d3f-104">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="73d3f-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="73d3f-105">Methods</span></span>

| <span data-ttu-id="73d3f-106">Methode</span><span class="sxs-lookup"><span data-stu-id="73d3f-106">Method</span></span>           | <span data-ttu-id="73d3f-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="73d3f-107">Return Type</span></span>    |<span data-ttu-id="73d3f-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73d3f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="73d3f-109">ChartAxis abrufen</span><span class="sxs-lookup"><span data-stu-id="73d3f-109">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="73d3f-110">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="73d3f-110">ChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="73d3f-111">Dient zum Lesen der Eigenschaften und der Beziehungen des chartAxis-Objekts.</span><span class="sxs-lookup"><span data-stu-id="73d3f-111">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="73d3f-112">Update</span><span class="sxs-lookup"><span data-stu-id="73d3f-112">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="73d3f-113">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="73d3f-113">ChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="73d3f-114">Dient zum Aktualisieren des ChartAxis-Objekts.</span><span class="sxs-lookup"><span data-stu-id="73d3f-114">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="73d3f-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="73d3f-115">Properties</span></span>
| <span data-ttu-id="73d3f-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="73d3f-116">Property</span></span>     | <span data-ttu-id="73d3f-117">Typ</span><span class="sxs-lookup"><span data-stu-id="73d3f-117">Type</span></span>   |<span data-ttu-id="73d3f-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73d3f-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73d3f-119">majorUnit</span><span class="sxs-lookup"><span data-stu-id="73d3f-119">majorUnit</span></span>|<span data-ttu-id="73d3f-120">object</span><span class="sxs-lookup"><span data-stu-id="73d3f-120">object</span></span>|<span data-ttu-id="73d3f-p101">Stellt das Intervall zwischen zwei Hauptteilstrichen dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden.  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="73d3f-p101">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="73d3f-124">maximum</span><span class="sxs-lookup"><span data-stu-id="73d3f-124">maximum</span></span>|<span data-ttu-id="73d3f-125">object</span><span class="sxs-lookup"><span data-stu-id="73d3f-125">object</span></span>|<span data-ttu-id="73d3f-p102">Stellt den Maximalwert auf der Größenachse dar.  Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte).  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="73d3f-p102">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="73d3f-129">minimum</span><span class="sxs-lookup"><span data-stu-id="73d3f-129">minimum</span></span>|<span data-ttu-id="73d3f-130">object</span><span class="sxs-lookup"><span data-stu-id="73d3f-130">object</span></span>|<span data-ttu-id="73d3f-p103">Stellt den Mindestwert auf der Größenachse dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte).  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="73d3f-p103">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="73d3f-134">minorUnit</span><span class="sxs-lookup"><span data-stu-id="73d3f-134">minorUnit</span></span>|<span data-ttu-id="73d3f-135">object</span><span class="sxs-lookup"><span data-stu-id="73d3f-135">object</span></span>|<span data-ttu-id="73d3f-p104">Stellt das Intervall zwischen zwei Hilfsteilstrichen dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte). Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="73d3f-p104">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73d3f-139">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="73d3f-139">Relationships</span></span>
| <span data-ttu-id="73d3f-140">Beziehung</span><span class="sxs-lookup"><span data-stu-id="73d3f-140">Relationship</span></span> | <span data-ttu-id="73d3f-141">Typ</span><span class="sxs-lookup"><span data-stu-id="73d3f-141">Type</span></span>   |<span data-ttu-id="73d3f-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73d3f-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73d3f-143">format</span><span class="sxs-lookup"><span data-stu-id="73d3f-143">format</span></span>|[<span data-ttu-id="73d3f-144">ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="73d3f-144">ChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="73d3f-p105">Stellt die Formatierung für ein Diagrammobjekt dar, einschließlich Linien- und Schriftartformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="73d3f-p105">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="73d3f-147">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="73d3f-147">majorGridlines</span></span>|[<span data-ttu-id="73d3f-148">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="73d3f-148">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="73d3f-p106">Gibt ein Gitternetzlinien-Objekt zurück, das die Hauptgitternetzlinien für die angegebene Achse darstellt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="73d3f-p106">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="73d3f-151">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="73d3f-151">minorGridlines</span></span>|[<span data-ttu-id="73d3f-152">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="73d3f-152">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="73d3f-p107">Gibt ein Gitternetzlinien-Objekt zurück, das die Hilfsgitternetzlinien für die angegebene Achse darstellt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="73d3f-p107">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="73d3f-155">title</span><span class="sxs-lookup"><span data-stu-id="73d3f-155">title</span></span>|[<span data-ttu-id="73d3f-156">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="73d3f-156">ChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="73d3f-p108">Stellt den Achsentitel dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="73d3f-p108">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73d3f-159">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="73d3f-159">JSON representation</span></span>

<span data-ttu-id="73d3f-160">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="73d3f-160">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartaxis"
}-->

```json
{
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxis.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
