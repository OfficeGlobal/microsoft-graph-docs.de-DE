# <a name="timeconstraint-resource-type"></a><span data-ttu-id="00030-101">Ressourcentyp „timeConstraint“</span><span class="sxs-lookup"><span data-stu-id="00030-101">timeConstraint resource type</span></span>

<span data-ttu-id="00030-102">Schränkt Vorschläge für Besprechungstermine entsprechend der angegebenen Art der Aktivität und der offenen Zeitfenster auf bestimmte Stunden und Tage der Woche ein.</span><span class="sxs-lookup"><span data-stu-id="00030-102">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="00030-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="00030-103">JSON representation</span></span>

<span data-ttu-id="00030-104">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="00030-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeConstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="00030-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="00030-105">Properties</span></span>
| <span data-ttu-id="00030-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="00030-106">Property</span></span>     | <span data-ttu-id="00030-107">Typ</span><span class="sxs-lookup"><span data-stu-id="00030-107">Type</span></span>   |<span data-ttu-id="00030-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00030-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00030-109">activityDomain</span><span class="sxs-lookup"><span data-stu-id="00030-109">activityDomain</span></span>|<span data-ttu-id="00030-110">activityDomain</span><span class="sxs-lookup"><span data-stu-id="00030-110">activityDomain</span></span>|<span data-ttu-id="00030-111">Die Art der Aktivität, optional.</span><span class="sxs-lookup"><span data-stu-id="00030-111">The nature of the activity, optional. Possible values are: , , , or .</span></span> <span data-ttu-id="00030-112">Die möglichen Werte sind: `work`, `personal`, `unrestricted` oder `unknown`.</span><span class="sxs-lookup"><span data-stu-id="00030-112">The possible values are  `work`,  `personal`,  `unrestricted`, or  `unknown`.</span></span>|
|<span data-ttu-id="00030-113">timeslots</span><span class="sxs-lookup"><span data-stu-id="00030-113">timeslots</span></span>|<span data-ttu-id="00030-114">[timeSlot](timeslot.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="00030-114">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="00030-115">Ein Array von Zeitfenstern.</span><span class="sxs-lookup"><span data-stu-id="00030-115">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
