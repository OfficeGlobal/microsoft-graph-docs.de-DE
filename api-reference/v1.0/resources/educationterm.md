# <a name="educationterm-resource-type"></a><span data-ttu-id="3b907-101">educationTerm-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3b907-101">educationTerm resource type</span></span>

<span data-ttu-id="3b907-102">Ein Zeitraum.</span><span class="sxs-lookup"><span data-stu-id="3b907-102">A term.</span></span> <span data-ttu-id="3b907-103">Er stellt einen festgelegten Teil des akademischen Jahres dar.</span><span class="sxs-lookup"><span data-stu-id="3b907-103">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="3b907-104">Er wird in [educationClass](educationclass.md) verwendet.</span><span class="sxs-lookup"><span data-stu-id="3b907-104">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3b907-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3b907-105">Properties</span></span>
| <span data-ttu-id="3b907-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3b907-106">Property</span></span>     | <span data-ttu-id="3b907-107">Typ</span><span class="sxs-lookup"><span data-stu-id="3b907-107">Type</span></span>   |<span data-ttu-id="3b907-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b907-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b907-109">displayName</span><span class="sxs-lookup"><span data-stu-id="3b907-109">displayName</span></span>| <span data-ttu-id="3b907-110">String</span><span class="sxs-lookup"><span data-stu-id="3b907-110">String</span></span>| <span data-ttu-id="3b907-111">Der Anzeigename des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="3b907-111">Display name of the template.</span></span>| 
|<span data-ttu-id="3b907-112">externalId</span><span class="sxs-lookup"><span data-stu-id="3b907-112">externalId</span></span>|<span data-ttu-id="3b907-113">String</span><span class="sxs-lookup"><span data-stu-id="3b907-113">String</span></span>| <span data-ttu-id="3b907-114">Die ID des Zeitraums im Synchronisierungssystem</span><span class="sxs-lookup"><span data-stu-id="3b907-114">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="3b907-115">startDate</span><span class="sxs-lookup"><span data-stu-id="3b907-115">startDate</span></span>|<span data-ttu-id="3b907-116">Date</span><span class="sxs-lookup"><span data-stu-id="3b907-116">Date</span></span>|<span data-ttu-id="3b907-117">Anfang des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="3b907-117">Start of the term.</span></span>|
|<span data-ttu-id="3b907-118">endDate</span><span class="sxs-lookup"><span data-stu-id="3b907-118">endDate</span></span>|<span data-ttu-id="3b907-119">Date</span><span class="sxs-lookup"><span data-stu-id="3b907-119">Date</span></span>|<span data-ttu-id="3b907-120">Ende des Zeitraums</span><span class="sxs-lookup"><span data-stu-id="3b907-120">End of the document.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b907-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3b907-121">JSON representation</span></span>

<span data-ttu-id="3b907-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3b907-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->