# <a name="attendee-resource-type"></a><span data-ttu-id="b7f17-101">attendee-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b7f17-101">attendee resource type</span></span>

<span data-ttu-id="b7f17-102">Ein Teilnehmer eines Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="b7f17-102">An event attendee.</span></span>

<span data-ttu-id="b7f17-103">Abgeleitet von [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="b7f17-103">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b7f17-104">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b7f17-104">Properties</span></span>
| <span data-ttu-id="b7f17-105">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b7f17-105">Property</span></span>     | <span data-ttu-id="b7f17-106">Typ</span><span class="sxs-lookup"><span data-stu-id="b7f17-106">Type</span></span>   |<span data-ttu-id="b7f17-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b7f17-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7f17-108">status</span><span class="sxs-lookup"><span data-stu-id="b7f17-108">status</span></span>|[<span data-ttu-id="b7f17-109">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="b7f17-109">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="b7f17-110">Die Antwort des Teilnehmers (keine, akzeptiert, abgelehnt, usw.) für das Ereignis und das Datum und die Uhrzeit, an dem/der die Antwort gesendet wurde.</span><span class="sxs-lookup"><span data-stu-id="b7f17-110">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="b7f17-111">Typ</span><span class="sxs-lookup"><span data-stu-id="b7f17-111">type</span></span>|<span data-ttu-id="b7f17-112">String</span><span class="sxs-lookup"><span data-stu-id="b7f17-112">String</span></span>|<span data-ttu-id="b7f17-113">Der Teilnehmertyp: `Required`, `Optional`, `Resource`.</span><span class="sxs-lookup"><span data-stu-id="b7f17-113">The attendee type: `Required`, `Optional`, `Resource`.</span></span>|
|<span data-ttu-id="b7f17-114">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b7f17-114">emailAddress</span></span>|[<span data-ttu-id="b7f17-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b7f17-115">emailAddress</span></span>](emailAddress.md)|<span data-ttu-id="b7f17-116">Enthält den Namen und die SMTP-Adresse des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="b7f17-116">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7f17-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b7f17-117">JSON representation</span></span>

<span data-ttu-id="b7f17-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b7f17-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->