---
title: followupFlag-Ressourcentyp
description: 'Ermöglicht das Aktivieren von ein Flag in einem Element für den Benutzer zu einem späteren Zeitpunkt zu verfolgen. '
ms.openlocfilehash: 5aa9d82fc90d7142717ac5ef05f9d837bac371ba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019573"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="524fb-103">followupFlag-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="524fb-103">followupFlag resource type</span></span>


<span data-ttu-id="524fb-104">Ermöglicht das Aktivieren von ein Flag in einem Element für den Benutzer zu einem späteren Zeitpunkt zu verfolgen.</span><span class="sxs-lookup"><span data-stu-id="524fb-104">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="524fb-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="524fb-105">Properties</span></span>
| <span data-ttu-id="524fb-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="524fb-106">Property</span></span>     | <span data-ttu-id="524fb-107">Typ</span><span class="sxs-lookup"><span data-stu-id="524fb-107">Type</span></span>   |<span data-ttu-id="524fb-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="524fb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="524fb-109">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="524fb-109">completedDateTime</span></span>|[<span data-ttu-id="524fb-110">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="524fb-110">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="524fb-111">Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beendet wurde.</span><span class="sxs-lookup"><span data-stu-id="524fb-111">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="524fb-112">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="524fb-112">dueDateTime</span></span>|<span data-ttu-id="524fb-113">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="524fb-113">**dateTimeTimeZone**</span></span>|<span data-ttu-id="524fb-114">Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beendet sein muss.</span><span class="sxs-lookup"><span data-stu-id="524fb-114">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="524fb-115">flagStatus</span><span class="sxs-lookup"><span data-stu-id="524fb-115">flagStatus</span></span>|<span data-ttu-id="524fb-116">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="524fb-116">followupFlagStatus</span></span>|<span data-ttu-id="524fb-117">Der Status für die Weiterverfolgung eines Elements.</span><span class="sxs-lookup"><span data-stu-id="524fb-117">The status for follow-up for an item.</span></span> <span data-ttu-id="524fb-118">Mögliche Werte sind: `notFlagged`, `complete` und `flagged`.</span><span class="sxs-lookup"><span data-stu-id="524fb-118">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="524fb-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="524fb-119">startDateTime</span></span>|<span data-ttu-id="524fb-120">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="524fb-120">**dateTimeTimeZone**</span></span>|<span data-ttu-id="524fb-121">Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beginnen soll.</span><span class="sxs-lookup"><span data-stu-id="524fb-121">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="524fb-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="524fb-122">JSON representation</span></span>

<span data-ttu-id="524fb-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="524fb-123">Here is a JSON representation of the resource</span></span>

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
