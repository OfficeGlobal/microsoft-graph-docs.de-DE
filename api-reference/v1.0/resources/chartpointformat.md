---
title: ChartPointFormat-Ressourcentyp
description: Stellt das Formatierungsobjekt für Diagrammpunkte dar.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 1c1b0a4a7d9076771da11061723f275079d429cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976996"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="66f66-103">ChartPointFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="66f66-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="66f66-104">Stellt das Formatierungsobjekt für Diagrammpunkte dar.</span><span class="sxs-lookup"><span data-stu-id="66f66-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="66f66-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="66f66-105">Methods</span></span>
<span data-ttu-id="66f66-106">Keine</span><span class="sxs-lookup"><span data-stu-id="66f66-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="66f66-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="66f66-107">Properties</span></span>
<span data-ttu-id="66f66-108">Keine</span><span class="sxs-lookup"><span data-stu-id="66f66-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="66f66-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="66f66-109">Relationships</span></span>
| <span data-ttu-id="66f66-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="66f66-110">Relationship</span></span> | <span data-ttu-id="66f66-111">Typ</span><span class="sxs-lookup"><span data-stu-id="66f66-111">Type</span></span>   |<span data-ttu-id="66f66-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66f66-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66f66-113">fill</span><span class="sxs-lookup"><span data-stu-id="66f66-113">fill</span></span>|[<span data-ttu-id="66f66-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="66f66-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="66f66-p101">Stellt die Füllung eines Diagramms dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="66f66-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="66f66-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="66f66-117">JSON representation</span></span>

<span data-ttu-id="66f66-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="66f66-118">Here is a JSON representation of the resource.</span></span>

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
