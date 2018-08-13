# <a name="attendee-resource-type"></a><span data-ttu-id="ce1a6-101">attendee-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ce1a6-101">attendee resource type</span></span>

<span data-ttu-id="ce1a6-102">Ein Teilnehmer eines Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="ce1a6-102">An event attendee.</span></span> <span data-ttu-id="ce1a6-103">Dies kann eine Person oder eine Ressource sein, wie z. B. Besprechungsräume oder Geräte, die als Ressource auf dem Exchange-Server für den Mandanten eingerichtet wurden.</span><span class="sxs-lookup"><span data-stu-id="ce1a6-103">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="ce1a6-104">Abgeleitet von [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="ce1a6-104">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ce1a6-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ce1a6-105">Properties</span></span>
| <span data-ttu-id="ce1a6-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ce1a6-106">Property</span></span>     | <span data-ttu-id="ce1a6-107">Typ</span><span class="sxs-lookup"><span data-stu-id="ce1a6-107">Type</span></span>   |<span data-ttu-id="ce1a6-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce1a6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce1a6-109">status</span><span class="sxs-lookup"><span data-stu-id="ce1a6-109">status</span></span>|[<span data-ttu-id="ce1a6-110">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="ce1a6-110">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="ce1a6-111">Die Antwort des Teilnehmers (keine, akzeptiert, abgelehnt, usw.) für das Ereignis und das Datum und die Uhrzeit, an dem/der die Antwort gesendet wurde.</span><span class="sxs-lookup"><span data-stu-id="ce1a6-111">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="ce1a6-112">Typ</span><span class="sxs-lookup"><span data-stu-id="ce1a6-112">type</span></span>|<span data-ttu-id="ce1a6-113">String</span><span class="sxs-lookup"><span data-stu-id="ce1a6-113">String</span></span>|<span data-ttu-id="ce1a6-114">Der Teilnehmertyp: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="ce1a6-114">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="ce1a6-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ce1a6-115">emailAddress</span></span>|[<span data-ttu-id="ce1a6-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ce1a6-116">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="ce1a6-117">Enthält den Namen und die SMTP-Adresse des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="ce1a6-117">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ce1a6-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ce1a6-118">JSON representation</span></span>

<span data-ttu-id="ce1a6-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ce1a6-119">Here is a JSON representation of the resource</span></span>

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