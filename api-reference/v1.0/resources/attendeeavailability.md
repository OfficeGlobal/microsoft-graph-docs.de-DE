# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="c22b7-101">Ressourcentyp „attendeeAvailability“</span><span class="sxs-lookup"><span data-stu-id="c22b7-101">attendeeAvailability resource type</span></span>

<span data-ttu-id="c22b7-102">Typ und Verfügbarkeit eines Teilnehmers</span><span class="sxs-lookup"><span data-stu-id="c22b7-102">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c22b7-103">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c22b7-103">JSON representation</span></span>

<span data-ttu-id="c22b7-104">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c22b7-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="c22b7-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c22b7-105">Properties</span></span>
| <span data-ttu-id="c22b7-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c22b7-106">Property</span></span>     | <span data-ttu-id="c22b7-107">Typ</span><span class="sxs-lookup"><span data-stu-id="c22b7-107">Type</span></span>   |<span data-ttu-id="c22b7-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c22b7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c22b7-109">Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="c22b7-109">attendee</span></span>|[<span data-ttu-id="c22b7-110">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="c22b7-110">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="c22b7-111">Der Typ des Teilnehmers. Unterschieden wird zwischen Personen und Ressourcen. Bei Personen wird zusätzlich differenziert zwischen erforderlichen und optionalen Teilnehmern.</span><span class="sxs-lookup"><span data-stu-id="c22b7-111">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="c22b7-112">Verfügbarkeit</span><span class="sxs-lookup"><span data-stu-id="c22b7-112">availability</span></span>|<span data-ttu-id="c22b7-113">FreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="c22b7-113">FreeBusyStatus</span></span>| <span data-ttu-id="c22b7-114">Der Verfügbarkeitsstatus des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="c22b7-114">The availability status of the attendee. Possible values are: , , , , , .</span></span> <span data-ttu-id="c22b7-115">Mögliche Werte: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c22b7-115">The possible values are `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`, , , , , , or .</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
