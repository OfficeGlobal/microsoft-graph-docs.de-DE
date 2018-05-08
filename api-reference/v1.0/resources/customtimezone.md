# <a name="customtimezone-resource-type"></a><span data-ttu-id="3ad16-101">customTimeZone-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3ad16-101">customTimeZone resource type</span></span>

<span data-ttu-id="3ad16-102">Stellt eine Zeitzone dar, in der der Übergang von Standardzeit zu Sommerzeit oder umgekehrt nicht Standard ist.</span><span class="sxs-lookup"><span data-stu-id="3ad16-102">Represents a time zone where the transition from standard to daylight saving time, or vice versa is not standard.</span></span>


## <a name="properties"></a><span data-ttu-id="3ad16-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3ad16-103">Properties</span></span>
| <span data-ttu-id="3ad16-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3ad16-104">Property</span></span>     | <span data-ttu-id="3ad16-105">Typ</span><span class="sxs-lookup"><span data-stu-id="3ad16-105">Type</span></span>   |<span data-ttu-id="3ad16-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ad16-106">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3ad16-107">bias</span><span class="sxs-lookup"><span data-stu-id="3ad16-107">Bias</span></span> | <span data-ttu-id="3ad16-108">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="3ad16-108">Edm.Int32</span></span> | <span data-ttu-id="3ad16-109">Der Zeitversatz der Zeitzone von der Koordinierten Weltzeit (UTC).</span><span class="sxs-lookup"><span data-stu-id="3ad16-109">The time offset of the time zone from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="3ad16-110">Dieser Wert wird in Minuten angegeben.</span><span class="sxs-lookup"><span data-stu-id="3ad16-110">This value is in points.</span></span> <span data-ttu-id="3ad16-111">Zeitzonen, die der UTC voraus sind, haben einen positiven Versatz; Zeitzonen, die hinter der UTC liegen, haben einen negativen Versatz.</span><span class="sxs-lookup"><span data-stu-id="3ad16-111">Time zones that are ahead of UTC have a positive offset; time zones that are behind UTC have a negative offset.</span></span>|
| <span data-ttu-id="3ad16-112">daylightOffset</span><span class="sxs-lookup"><span data-stu-id="3ad16-112">daylightOffset</span></span> | [<span data-ttu-id="3ad16-113">daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="3ad16-113">daylightTimeZoneOffset</span></span>](daylighttimezoneoffset.md) | <span data-ttu-id="3ad16-114">Gibt an, wann die Zeitzone von Standardzeit in Sommerzeit wechselt.</span><span class="sxs-lookup"><span data-stu-id="3ad16-114">Specifies when the time zone switches from standard time to daylight saving time.</span></span> |
| <span data-ttu-id="3ad16-115">name</span><span class="sxs-lookup"><span data-stu-id="3ad16-115">name</span></span> | <span data-ttu-id="3ad16-116">string</span><span class="sxs-lookup"><span data-stu-id="3ad16-116">string</span></span> | <span data-ttu-id="3ad16-117">Der Name der benutzerdefinierten Zeitzone.</span><span class="sxs-lookup"><span data-stu-id="3ad16-117">The name of the custom time zone.</span></span> |
| <span data-ttu-id="3ad16-118">standardOffset</span><span class="sxs-lookup"><span data-stu-id="3ad16-118">standardOffset</span></span> | [<span data-ttu-id="3ad16-119">standardTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="3ad16-119">standardTimeZoneOffset</span></span>](standardtimezoneoffset.md) | <span data-ttu-id="3ad16-120">Gibt an, wann die Zeitzone von Sommerzeit in Standardzeit wechselt.</span><span class="sxs-lookup"><span data-stu-id="3ad16-120">Specifies when the time zone switches from daylight saving time to standard time.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="3ad16-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3ad16-121">JSON representation</span></span>

<span data-ttu-id="3ad16-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3ad16-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.customTimeZone"
}-->

```json
{
  "bias": "Int32",
  "daylightOffset": {"@odata.type": "microsoft.graph.daylightTimeZoneOffset"},
  "name": "string",
  "standardOffset": {"@odata.type": "microsoft.graph.standardTimeZoneOffset"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->