---
title: ChartPointFormat-Ressourcentyp
description: Stellt das Formatierungsobjekt für Diagrammpunkte dar.
ms.openlocfilehash: f06b31ad030dd587128f35667145f19d5cbd2e7e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018019"
---
# <a name="chartpointformat-resource-type"></a><span data-ttu-id="1a1de-103">ChartPointFormat-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1a1de-103">ChartPointFormat resource type</span></span>

<span data-ttu-id="1a1de-104">Stellt das Formatierungsobjekt für Diagrammpunkte dar.</span><span class="sxs-lookup"><span data-stu-id="1a1de-104">Represents formatting object for chart points.</span></span>


## <a name="methods"></a><span data-ttu-id="1a1de-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="1a1de-105">Methods</span></span>
<span data-ttu-id="1a1de-106">Keine</span><span class="sxs-lookup"><span data-stu-id="1a1de-106">None</span></span>

## <a name="properties"></a><span data-ttu-id="1a1de-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1a1de-107">Properties</span></span>
<span data-ttu-id="1a1de-108">Keine</span><span class="sxs-lookup"><span data-stu-id="1a1de-108">None</span></span>

## <a name="relationships"></a><span data-ttu-id="1a1de-109">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1a1de-109">Relationships</span></span>
| <span data-ttu-id="1a1de-110">Beziehung</span><span class="sxs-lookup"><span data-stu-id="1a1de-110">Relationship</span></span> | <span data-ttu-id="1a1de-111">Typ</span><span class="sxs-lookup"><span data-stu-id="1a1de-111">Type</span></span>   |<span data-ttu-id="1a1de-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1a1de-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a1de-113">fill</span><span class="sxs-lookup"><span data-stu-id="1a1de-113">fill</span></span>|[<span data-ttu-id="1a1de-114">WorkbookChartFill</span><span class="sxs-lookup"><span data-stu-id="1a1de-114">WorkbookChartFill</span></span>](chartfill.md)|<span data-ttu-id="1a1de-p101">Stellt die Füllung eines Diagramms dar, einschließlich Informationen zur Hintergrundformatierung. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="1a1de-p101">Represents the fill format of a chart, which includes background formating information. Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1a1de-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1a1de-117">JSON representation</span></span>

<span data-ttu-id="1a1de-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1a1de-118">Here is a JSON representation of the resource.</span></span>

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