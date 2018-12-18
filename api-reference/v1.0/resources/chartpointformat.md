---
title: ChartPointFormat-Ressourcentyp
description: Stellt das Formatierungsobjekt für Diagrammpunkte dar.
author: lumine2008
ms.openlocfilehash: 94ba58eb60f80cf704de3d8a44e6e96f010429a7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311312"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="a922d-103">ChartPointFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a922d-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="a922d-104">Stellt das Formatierungsobjekt für Diagrammpunkte dar.</span><span class="sxs-lookup"><span data-stu-id="a922d-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="a922d-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="a922d-105">Methods</span></span>
<span data-ttu-id="a922d-106">Keine</span><span class="sxs-lookup"><span data-stu-id="a922d-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="a922d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a922d-107">Properties</span></span>
<span data-ttu-id="a922d-108">Keine</span><span class="sxs-lookup"><span data-stu-id="a922d-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="a922d-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a922d-109">Relationships</span></span>
| <span data-ttu-id="a922d-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="a922d-110">Relationship</span></span> | <span data-ttu-id="a922d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a922d-111">Type</span></span>   |<span data-ttu-id="a922d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a922d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a922d-113">fill</span><span class="sxs-lookup"><span data-stu-id="a922d-113">fill</span></span>|[<span data-ttu-id="a922d-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="a922d-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="a922d-p101">Stellt die Füllung eines Diagramms dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a922d-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="a922d-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a922d-117">JSON representation</span></span>

<span data-ttu-id="a922d-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a922d-118">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartPointFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPointFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->