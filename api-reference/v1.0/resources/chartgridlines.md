---
title: ChartGridlines-Ressourcentyp
description: Stellt Haupt-Gitternetzlinien oder Hilfs-Gitternetzlinien auf einer Diagrammachse dar.
author: lumine2008
ms.openlocfilehash: 2aaf044b09d061af4853e76e0f2ba118bd1b2321
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353032"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="0aa35-103">ChartGridlines-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0aa35-103">ChartGridlines resource type</span></span>

<span data-ttu-id="0aa35-104">Stellt Haupt-Gitternetzlinien oder Hilfs-Gitternetzlinien auf einer Diagrammachse dar.</span><span class="sxs-lookup"><span data-stu-id="0aa35-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="0aa35-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="0aa35-105">Methods</span></span>

| <span data-ttu-id="0aa35-106">Methode</span><span class="sxs-lookup"><span data-stu-id="0aa35-106">Method</span></span>           | <span data-ttu-id="0aa35-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0aa35-107">Return Type</span></span>    |<span data-ttu-id="0aa35-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0aa35-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0aa35-109">ChartGridlines abrufen</span><span class="sxs-lookup"><span data-stu-id="0aa35-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="0aa35-110">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="0aa35-110">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="0aa35-111">Dient zum Lesender Eigenschaften und der Beziehungen des chartGridlines-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0aa35-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="0aa35-112">Update</span><span class="sxs-lookup"><span data-stu-id="0aa35-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="0aa35-113">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="0aa35-113">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="0aa35-114">Dient zum Aktualisieren des ChartGridlines-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0aa35-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0aa35-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0aa35-115">Properties</span></span>
| <span data-ttu-id="0aa35-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0aa35-116">Property</span></span>     | <span data-ttu-id="0aa35-117">Typ</span><span class="sxs-lookup"><span data-stu-id="0aa35-117">Type</span></span>   |<span data-ttu-id="0aa35-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0aa35-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0aa35-119">visible</span><span class="sxs-lookup"><span data-stu-id="0aa35-119">visible</span></span>|<span data-ttu-id="0aa35-120">boolean</span><span class="sxs-lookup"><span data-stu-id="0aa35-120">boolean</span></span>|<span data-ttu-id="0aa35-121">Boolescher Wert, der angibt, ob die Achsengitternetzlinien angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="0aa35-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0aa35-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0aa35-122">Relationships</span></span>
| <span data-ttu-id="0aa35-123">Beziehung</span><span class="sxs-lookup"><span data-stu-id="0aa35-123">Relationship</span></span> | <span data-ttu-id="0aa35-124">Typ</span><span class="sxs-lookup"><span data-stu-id="0aa35-124">Type</span></span>   |<span data-ttu-id="0aa35-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0aa35-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0aa35-126">Format</span><span class="sxs-lookup"><span data-stu-id="0aa35-126">format</span></span>|[<span data-ttu-id="0aa35-127">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="0aa35-127">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="0aa35-p101">Stellt die Formatierung der Diagrammgitternetzlinien dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="0aa35-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0aa35-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0aa35-130">JSON representation</span></span>

<span data-ttu-id="0aa35-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0aa35-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartGridlines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->