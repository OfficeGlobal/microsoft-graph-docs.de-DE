---
title: followupFlag-Ressourcentyp
description: Ermöglicht das Festlegen einer Kennzeichnung für den Benutzer zur späteren Weiterverfolgung. Unterstützte Elemente umfassen message und contact.
localization_priority: Normal
ms.openlocfilehash: aa056d141bfac82b9f039ed705f6de49893783fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869378"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="bb8c1-104">followupFlag-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bb8c1-104">followupFlag resource type</span></span>

> <span data-ttu-id="bb8c1-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bb8c1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb8c1-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bb8c1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bb8c1-107">Ermöglicht das Festlegen einer Kennzeichnung für den Benutzer zur späteren Weiterverfolgung.</span><span class="sxs-lookup"><span data-stu-id="bb8c1-107">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="bb8c1-108">Unterstützte Elemente umfassen [message](message.md) und [contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="bb8c1-108">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bb8c1-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bb8c1-109">Properties</span></span>
| <span data-ttu-id="bb8c1-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bb8c1-110">Property</span></span>     | <span data-ttu-id="bb8c1-111">Typ</span><span class="sxs-lookup"><span data-stu-id="bb8c1-111">Type</span></span>   |<span data-ttu-id="bb8c1-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb8c1-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb8c1-113">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb8c1-113">completedDateTime</span></span>|[<span data-ttu-id="bb8c1-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="bb8c1-114">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="bb8c1-115">Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beendet wurde.</span><span class="sxs-lookup"><span data-stu-id="bb8c1-115">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="bb8c1-116">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="bb8c1-116">dueDateTime</span></span>|<span data-ttu-id="bb8c1-117">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="bb8c1-117">**dateTimeTimeZone**</span></span>|<span data-ttu-id="bb8c1-118">Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beendet sein muss.</span><span class="sxs-lookup"><span data-stu-id="bb8c1-118">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="bb8c1-119">flagStatus</span><span class="sxs-lookup"><span data-stu-id="bb8c1-119">flagStatus</span></span>|<span data-ttu-id="bb8c1-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb8c1-120">String</span></span>|<span data-ttu-id="bb8c1-121">Der Status für die Weiterverfolgung eines Elements.</span><span class="sxs-lookup"><span data-stu-id="bb8c1-121">The status for follow-up for an item.</span></span> <span data-ttu-id="bb8c1-122">Mögliche Werte sind: `notFlagged`, `complete` und `flagged`.</span><span class="sxs-lookup"><span data-stu-id="bb8c1-122">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="bb8c1-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bb8c1-123">startDateTime</span></span>|<span data-ttu-id="bb8c1-124">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="bb8c1-124">**dateTimeTimeZone**</span></span>|<span data-ttu-id="bb8c1-125">Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beginnen soll.</span><span class="sxs-lookup"><span data-stu-id="bb8c1-125">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb8c1-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bb8c1-126">JSON representation</span></span>

<span data-ttu-id="bb8c1-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bb8c1-127">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
