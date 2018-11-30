---
title: patternedRecurrence-Ressourcentyp
description: Serienmuster und -bereich.
ms.openlocfilehash: 10a90db032cd7461e28bc096fd6213df44f3ea45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017020"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="3f21b-103">patternedRecurrence-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3f21b-103">patternedRecurrence resource type</span></span>

<span data-ttu-id="3f21b-104">Serienmuster und -bereich.</span><span class="sxs-lookup"><span data-stu-id="3f21b-104">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="3f21b-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3f21b-105">Properties</span></span>
| <span data-ttu-id="3f21b-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3f21b-106">Property</span></span>     | <span data-ttu-id="3f21b-107">Typ</span><span class="sxs-lookup"><span data-stu-id="3f21b-107">Type</span></span>   |<span data-ttu-id="3f21b-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3f21b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f21b-109">Muster</span><span class="sxs-lookup"><span data-stu-id="3f21b-109">pattern</span></span>|[<span data-ttu-id="3f21b-110">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="3f21b-110">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="3f21b-111">Die Häufigkeit eines Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="3f21b-111">The frequency of an event.</span></span>|
|<span data-ttu-id="3f21b-112">Bereich</span><span class="sxs-lookup"><span data-stu-id="3f21b-112">range</span></span>|[<span data-ttu-id="3f21b-113">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="3f21b-113">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="3f21b-114">Die Dauer eines Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="3f21b-114">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3f21b-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3f21b-115">JSON representation</span></span>

<span data-ttu-id="3f21b-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3f21b-116">Here is a JSON representation of the resource</span></span>

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
