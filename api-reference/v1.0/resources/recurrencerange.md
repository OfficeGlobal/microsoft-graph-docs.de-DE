# <a name="recurrencerange-resource-type"></a><span data-ttu-id="39756-101">recurrenceRange-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="39756-101">recurrenceRange resource type</span></span>

<span data-ttu-id="39756-102">Die Dauer eines Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="39756-102">The duration of an event.</span></span>

## <a name="properties"></a><span data-ttu-id="39756-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="39756-103">Properties</span></span>

| <span data-ttu-id="39756-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="39756-104">Property</span></span>     | <span data-ttu-id="39756-105">Typ</span><span class="sxs-lookup"><span data-stu-id="39756-105">Type</span></span>   |<span data-ttu-id="39756-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="39756-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39756-107">endDate</span><span class="sxs-lookup"><span data-stu-id="39756-107">endDate</span></span>|<span data-ttu-id="39756-108">Datum</span><span class="sxs-lookup"><span data-stu-id="39756-108">Date</span></span>|<span data-ttu-id="39756-109">Das Enddatum der Serie.</span><span class="sxs-lookup"><span data-stu-id="39756-109">The end date of the series.</span></span>|
|<span data-ttu-id="39756-110">numberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="39756-110">numberOfOccurrences</span></span>|<span data-ttu-id="39756-111">Int32</span><span class="sxs-lookup"><span data-stu-id="39756-111">Int32</span></span>|<span data-ttu-id="39756-112">Wie oft das Ereignis wiederholt werden soll.</span><span class="sxs-lookup"><span data-stu-id="39756-112">How many times to repeat the event.</span></span>|
|<span data-ttu-id="39756-113">recurrenceTimeZone</span><span class="sxs-lookup"><span data-stu-id="39756-113">recurrenceTimeZone</span></span>|<span data-ttu-id="39756-114">String</span><span class="sxs-lookup"><span data-stu-id="39756-114">String</span></span> |<span data-ttu-id="39756-115">Zeitzone für die **startDate**- und **endDate**-Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="39756-115">Time zone for the **startDate** and **endDate** properties.</span></span> |
|<span data-ttu-id="39756-116">startDate</span><span class="sxs-lookup"><span data-stu-id="39756-116">startDate</span></span>|<span data-ttu-id="39756-117">Datum</span><span class="sxs-lookup"><span data-stu-id="39756-117">Date</span></span>|<span data-ttu-id="39756-118">Das Startdatum der Serie.</span><span class="sxs-lookup"><span data-stu-id="39756-118">The start date of the series.</span></span>|
|<span data-ttu-id="39756-119">type</span><span class="sxs-lookup"><span data-stu-id="39756-119">type</span></span>|<span data-ttu-id="39756-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="39756-120">String</span></span>|<span data-ttu-id="39756-p101">Der Serienbereich: EndDate = 0, NoEnd = 1, Numbered = 2. Mögliche Werte: `EndDate`, `NoEnd`, `Numbered`.</span><span class="sxs-lookup"><span data-stu-id="39756-p101">The recurrence range: EndDate = 0, NoEnd = 1, Numbered = 2. Possible values are: `EndDate`, `NoEnd`, `Numbered`.</span></span>||

## <a name="json-representation"></a><span data-ttu-id="39756-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="39756-123">JSON representation</span></span>

<span data-ttu-id="39756-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="39756-124">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencerange"
}-->

```json
{
  "endDate": "String (timestamp)",
  "numberOfOccurrences": 1024,
  "recurrenceTimeZone": "string",
  "startDate": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
