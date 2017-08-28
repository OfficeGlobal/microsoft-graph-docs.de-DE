# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="6df41-101">patternedRecurrence-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6df41-101">patternedRecurrence resource type</span></span>

<span data-ttu-id="6df41-102">Serienmuster und -bereich.</span><span class="sxs-lookup"><span data-stu-id="6df41-102">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="6df41-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6df41-103">Properties</span></span>
| <span data-ttu-id="6df41-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6df41-104">Property</span></span>     | <span data-ttu-id="6df41-105">Typ</span><span class="sxs-lookup"><span data-stu-id="6df41-105">Type</span></span>   |<span data-ttu-id="6df41-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6df41-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6df41-107">Muster</span><span class="sxs-lookup"><span data-stu-id="6df41-107">pattern</span></span>|[<span data-ttu-id="6df41-108">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="6df41-108">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="6df41-109">Die Häufigkeit eines Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="6df41-109">The frequency of an event.</span></span>|
|<span data-ttu-id="6df41-110">Bereich</span><span class="sxs-lookup"><span data-stu-id="6df41-110">range</span></span>|[<span data-ttu-id="6df41-111">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="6df41-111">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="6df41-112">Die Dauer eines Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="6df41-112">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6df41-113">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6df41-113">JSON representation</span></span>

<span data-ttu-id="6df41-114">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6df41-114">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.patternedrecurrence"
}-->

```json
{
  "pattern": {"@odata.type": "microsoft.graph.recurrencePattern"},
  "range": {"@odata.type": "microsoft.graph.recurrenceRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->