---
title: patternedRecurrence-Ressourcentyp
description: Serienmuster und -bereich.
localization_priority: Normal
ms.openlocfilehash: 8a9581150e3b7790f32268eb34f35b22abcb3642
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840796"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="766bb-103">patternedRecurrence-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="766bb-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="766bb-104">Serienmuster und -bereich.</span><span class="sxs-lookup"><span data-stu-id="766bb-104">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="766bb-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="766bb-105">Properties</span></span>
| <span data-ttu-id="766bb-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="766bb-106">Property</span></span>     | <span data-ttu-id="766bb-107">Typ</span><span class="sxs-lookup"><span data-stu-id="766bb-107">Type</span></span>   |<span data-ttu-id="766bb-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="766bb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="766bb-109">Muster</span><span class="sxs-lookup"><span data-stu-id="766bb-109">pattern</span></span>|[<span data-ttu-id="766bb-110">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="766bb-110">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="766bb-111">Die Häufigkeit eines Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="766bb-111">The frequency of an event.</span></span>|
|<span data-ttu-id="766bb-112">Bereich</span><span class="sxs-lookup"><span data-stu-id="766bb-112">range</span></span>|[<span data-ttu-id="766bb-113">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="766bb-113">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="766bb-114">Die Dauer eines Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="766bb-114">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="766bb-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="766bb-115">JSON representation</span></span>

<span data-ttu-id="766bb-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="766bb-116">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.patternedRecurrence"
}-->

```json
{
  "pattern": {"@odata.type": "microsoft.graph.recurrencePattern"},
  "range": {"@odata.type": "microsoft.graph.recurrenceRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
