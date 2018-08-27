# <a name="reminder-resource-type"></a><span data-ttu-id="20b1c-101">Ressourcentyp Erinnerung</span><span class="sxs-lookup"><span data-stu-id="20b1c-101">reminder resource type</span></span>

<span data-ttu-id="20b1c-102">Eine Erinnerung für ein [Ereignis](event.md) in einem [Kalender](calendar.md) des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="20b1c-102">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="20b1c-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="20b1c-103">Properties</span></span>
| <span data-ttu-id="20b1c-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="20b1c-104">Property</span></span>     | <span data-ttu-id="20b1c-105">Typ</span><span class="sxs-lookup"><span data-stu-id="20b1c-105">Type</span></span>   |<span data-ttu-id="20b1c-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="20b1c-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20b1c-107">changeKey</span><span class="sxs-lookup"><span data-stu-id="20b1c-107">changeKey</span></span>|<span data-ttu-id="20b1c-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="20b1c-108">String</span></span>|<span data-ttu-id="20b1c-p101">Gibt die Version der Erinnerung an. Jedes Mal, wenn die Erinnerung geändert wird, wird auch **changeKey** geändert. Auf diese Weise kann Exchange Änderungen an der korrekten Version des Objekts vornehmen.</span><span class="sxs-lookup"><span data-stu-id="20b1c-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="20b1c-112">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="20b1c-112">eventEndTime</span></span>|[<span data-ttu-id="20b1c-113">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="20b1c-113">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="20b1c-114">Datum, Uhrzeit und Zeitzone für das Ende des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="20b1c-114">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="20b1c-115">eventId</span><span class="sxs-lookup"><span data-stu-id="20b1c-115">eventId</span></span>|<span data-ttu-id="20b1c-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="20b1c-116">String</span></span>|<span data-ttu-id="20b1c-p102">Die eindeutige ID des Ereignisses. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="20b1c-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="20b1c-119">eventLocation</span><span class="sxs-lookup"><span data-stu-id="20b1c-119">eventLocation</span></span>|[<span data-ttu-id="20b1c-120">Ort</span><span class="sxs-lookup"><span data-stu-id="20b1c-120">Location</span></span>](location.md)|<span data-ttu-id="20b1c-121">Der Speicherort des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="20b1c-121">The location of the event.</span></span>|
|<span data-ttu-id="20b1c-122">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="20b1c-122">eventStartTime</span></span>|[<span data-ttu-id="20b1c-123">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="20b1c-123">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="20b1c-124">Datum, Uhrzeit und Zeitzone für den Beginn des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="20b1c-124">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="20b1c-125">eventSubject</span><span class="sxs-lookup"><span data-stu-id="20b1c-125">eventSubject</span></span>|<span data-ttu-id="20b1c-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="20b1c-126">String</span></span>|<span data-ttu-id="20b1c-127">Der Text der Betreffzeile des Ereignisses.</span><span class="sxs-lookup"><span data-stu-id="20b1c-127">The text of the event's subject line.</span></span>|
|<span data-ttu-id="20b1c-128">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="20b1c-128">eventWebLink</span></span>|<span data-ttu-id="20b1c-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="20b1c-129">String</span></span>|<span data-ttu-id="20b1c-130">Die URL zum Öfnen des Ereignisses in Outlook im Web.</span><span class="sxs-lookup"><span data-stu-id="20b1c-130">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="20b1c-p103">Das Ereignis wird im Browser geöffnet, wenn Sie über Outlook im Web bei Ihrem Postfach angemeldet sind. Sie werden aufgefordert, sich anzumelden, wenn Sie noch nicht beim Browser angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="20b1c-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="20b1c-133">Auf diese URL kann von einem iFrame aus zugegriffen werden.</span><span class="sxs-lookup"><span data-stu-id="20b1c-133">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="20b1c-134">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="20b1c-134">reminderFireTime</span></span>|[<span data-ttu-id="20b1c-135">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="20b1c-135">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="20b1c-136">Datum, Uhrzeit und Zeitzone für das Ausführen der Erinnerung.</span><span class="sxs-lookup"><span data-stu-id="20b1c-136">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20b1c-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="20b1c-137">JSON representation</span></span>

<span data-ttu-id="20b1c-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="20b1c-138">Here is a JSON representation of the resource</span></span>

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