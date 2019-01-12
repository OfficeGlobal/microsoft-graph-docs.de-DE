---
title: ChartAxis-Ressourcentyp
description: Stellt eine einzelne Achse in einem Diagramm dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c6344f2bbb102e2e2402dba267538cb46d4c0fbe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914192"
---
# <a name="chartaxis-resource-type"></a><span data-ttu-id="f4c0d-103">ChartAxis-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f4c0d-103">ChartAxis resource type</span></span>

> <span data-ttu-id="f4c0d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f4c0d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4c0d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f4c0d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f4c0d-106">Stellt eine einzelne Achse in einem Diagramm dar.</span><span class="sxs-lookup"><span data-stu-id="f4c0d-106">Represents a single axis in a chart.</span></span>


## <a name="methods"></a><span data-ttu-id="f4c0d-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="f4c0d-107">Methods</span></span>

| <span data-ttu-id="f4c0d-108">Methode</span><span class="sxs-lookup"><span data-stu-id="f4c0d-108">Method</span></span>           | <span data-ttu-id="f4c0d-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f4c0d-109">Return Type</span></span>    |<span data-ttu-id="f4c0d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4c0d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f4c0d-111">ChartAxis abrufen</span><span class="sxs-lookup"><span data-stu-id="f4c0d-111">Get ChartAxis</span></span>](../api/chartaxis-get.md) | [<span data-ttu-id="f4c0d-112">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="f4c0d-112">ChartAxis</span></span>](chartaxis.md) |<span data-ttu-id="f4c0d-113">Dient zum Lesen der Eigenschaften und der Beziehungen des chartAxis-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f4c0d-113">Read properties and relationships of chartAxis object.</span></span>|
|[<span data-ttu-id="f4c0d-114">Update</span><span class="sxs-lookup"><span data-stu-id="f4c0d-114">Update</span></span>](../api/chartaxis-update.md) | [<span data-ttu-id="f4c0d-115">ChartAxis</span><span class="sxs-lookup"><span data-stu-id="f4c0d-115">ChartAxis</span></span>](chartaxis.md)   |<span data-ttu-id="f4c0d-116">Dient zum Aktualisieren des ChartAxis-Objekts.</span><span class="sxs-lookup"><span data-stu-id="f4c0d-116">Update ChartAxis object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f4c0d-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f4c0d-117">Properties</span></span>
| <span data-ttu-id="f4c0d-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f4c0d-118">Property</span></span>     | <span data-ttu-id="f4c0d-119">Typ</span><span class="sxs-lookup"><span data-stu-id="f4c0d-119">Type</span></span>   |<span data-ttu-id="f4c0d-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4c0d-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4c0d-121">majorUnit</span><span class="sxs-lookup"><span data-stu-id="f4c0d-121">majorUnit</span></span>|<span data-ttu-id="f4c0d-122">object</span><span class="sxs-lookup"><span data-stu-id="f4c0d-122">object</span></span>|<span data-ttu-id="f4c0d-p102">Stellt das Intervall zwischen zwei Hauptteilstrichen dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden.  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="f4c0d-p102">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="f4c0d-126">maximum</span><span class="sxs-lookup"><span data-stu-id="f4c0d-126">maximum</span></span>|<span data-ttu-id="f4c0d-127">object</span><span class="sxs-lookup"><span data-stu-id="f4c0d-127">object</span></span>|<span data-ttu-id="f4c0d-p103">Stellt den Maximalwert auf der Größenachse dar.  Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte).  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="f4c0d-p103">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="f4c0d-131">minimum</span><span class="sxs-lookup"><span data-stu-id="f4c0d-131">minimum</span></span>|<span data-ttu-id="f4c0d-132">object</span><span class="sxs-lookup"><span data-stu-id="f4c0d-132">object</span></span>|<span data-ttu-id="f4c0d-p104">Stellt den Mindestwert auf der Größenachse dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte).  Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="f4c0d-p104">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="f4c0d-136">minorUnit</span><span class="sxs-lookup"><span data-stu-id="f4c0d-136">minorUnit</span></span>|<span data-ttu-id="f4c0d-137">object</span><span class="sxs-lookup"><span data-stu-id="f4c0d-137">object</span></span>|<span data-ttu-id="f4c0d-p105">Stellt das Intervall zwischen zwei Hilfsteilstrichen dar. Kann auf einen numerischen Wert oder eine leere Zeichenfolge festgelegt werden (für automatische Achsenwerte). Der zurückgegebene Wert ist immer eine Zahl.</span><span class="sxs-lookup"><span data-stu-id="f4c0d-p105">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4c0d-141">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f4c0d-141">Relationships</span></span>
| <span data-ttu-id="f4c0d-142">Beziehung</span><span class="sxs-lookup"><span data-stu-id="f4c0d-142">Relationship</span></span> | <span data-ttu-id="f4c0d-143">Typ</span><span class="sxs-lookup"><span data-stu-id="f4c0d-143">Type</span></span>   |<span data-ttu-id="f4c0d-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f4c0d-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4c0d-145">format</span><span class="sxs-lookup"><span data-stu-id="f4c0d-145">format</span></span>|[<span data-ttu-id="f4c0d-146">ChartAxisFormat</span><span class="sxs-lookup"><span data-stu-id="f4c0d-146">ChartAxisFormat</span></span>](chartaxisformat.md)|<span data-ttu-id="f4c0d-p106">Stellt die Formatierung für ein Diagrammobjekt dar, einschließlich Linien- und Schriftartformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f4c0d-p106">Represents the formatting of a chart object, which includes line and font formatting. Read-only.</span></span>|
|<span data-ttu-id="f4c0d-149">majorGridlines</span><span class="sxs-lookup"><span data-stu-id="f4c0d-149">majorGridlines</span></span>|[<span data-ttu-id="f4c0d-150">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="f4c0d-150">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="f4c0d-p107">Gibt ein Gitternetzlinien-Objekt zurück, das die Hauptgitternetzlinien für die angegebene Achse darstellt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f4c0d-p107">Returns a gridlines object that represents the major gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="f4c0d-153">minorGridlines</span><span class="sxs-lookup"><span data-stu-id="f4c0d-153">minorGridlines</span></span>|[<span data-ttu-id="f4c0d-154">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="f4c0d-154">ChartGridlines</span></span>](chartgridlines.md)|<span data-ttu-id="f4c0d-p108">Gibt ein Gitternetzlinien-Objekt zurück, das die Hilfsgitternetzlinien für die angegebene Achse darstellt. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f4c0d-p108">Returns a Gridlines object that represents the minor gridlines for the specified axis. Read-only.</span></span>|
|<span data-ttu-id="f4c0d-157">title</span><span class="sxs-lookup"><span data-stu-id="f4c0d-157">title</span></span>|[<span data-ttu-id="f4c0d-158">ChartAxisTitle</span><span class="sxs-lookup"><span data-stu-id="f4c0d-158">ChartAxisTitle</span></span>](chartaxistitle.md)|<span data-ttu-id="f4c0d-p109">Stellt den Achsentitel dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="f4c0d-p109">Represents the axis title. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4c0d-161">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f4c0d-161">JSON representation</span></span>

<span data-ttu-id="f4c0d-162">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f4c0d-162">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
