---
title: ChartPointFormat-Ressourcentyp
description: Stellt das Formatierungsobjekt für Diagrammpunkte dar.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 5923252a9fce47eedc58751def301b6515560ddd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883342"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="7a5bc-103">ChartPointFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7a5bc-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="7a5bc-104">Stellt das Formatierungsobjekt für Diagrammpunkte dar.</span><span class="sxs-lookup"><span data-stu-id="7a5bc-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="7a5bc-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="7a5bc-105">Methods</span></span>
<span data-ttu-id="7a5bc-106">Keine</span><span class="sxs-lookup"><span data-stu-id="7a5bc-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="7a5bc-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7a5bc-107">Properties</span></span>
<span data-ttu-id="7a5bc-108">Keine</span><span class="sxs-lookup"><span data-stu-id="7a5bc-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="7a5bc-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7a5bc-109">Relationships</span></span>
| <span data-ttu-id="7a5bc-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="7a5bc-110">Relationship</span></span> | <span data-ttu-id="7a5bc-111">Typ</span><span class="sxs-lookup"><span data-stu-id="7a5bc-111">Type</span></span>   |<span data-ttu-id="7a5bc-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7a5bc-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a5bc-113">fill</span><span class="sxs-lookup"><span data-stu-id="7a5bc-113">fill</span></span>|[<span data-ttu-id="7a5bc-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="7a5bc-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="7a5bc-p101">Stellt die Füllung eines Diagramms dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="7a5bc-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="7a5bc-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7a5bc-117">JSON representation</span></span>

<span data-ttu-id="7a5bc-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7a5bc-118">Here is a JSON representation of the resource.</span></span>

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
