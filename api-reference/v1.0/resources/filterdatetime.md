# <a name="filterdatetime-resource-type"></a><span data-ttu-id="9eb7c-101">FilterDatetime-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9eb7c-101">FilterDatetime resource type</span></span>

<span data-ttu-id="9eb7c-102">Stellt dar, wie ein Datum beim Filtern nach Werten gefiltert wird.</span><span class="sxs-lookup"><span data-stu-id="9eb7c-102">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="9eb7c-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9eb7c-103">Properties</span></span>
| <span data-ttu-id="9eb7c-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9eb7c-104">Property</span></span>     | <span data-ttu-id="9eb7c-105">Typ</span><span class="sxs-lookup"><span data-stu-id="9eb7c-105">Type</span></span>   |<span data-ttu-id="9eb7c-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9eb7c-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9eb7c-107">date</span><span class="sxs-lookup"><span data-stu-id="9eb7c-107">date</span></span>|<span data-ttu-id="9eb7c-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eb7c-108">string</span></span>|<span data-ttu-id="9eb7c-109">Das Datum im ISO8601-Format zum Filtern von Daten.</span><span class="sxs-lookup"><span data-stu-id="9eb7c-109">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="9eb7c-110">specificity</span><span class="sxs-lookup"><span data-stu-id="9eb7c-110">specificity</span></span>|<span data-ttu-id="9eb7c-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9eb7c-111">string</span></span>|<span data-ttu-id="9eb7c-112">Wie spezifisch die Daten bestimmt werden sollen, um die Daten zu halten.</span><span class="sxs-lookup"><span data-stu-id="9eb7c-112">How specific the date should be used to keep data.</span></span> <span data-ttu-id="9eb7c-113">Angenommen, das Datum ist der 02.04.2005 und die Spezifität wird auf „Monat“ festgelegt, hält der Filter-Vorgang alle Zeilen mit einem Datum im Monat April 2009.</span><span class="sxs-lookup"><span data-stu-id="9eb7c-113">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: , , , , , .</span></span> <span data-ttu-id="9eb7c-114">Die mögliche Werte sind: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span><span class="sxs-lookup"><span data-stu-id="9eb7c-114">The possible values are `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`, , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="9eb7c-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9eb7c-115">Relationships</span></span>
<span data-ttu-id="9eb7c-116">Keine</span><span class="sxs-lookup"><span data-stu-id="9eb7c-116">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9eb7c-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9eb7c-117">JSON representation</span></span>

<span data-ttu-id="9eb7c-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9eb7c-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->