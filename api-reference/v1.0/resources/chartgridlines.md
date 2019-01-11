---
title: ChartGridlines-Ressourcentyp
description: Stellt Haupt-Gitternetzlinien oder Hilfs-Gitternetzlinien auf einer Diagrammachse dar.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: b95bc8c23ea71abb0d2c3f54e218d425e3d188ea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880346"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="26b55-103">ChartGridlines-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="26b55-103">ChartGridlines resource type</span></span>

<span data-ttu-id="26b55-104">Stellt Haupt-Gitternetzlinien oder Hilfs-Gitternetzlinien auf einer Diagrammachse dar.</span><span class="sxs-lookup"><span data-stu-id="26b55-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="26b55-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="26b55-105">Methods</span></span>

| <span data-ttu-id="26b55-106">Methode</span><span class="sxs-lookup"><span data-stu-id="26b55-106">Method</span></span>           | <span data-ttu-id="26b55-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="26b55-107">Return Type</span></span>    |<span data-ttu-id="26b55-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26b55-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="26b55-109">ChartGridlines abrufen</span><span class="sxs-lookup"><span data-stu-id="26b55-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="26b55-110">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="26b55-110">WorkbookChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="26b55-111">Dient zum Lesender Eigenschaften und der Beziehungen des chartGridlines-Objekts.</span><span class="sxs-lookup"><span data-stu-id="26b55-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="26b55-112">Update</span><span class="sxs-lookup"><span data-stu-id="26b55-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="26b55-113">WorkbookChartGridlines</span><span class="sxs-lookup"><span data-stu-id="26b55-113">WorkbookChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="26b55-114">Dient zum Aktualisieren des ChartGridlines-Objekts.</span><span class="sxs-lookup"><span data-stu-id="26b55-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="26b55-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="26b55-115">Properties</span></span>
| <span data-ttu-id="26b55-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="26b55-116">Property</span></span>     | <span data-ttu-id="26b55-117">Typ</span><span class="sxs-lookup"><span data-stu-id="26b55-117">Type</span></span>   |<span data-ttu-id="26b55-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26b55-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26b55-119">visible</span><span class="sxs-lookup"><span data-stu-id="26b55-119">visible</span></span>|<span data-ttu-id="26b55-120">boolean</span><span class="sxs-lookup"><span data-stu-id="26b55-120">boolean</span></span>|<span data-ttu-id="26b55-121">Boolescher Wert, der angibt, ob die Achsengitternetzlinien angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="26b55-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26b55-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="26b55-122">Relationships</span></span>
| <span data-ttu-id="26b55-123">Beziehung</span><span class="sxs-lookup"><span data-stu-id="26b55-123">Relationship</span></span> | <span data-ttu-id="26b55-124">Typ</span><span class="sxs-lookup"><span data-stu-id="26b55-124">Type</span></span>   |<span data-ttu-id="26b55-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26b55-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26b55-126">format</span><span class="sxs-lookup"><span data-stu-id="26b55-126">format</span></span>|[<span data-ttu-id="26b55-127">WorkbookChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="26b55-127">WorkbookChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="26b55-p101">Stellt die Formatierung der Diagrammgitternetzlinien dar. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="26b55-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26b55-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="26b55-130">JSON representation</span></span>

<span data-ttu-id="26b55-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="26b55-131">Here is a JSON representation of the resource.</span></span>

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
