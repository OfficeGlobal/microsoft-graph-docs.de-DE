---
title: patternedRecurrence-Ressourcentyp
description: Serienmuster und -bereich.
ms.openlocfilehash: 205c563d8b4cecc0a817dd1893a6c4f002eb4e06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065989"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="6ec48-103">patternedRecurrence-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6ec48-103">patternedRecurrence resource type</span></span>

> <span data-ttu-id="6ec48-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6ec48-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ec48-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6ec48-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ec48-106">Serienmuster und -bereich.</span><span class="sxs-lookup"><span data-stu-id="6ec48-106">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="6ec48-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6ec48-107">Properties</span></span>
| <span data-ttu-id="6ec48-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6ec48-108">Property</span></span>     | <span data-ttu-id="6ec48-109">Typ</span><span class="sxs-lookup"><span data-stu-id="6ec48-109">Type</span></span>   |<span data-ttu-id="6ec48-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ec48-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ec48-111">Muster</span><span class="sxs-lookup"><span data-stu-id="6ec48-111">pattern</span></span>|[<span data-ttu-id="6ec48-112">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="6ec48-112">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="6ec48-113">Die Häufigkeit eines Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="6ec48-113">The frequency of an event.</span></span>|
|<span data-ttu-id="6ec48-114">Bereich</span><span class="sxs-lookup"><span data-stu-id="6ec48-114">range</span></span>|[<span data-ttu-id="6ec48-115">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="6ec48-115">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="6ec48-116">Die Dauer eines Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="6ec48-116">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6ec48-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6ec48-117">JSON representation</span></span>

<span data-ttu-id="6ec48-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ec48-118">Here is a JSON representation of the resource</span></span>

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
