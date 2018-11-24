# <a name="followupflag-resource-type"></a><span data-ttu-id="0e8e5-101">followupFlag-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0e8e5-101">followupFlag resource type</span></span>


<span data-ttu-id="0e8e5-102">Ermöglicht das Aktivieren von ein Flag in einem Element für den Benutzer zu einem späteren Zeitpunkt zu verfolgen.</span><span class="sxs-lookup"><span data-stu-id="0e8e5-102">Allows setting a flag in an item for the user to follow up on later.</span></span> 

## <a name="properties"></a><span data-ttu-id="0e8e5-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0e8e5-103">Properties</span></span>
| <span data-ttu-id="0e8e5-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0e8e5-104">Property</span></span>     | <span data-ttu-id="0e8e5-105">Typ</span><span class="sxs-lookup"><span data-stu-id="0e8e5-105">Type</span></span>   |<span data-ttu-id="0e8e5-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e8e5-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e8e5-107">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e8e5-107">completedDateTime</span></span>|[<span data-ttu-id="0e8e5-108">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="0e8e5-108">dateTimeTimeZone</span></span>](dateTimeTimeZone.md)|<span data-ttu-id="0e8e5-109">Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beendet wurde.</span><span class="sxs-lookup"><span data-stu-id="0e8e5-109">The date and time that the follow-up was finished.</span></span>|
|<span data-ttu-id="0e8e5-110">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="0e8e5-110">dueDateTime</span></span>|<span data-ttu-id="0e8e5-111">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="0e8e5-111">**dateTimeTimeZone**</span></span>|<span data-ttu-id="0e8e5-112">Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beendet sein muss.</span><span class="sxs-lookup"><span data-stu-id="0e8e5-112">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="0e8e5-113">flagStatus</span><span class="sxs-lookup"><span data-stu-id="0e8e5-113">flagStatus</span></span>|<span data-ttu-id="0e8e5-114">followupFlagStatus</span><span class="sxs-lookup"><span data-stu-id="0e8e5-114">followupFlagStatus</span></span>|<span data-ttu-id="0e8e5-115">Der Status für die Weiterverfolgung eines Elements.</span><span class="sxs-lookup"><span data-stu-id="0e8e5-115">The status for follow-up for an item.</span></span> <span data-ttu-id="0e8e5-116">Mögliche Werte sind: `notFlagged`, `complete` und `flagged`.</span><span class="sxs-lookup"><span data-stu-id="0e8e5-116">Possible values are `notFlagged`, `complete`, and `flagged`.</span></span>|
|<span data-ttu-id="0e8e5-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0e8e5-117">startDateTime</span></span>|<span data-ttu-id="0e8e5-118">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="0e8e5-118">**dateTimeTimeZone**</span></span>|<span data-ttu-id="0e8e5-119">Datum und Uhrzeit, zu dem bzw. der die Weiterverfolgung beginnen soll.</span><span class="sxs-lookup"><span data-stu-id="0e8e5-119">The date and time that the follow-up is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e8e5-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0e8e5-120">JSON representation</span></span>

<span data-ttu-id="0e8e5-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0e8e5-121">Here is a JSON representation of the resource</span></span>

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
