# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="1b0d1-101">daylightTimeZoneOffset-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="1b0d1-101">daylightTimeZoneOffset resource type</span></span>

<span data-ttu-id="1b0d1-102">Gibt an, wann eine Zeitzone von Standardzeit in Sommerzeit wechselt.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-102">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="1b0d1-103">Wenn eine Zeitzone beispielsweise mit den folgenden Eigenschaften angegeben wird:</span><span class="sxs-lookup"><span data-stu-id="1b0d1-103">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="1b0d1-104">**bias** ist 300</span><span class="sxs-lookup"><span data-stu-id="1b0d1-104">**bias** is 300</span></span>
- <span data-ttu-id="1b0d1-105">**daylightBias** ist -100</span><span class="sxs-lookup"><span data-stu-id="1b0d1-105">**daylightBias** is -100</span></span>
- <span data-ttu-id="1b0d1-106">**dayOccurrence** ist 4</span><span class="sxs-lookup"><span data-stu-id="1b0d1-106">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="1b0d1-107">**dayOfWeek** ist „Sonntag“</span><span class="sxs-lookup"><span data-stu-id="1b0d1-107">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="1b0d1-108">**month** ist 5</span><span class="sxs-lookup"><span data-stu-id="1b0d1-108">**month** is 5</span></span>
- <span data-ttu-id="1b0d1-109">**time** ist  02:00:00 _ **year** ist 0. Dies bedeutet, dass die Zeit während der Sommerzeit +300-100=200 Minuten vor der UTC-Zeit liegt.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-109">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="1b0d1-110">Der Übergang von Sommerzeit zu Standardzeit findet jedes Jahr um 2 Uhr am vierten Sonntag im Mai stattfindet.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-110">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="1b0d1-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1b0d1-111">Properties</span></span>
| <span data-ttu-id="1b0d1-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1b0d1-112">Property</span></span>     | <span data-ttu-id="1b0d1-113">Typ</span><span class="sxs-lookup"><span data-stu-id="1b0d1-113">Type</span></span>   |<span data-ttu-id="1b0d1-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b0d1-114">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1b0d1-115">daylightBias</span><span class="sxs-lookup"><span data-stu-id="1b0d1-115">daylightBias</span></span> | <span data-ttu-id="1b0d1-116">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="1b0d1-116">Edm.Int32</span></span> | <span data-ttu-id="1b0d1-117">Der Zeitversatz der Sommerzeit von der Koordinierten Weltzeit (UTC).</span><span class="sxs-lookup"><span data-stu-id="1b0d1-117">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="1b0d1-118">Dieser Wert wird in Minuten angegeben.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-118">This value is in minutes.</span></span>  |
| <span data-ttu-id="1b0d1-119">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="1b0d1-119">dayOccurrence</span></span> | <span data-ttu-id="1b0d1-120">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="1b0d1-120">Edm.Int32</span></span> | <span data-ttu-id="1b0d1-121">Stellt das n-te Vorkommen des Wochentags dar, an dem der Übergang von Standardzeit zu Sommerzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-121">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="1b0d1-122">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="1b0d1-122">dayOfWeek</span></span> | <span data-ttu-id="1b0d1-123">string</span><span class="sxs-lookup"><span data-stu-id="1b0d1-123">string</span></span> | <span data-ttu-id="1b0d1-124">Stellt den Wochentag dar, an dem der Übergang von Standardzeit zu Sommerzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-124">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="1b0d1-125">Monat</span><span class="sxs-lookup"><span data-stu-id="1b0d1-125">month</span></span> | <span data-ttu-id="1b0d1-126">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="1b0d1-126">Edm.Int32</span></span> | <span data-ttu-id="1b0d1-127">Stellt den Monat dar, in dem der Übergang von Standardzeit zu Sommerzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-127">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="1b0d1-128">Uhrzeit</span><span class="sxs-lookup"><span data-stu-id="1b0d1-128">time</span></span> | <span data-ttu-id="1b0d1-129">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="1b0d1-129">Edm.TimeOfDay</span></span> | <span data-ttu-id="1b0d1-130">Stellt die Uhrzeit dar, zu der der Übergang von Standardzeit zu Sommerzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-130">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="1b0d1-131">Jahr</span><span class="sxs-lookup"><span data-stu-id="1b0d1-131">year</span></span> | <span data-ttu-id="1b0d1-132">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="1b0d1-132">Edm.Int32</span></span> | <span data-ttu-id="1b0d1-133">Stellt dar, wie häufig der Wechsel von Standardzeit zu Sommerzeit in einem Jahr erfolgt.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-133">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="1b0d1-134">Der Wert 0 bedeutet z. B. jedes Jahr.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-134">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1b0d1-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1b0d1-135">JSON representation</span></span>

<span data-ttu-id="1b0d1-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1b0d1-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.standardTimeZoneOffset",
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}-->

```json
{
  "daylightBias": "Int32",
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->