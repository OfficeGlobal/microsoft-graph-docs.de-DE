# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="d220e-101">Ressourcentyp automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="d220e-101">automaticRepliesMailTips resource type</span></span>


<span data-ttu-id="d220e-102">[E-Mail-Infos](../resources/mailtips.md) zu automatischen Antworten, die für ein Postfach eingerichtet wurden.</span><span class="sxs-lookup"><span data-stu-id="d220e-102">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="d220e-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d220e-103">Properties</span></span>
| <span data-ttu-id="d220e-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d220e-104">Property</span></span>     | <span data-ttu-id="d220e-105">Typ</span><span class="sxs-lookup"><span data-stu-id="d220e-105">Type</span></span>   |<span data-ttu-id="d220e-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d220e-106">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="d220e-107">Nachricht</span><span class="sxs-lookup"><span data-stu-id="d220e-107">message</span></span> | <span data-ttu-id="d220e-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d220e-108">String</span></span> | <span data-ttu-id="d220e-109">Die Nachricht der automatischen Antwort.</span><span class="sxs-lookup"><span data-stu-id="d220e-109">The automatic reply message.</span></span> |
| <span data-ttu-id="d220e-110">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="d220e-110">messageLanguage</span></span> | [<span data-ttu-id="d220e-111">localeInfo</span><span class="sxs-lookup"><span data-stu-id="d220e-111">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="d220e-112">Die Sprache der Nachricht der automatischen Antwort.</span><span class="sxs-lookup"><span data-stu-id="d220e-112">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="d220e-113">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="d220e-113">ScheduledEndTime</span></span> | [<span data-ttu-id="d220e-114">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d220e-114">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="d220e-115">Das Datum und die Uhrzeit, für die das Ende der automatischen Antworten festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="d220e-115">The date and time that automatic replies are set to end, if Status is set to .</span></span> |
| <span data-ttu-id="d220e-116">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="d220e-116">ScheduledStartTime</span></span> | [<span data-ttu-id="d220e-117">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="d220e-117">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="d220e-118">Datum und Uhrzeit, für die der Beginn der automatischen Antworten festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="d220e-118">The date and time that automatic replies are set to begin, if Status is set to .</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d220e-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d220e-119">JSON representation</span></span>

<span data-ttu-id="d220e-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d220e-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->