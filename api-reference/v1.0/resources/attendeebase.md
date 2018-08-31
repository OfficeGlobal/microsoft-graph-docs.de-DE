# <a name="attendeebase-resource-type"></a><span data-ttu-id="8b8e9-101">Ressourcentyp „attendeeBase“</span><span class="sxs-lookup"><span data-stu-id="8b8e9-101">attendeeBase resource type</span></span>

<span data-ttu-id="8b8e9-102">Der Typ eines Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="8b8e9-102">The type of attendee.</span></span>

<span data-ttu-id="8b8e9-103">Abgeleitet von [recipient](recipient.md).</span><span class="sxs-lookup"><span data-stu-id="8b8e9-103">Derived from [recipient](recipient.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b8e9-104">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8b8e9-104">JSON representation</span></span>

<span data-ttu-id="8b8e9-105">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8b8e9-105">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.recipient",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a><span data-ttu-id="8b8e9-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8b8e9-106">Properties</span></span>
| <span data-ttu-id="8b8e9-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8b8e9-107">Property</span></span>     | <span data-ttu-id="8b8e9-108">Typ</span><span class="sxs-lookup"><span data-stu-id="8b8e9-108">Type</span></span>   |<span data-ttu-id="8b8e9-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b8e9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b8e9-110">type</span><span class="sxs-lookup"><span data-stu-id="8b8e9-110">type</span></span>|<span data-ttu-id="8b8e9-111">attendeeType</span><span class="sxs-lookup"><span data-stu-id="8b8e9-111">AttendeeType</span></span>| <span data-ttu-id="8b8e9-112">Der Typ eines Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="8b8e9-112">The type of attendee.</span></span> <span data-ttu-id="8b8e9-113">Mögliche Werte sind `required`, `optional`,`resource`.</span><span class="sxs-lookup"><span data-stu-id="8b8e9-113">The possible values are `required`, `optional`, `resource`, , , , , , , , , or .</span></span> <span data-ttu-id="8b8e9-114">Hinweis: Wenn der Teilnehmer eine Person ist, berücksichtigt [FindMeetingTimes](../api/user_findmeetingtimes.md) immer, dass die Person vom `Required`-Typ ist.</span><span class="sxs-lookup"><span data-stu-id="8b8e9-114">The type of attendee. Possible values are: , , . Currently if the attendee is a person, [findMeetingTimes](../api/user_findmeetingtimes.md) always considers the person is of the `Required` type.</span></span>|
|<span data-ttu-id="8b8e9-115">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8b8e9-115">emailAddress</span></span>|[<span data-ttu-id="8b8e9-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8b8e9-116">emailAddress</span></span>](emailAddress.md)|<span data-ttu-id="8b8e9-117">Enthält den Namen und die SMTP-Adresse des Teilnehmers.</span><span class="sxs-lookup"><span data-stu-id="8b8e9-117">Includes the name and SMTP address of the attendee.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
