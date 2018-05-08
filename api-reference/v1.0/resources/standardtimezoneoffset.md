# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="d0b3a-101">standardTimeZoneOffset-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d0b3a-101">standardTimeZoneOffset resource type</span></span>

<span data-ttu-id="d0b3a-102">Gibt an, wann eine Zeitzone von Sommerzeit in Standardzeit wechselt.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-102">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="d0b3a-103">Wenn eine Zeitzone beispielsweise mit den folgenden Eigenschaften angegeben wird:</span><span class="sxs-lookup"><span data-stu-id="d0b3a-103">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="d0b3a-104">**dayOccurrence** ist 3</span><span class="sxs-lookup"><span data-stu-id="d0b3a-104">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="d0b3a-105">**dayOfWeek** ist „Sonntag“</span><span class="sxs-lookup"><span data-stu-id="d0b3a-105">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="d0b3a-106">**month** ist 10</span><span class="sxs-lookup"><span data-stu-id="d0b3a-106">**month** is 10</span></span>
- <span data-ttu-id="d0b3a-107">**time** 02:00:00 _ ist **year** ist 0. Dies bedeutet, dass der Übergang von Sommerzeit zu Standardzeit jedes Jahr um 2 Uhr am dritten Sonntag im Oktober stattfindet.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-107">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="d0b3a-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d0b3a-108">Properties</span></span>
| <span data-ttu-id="d0b3a-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d0b3a-109">Property</span></span>     | <span data-ttu-id="d0b3a-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d0b3a-110">Type</span></span>   |<span data-ttu-id="d0b3a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0b3a-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d0b3a-112">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="d0b3a-112">dayOccurrence</span></span> | <span data-ttu-id="d0b3a-113">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="d0b3a-113">Edm.Int32</span></span> | <span data-ttu-id="d0b3a-114">Stellt das n-te Vorkommen des Wochentags dar, an dem der Übergang von Sommerzeit zu Standardzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-114">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="d0b3a-115">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="d0b3a-115">DAYOFWEEK</span></span> | <span data-ttu-id="d0b3a-116">string</span><span class="sxs-lookup"><span data-stu-id="d0b3a-116">string</span></span> | <span data-ttu-id="d0b3a-117">Stellt den Wochentag dar, an dem der Übergang von Sommerzeit zu Standardzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-117">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="d0b3a-118">month</span><span class="sxs-lookup"><span data-stu-id="d0b3a-118">month</span></span> | <span data-ttu-id="d0b3a-119">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="d0b3a-119">Edm.Int32</span></span> | <span data-ttu-id="d0b3a-120">Stellt den Monat dar, an dem der Übergang von Sommerzeit zu Standardzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-120">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="d0b3a-121">time</span><span class="sxs-lookup"><span data-stu-id="d0b3a-121">time</span></span> | <span data-ttu-id="d0b3a-122">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d0b3a-122">Edm.TimeOfDay</span></span> | <span data-ttu-id="d0b3a-123">Stellt die Uhrzeit dar, zu der der Übergang von Sommerzeit zu Standardzeit erfolgt.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-123">Represents the time of day when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="d0b3a-124">year</span><span class="sxs-lookup"><span data-stu-id="d0b3a-124">year</span></span> | <span data-ttu-id="d0b3a-125">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="d0b3a-125">Edm.Int32</span></span> | <span data-ttu-id="d0b3a-126">Stellt dar, wie häufig der Wechsel von Sommerzeit zu Standardzeit in einem Jahr erfolgt.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-126">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="d0b3a-127">Der Wert 0 bedeutet z. B. jedes Jahr.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-127">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d0b3a-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d0b3a-128">JSON representation</span></span>

<span data-ttu-id="d0b3a-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.standardTimeZoneOffset"
}-->

```json
{
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
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->