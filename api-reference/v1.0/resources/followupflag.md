# <a name="followupflag-resource-type"></a><span data-ttu-id="6a0dc-101">followupFlag-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6a0dc-101">followupFlag resource type</span></span>


<span data-ttu-id="6a0dc-102">Ermöglicht das Festlegen einer Kennzeichnung für den Benutzer zur späteren Weiterverfolgung.</span><span class="sxs-lookup"><span data-stu-id="6a0dc-102">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="6a0dc-103">Unterstützte Elemente umfassen [message](message.md) und [contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="6a0dc-103">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6a0dc-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6a0dc-104">Properties</span></span>
| <span data-ttu-id="6a0dc-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6a0dc-105">Property</span></span>     | <span data-ttu-id="6a0dc-106">Typ</span><span class="sxs-lookup"><span data-stu-id="6a0dc-106">Type</span></span>   |<span data-ttu-id="6a0dc-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a0dc-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a0dc-108">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a0dc-108">completedDateTime</span></span>|[<span data-ttu-id="6a0dc-109">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="6a0dc-109">dateTimeTimeZone</span></span>](dateTimeTimeZone.md)|<span data-ttu-id="6a0dc-110">Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beendet wurde.</span><span class="sxs-lookup"><span data-stu-id="6a0dc-110">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="6a0dc-111">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="6a0dc-111">dueDateTime</span></span>|<span data-ttu-id="6a0dc-112">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="6a0dc-112">**dateTimeTimeZone**</span></span>|<span data-ttu-id="6a0dc-113">Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beendet sein muss.</span><span class="sxs-lookup"><span data-stu-id="6a0dc-113">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="6a0dc-114">flagStatus</span><span class="sxs-lookup"><span data-stu-id="6a0dc-114">flagStatus</span></span>|<span data-ttu-id="6a0dc-115">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="6a0dc-115">FollowupFlagStatus</span></span>|<span data-ttu-id="6a0dc-116">Der Status für die Weiterverfolgung eines Elements.</span><span class="sxs-lookup"><span data-stu-id="6a0dc-116">The status for follow-up for an item.</span></span> <span data-ttu-id="6a0dc-117">Mögliche Werte sind: `notFlagged`, `complete` und `flagged`.</span><span class="sxs-lookup"><span data-stu-id="6a0dc-117">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="6a0dc-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6a0dc-118">startDateTime</span></span>|<span data-ttu-id="6a0dc-119">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="6a0dc-119">**dateTimeTimeZone**</span></span>|<span data-ttu-id="6a0dc-120">Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beginnen soll.</span><span class="sxs-lookup"><span data-stu-id="6a0dc-120">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a0dc-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6a0dc-121">JSON representation</span></span>

<span data-ttu-id="6a0dc-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6a0dc-122">Here is a JSON representation of the resource</span></span>

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
