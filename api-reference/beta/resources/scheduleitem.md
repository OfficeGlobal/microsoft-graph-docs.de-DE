---
title: von ScheduleItem Ressourcentyp
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: ed6b7441996cdf00b33be03f70afb888cc9bb251
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511352"
---
# <a name="scheduleitem-resource-type"></a><span data-ttu-id="40ba8-104">von ScheduleItem Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="40ba8-104">scheduleItem resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="40ba8-105">Ein Element, das beschreibt die Verfügbarkeit eines Benutzers auf ein Ereignis tatsächliche auf Standardkalender des Benutzers entspricht.</span><span class="sxs-lookup"><span data-stu-id="40ba8-105">An item that describes the availability of a user corresponding to an actual event on the user's default calendar.</span></span> <span data-ttu-id="40ba8-106">Dieses Element gilt für als auch eine Ressource.</span><span class="sxs-lookup"><span data-stu-id="40ba8-106">This item applies to a resource as well.</span></span>

## <a name="properties"></a><span data-ttu-id="40ba8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="40ba8-107">Properties</span></span>
| <span data-ttu-id="40ba8-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="40ba8-108">Property</span></span>     | <span data-ttu-id="40ba8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="40ba8-109">Type</span></span>   |<span data-ttu-id="40ba8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40ba8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40ba8-111">end</span><span class="sxs-lookup"><span data-stu-id="40ba8-111">end</span></span> |[<span data-ttu-id="40ba8-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="40ba8-112">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="40ba8-113">Das Datum, Uhrzeit und Zeitzone, die das zugehörige Ereignis endet.</span><span class="sxs-lookup"><span data-stu-id="40ba8-113">The date, time, and time zone that the corresponding event ends.</span></span> |
|<span data-ttu-id="40ba8-114">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="40ba8-114">isPrivate</span></span> |<span data-ttu-id="40ba8-115">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="40ba8-115">Boolean</span></span> |<span data-ttu-id="40ba8-116">Die Vertraulichkeit des entsprechenden Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="40ba8-116">The sensitivity of the corresponding event.</span></span> <span data-ttu-id="40ba8-117">True, wenn das Ereignis markiert wird `private`false andernfalls.</span><span class="sxs-lookup"><span data-stu-id="40ba8-117">True if the event is marked `private`, false otherwise.</span></span> |
|<span data-ttu-id="40ba8-118">location</span><span class="sxs-lookup"><span data-stu-id="40ba8-118">location</span></span> |<span data-ttu-id="40ba8-119">String</span><span class="sxs-lookup"><span data-stu-id="40ba8-119">String</span></span> | <span data-ttu-id="40ba8-120">Der Speicherort, an dem entsprechenden Ereigniscode gehalten oder teilnahmen aus.</span><span class="sxs-lookup"><span data-stu-id="40ba8-120">The location where the corresponding event is held or attended from.</span></span> <span data-ttu-id="40ba8-121">Optional.</span><span class="sxs-lookup"><span data-stu-id="40ba8-121">Optional.</span></span>|
|<span data-ttu-id="40ba8-122">start</span><span class="sxs-lookup"><span data-stu-id="40ba8-122">start</span></span> |[<span data-ttu-id="40ba8-123">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="40ba8-123">dateTimeTimeZone</span></span>](datetimetimezone.md) |<span data-ttu-id="40ba8-124">Das Datum, Uhrzeit und Zeitzone, die das zugehörige Ereignis beginnt.</span><span class="sxs-lookup"><span data-stu-id="40ba8-124">The date, time, and time zone that the corresponding event starts.</span></span> |
|<span data-ttu-id="40ba8-125">status</span><span class="sxs-lookup"><span data-stu-id="40ba8-125">status</span></span> |<span data-ttu-id="40ba8-126">String</span><span class="sxs-lookup"><span data-stu-id="40ba8-126">String</span></span> | <span data-ttu-id="40ba8-127">Der Verfügbarkeitsstatus des Benutzers oder der Ressource während des entsprechenden Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="40ba8-127">The availability status of the user or resource during the corresponding event.</span></span> <span data-ttu-id="40ba8-128">Die möglichen Werte sind: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="40ba8-128">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span> |
|<span data-ttu-id="40ba8-129">subject</span><span class="sxs-lookup"><span data-stu-id="40ba8-129">subject</span></span> |<span data-ttu-id="40ba8-130">String</span><span class="sxs-lookup"><span data-stu-id="40ba8-130">String</span></span> | <span data-ttu-id="40ba8-131">Die Betreffzeile das entsprechende Ereignis.</span><span class="sxs-lookup"><span data-stu-id="40ba8-131">The corresponding event's subject line.</span></span> <span data-ttu-id="40ba8-132">Optional.</span><span class="sxs-lookup"><span data-stu-id="40ba8-132">Optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="40ba8-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="40ba8-133">JSON representation</span></span>

<span data-ttu-id="40ba8-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="40ba8-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleItem"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "isPrivate": true,
  "location": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "status": "String",
  "subject": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
