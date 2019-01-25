---
title: followupFlag-Ressourcentyp
description: Ermöglicht das Festlegen einer Kennzeichnung für den Benutzer zur späteren Weiterverfolgung. Unterstützte Elemente umfassen message und contact.
localization_priority: Normal
ms.openlocfilehash: f8ae4cdc04b48fe0b6dede437684215cefb75969
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509546"
---
# <a name="followupflag-resource-type"></a><span data-ttu-id="2c9cf-104">followupFlag-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2c9cf-104">followupFlag resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c9cf-105">Ermöglicht das Festlegen einer Kennzeichnung für den Benutzer zur späteren Weiterverfolgung.</span><span class="sxs-lookup"><span data-stu-id="2c9cf-105">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="2c9cf-106">Unterstützte Elemente umfassen [message](message.md) und [contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="2c9cf-106">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2c9cf-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2c9cf-107">Properties</span></span>
| <span data-ttu-id="2c9cf-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2c9cf-108">Property</span></span>     | <span data-ttu-id="2c9cf-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2c9cf-109">Type</span></span>   |<span data-ttu-id="2c9cf-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2c9cf-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c9cf-111">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c9cf-111">completedDateTime</span></span>|[<span data-ttu-id="2c9cf-112">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2c9cf-112">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2c9cf-113">Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beendet wurde.</span><span class="sxs-lookup"><span data-stu-id="2c9cf-113">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="2c9cf-114">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="2c9cf-114">dueDateTime</span></span>|<span data-ttu-id="2c9cf-115">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="2c9cf-115">**dateTimeTimeZone**</span></span>|<span data-ttu-id="2c9cf-116">Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beendet sein muss.</span><span class="sxs-lookup"><span data-stu-id="2c9cf-116">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="2c9cf-117">flagStatus</span><span class="sxs-lookup"><span data-stu-id="2c9cf-117">flagStatus</span></span>|<span data-ttu-id="2c9cf-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2c9cf-118">String</span></span>|<span data-ttu-id="2c9cf-119">Der Status für die Weiterverfolgung eines Elements.</span><span class="sxs-lookup"><span data-stu-id="2c9cf-119">The status for follow-up for an item.</span></span> <span data-ttu-id="2c9cf-120">Mögliche Werte sind: `notFlagged`, `complete` und `flagged`.</span><span class="sxs-lookup"><span data-stu-id="2c9cf-120">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="2c9cf-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2c9cf-121">startDateTime</span></span>|<span data-ttu-id="2c9cf-122">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="2c9cf-122">**dateTimeTimeZone**</span></span>|<span data-ttu-id="2c9cf-123">Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beginnen soll.</span><span class="sxs-lookup"><span data-stu-id="2c9cf-123">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2c9cf-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2c9cf-124">JSON representation</span></span>

<span data-ttu-id="2c9cf-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2c9cf-125">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/followupflag.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
