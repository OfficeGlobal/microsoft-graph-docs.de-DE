# <a name="reminder-resource-type"></a><span data-ttu-id="9393e-101">reminder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9393e-101">reminder resource type</span></span>



## <a name="properties"></a><span data-ttu-id="9393e-102">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9393e-102">Properties</span></span>
| <span data-ttu-id="9393e-103">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9393e-103">Property</span></span>     | <span data-ttu-id="9393e-104">Typ</span><span class="sxs-lookup"><span data-stu-id="9393e-104">Type</span></span>   |<span data-ttu-id="9393e-105">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9393e-105">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9393e-106">changeKey</span><span class="sxs-lookup"><span data-stu-id="9393e-106">changeKey</span></span>|<span data-ttu-id="9393e-107">String</span><span class="sxs-lookup"><span data-stu-id="9393e-107">String</span></span>|<span data-ttu-id="9393e-p101">Gibt die Version der Erinnerung an. Jedes Mal, wenn die Erinnerung geändert wird, wird auch **changeKey** geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen.</span><span class="sxs-lookup"><span data-stu-id="9393e-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="9393e-111">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="9393e-111">eventEndTime</span></span>|[<span data-ttu-id="9393e-112">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9393e-112">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9393e-113">Datum, Uhrzeit und Zeitzone für das Ende des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="9393e-113">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="9393e-114">eventId</span><span class="sxs-lookup"><span data-stu-id="9393e-114">eventId</span></span>|<span data-ttu-id="9393e-115">String</span><span class="sxs-lookup"><span data-stu-id="9393e-115">String</span></span>|<span data-ttu-id="9393e-p102">Die eindeutige ID des Ereignisses. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9393e-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="9393e-118">eventLocation</span><span class="sxs-lookup"><span data-stu-id="9393e-118">eventLocation</span></span>|[<span data-ttu-id="9393e-119">Location</span><span class="sxs-lookup"><span data-stu-id="9393e-119">Location</span></span>](location.md)|<span data-ttu-id="9393e-120">Der Speicherort des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="9393e-120">The location of the event.</span></span>|
|<span data-ttu-id="9393e-121">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="9393e-121">eventStartTime</span></span>|[<span data-ttu-id="9393e-122">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9393e-122">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9393e-123">Datum, Uhrzeit und Zeitzone für den Beginn des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="9393e-123">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="9393e-124">eventSubject</span><span class="sxs-lookup"><span data-stu-id="9393e-124">eventSubject</span></span>|<span data-ttu-id="9393e-125">String</span><span class="sxs-lookup"><span data-stu-id="9393e-125">String</span></span>|<span data-ttu-id="9393e-126">Der Text der Betreffzeile des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="9393e-126">The text of the event's subject line.</span></span>|
|<span data-ttu-id="9393e-127">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="9393e-127">eventWebLink</span></span>|<span data-ttu-id="9393e-128">String</span><span class="sxs-lookup"><span data-stu-id="9393e-128">String</span></span>|<span data-ttu-id="9393e-129">Die URL zum Öfnen des Ereignisses in Outlook im Web.</span><span class="sxs-lookup"><span data-stu-id="9393e-129">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="9393e-p103">Das Ereignis wird im Browser geöffnet, wenn Sie über Outlook im Web bei Ihrem Postfach angemeldet sind. Sie werden aufgefordert, sich anzumelden, wenn Sie noch nicht beim Browser angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="9393e-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="9393e-132">Auf diese URL kann von einem iFrame aus zugegriffen werden.</span><span class="sxs-lookup"><span data-stu-id="9393e-132">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="9393e-133">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="9393e-133">reminderFireTime</span></span>|[<span data-ttu-id="9393e-134">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9393e-134">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9393e-135">Datum, Uhrzeit und Zeitzone für das Ausführen der Erinnerung.</span><span class="sxs-lookup"><span data-stu-id="9393e-135">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9393e-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9393e-136">JSON representation</span></span>

<span data-ttu-id="9393e-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9393e-137">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reminder"
}-->

```json
{
  "changeKey": "string",
  "eventEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventId": "string",
  "eventLocation": {"@odata.type": "microsoft.graph.location"},
  "eventStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventSubject": "string",
  "eventWebLink": "string",
  "reminderFireTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->