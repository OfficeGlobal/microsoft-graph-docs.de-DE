# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a><span data-ttu-id="97278-101">Abrufen von Outlook-Ereignissen in einem freigegebenen oder delegierten Kalender</span><span class="sxs-lookup"><span data-stu-id="97278-101">Get Outlook events in a shared or delegated calendar</span></span>

<span data-ttu-id="97278-102">Kunden können in Outlook einen Kalender für andere Benutzer freigeben und diese Benutzer dadurch berechtigen, Ereignisse in diesem Kalender abzurufen oder zu ändern.</span><span class="sxs-lookup"><span data-stu-id="97278-102">In Outlook, customers can share a calendar with other users and let them view or modify events in that calendar.</span></span> <span data-ttu-id="97278-103">Kunden können auch die Berechtigung delegieren, an ihrer statt Besprechungsanfragen zu empfangen oder auf diese zu antworten oder Änderungen im Kalender vorzunehmen.</span><span class="sxs-lookup"><span data-stu-id="97278-103">Customers can also grant a delegate to act on their  behalf, to receive or respond to meeting requests, or create or change items in the calendar.</span></span>

<span data-ttu-id="97278-104">Calendar Microsoft Graph unterstützt programmgesteuert das Abrufen von Ereignissen in Kalendern, die von anderen Benutzern freigegeben wurden, sowie Zugriff auf die freigegebenen Kalender.</span><span class="sxs-lookup"><span data-stu-id="97278-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="97278-105">Die Unterstützung gilt auch für Kalender, die delegiert wurden.</span><span class="sxs-lookup"><span data-stu-id="97278-105">The support also applies to calendars that have been delegated.</span></span>

<span data-ttu-id="97278-106">Zum Beispiel hat Garth seinen Standardkalender für John freigegeben und John Lesezugriff gewährt.</span><span class="sxs-lookup"><span data-stu-id="97278-106">As an example, Garth has shared with John his default calendar and given John read access.</span></span> <span data-ttu-id="97278-107">Wenn John sich in Ihrer App angemeldet und delegierte Berechtigungen (Calendars.Read.Shared or Calendars.ReadWrite.Shared) bereitgestellt hat, kann Ihre App auf Garths Kalender sowie auf Ereignisse in diesem Kalender zugreifen, wie nachstehend beschrieben.</span><span class="sxs-lookup"><span data-stu-id="97278-107">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-an-event-in-the-shared-calendar"></a><span data-ttu-id="97278-108">Abrufen eines Ereignisses in dem freigegebenen Kalender</span><span class="sxs-lookup"><span data-stu-id="97278-108">Get an event in the shared calendar</span></span>

<span data-ttu-id="97278-109">Sie können ein bestimmtes Ereignis in Garths freigegebenem Kalender abrufen:</span><span class="sxs-lookup"><span data-stu-id="97278-109">You can get a specific event in Garth's shared default calendar:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

<span data-ttu-id="97278-110">Bei erfolgreichem Abschluss erhalten Sie HTTP 200 OK und die [Ereignis](../api-reference/v1.0/resources/event.md)-Instanz mit der ID `{id}` aus Garths Standardkalender.</span><span class="sxs-lookup"><span data-stu-id="97278-110">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/event.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-the-events-in-the-shared-calendar"></a><span data-ttu-id="97278-111">Alle Ereignisse in dem freigegebenen Kalender abrufen</span><span class="sxs-lookup"><span data-stu-id="97278-111">Get all the events in the shared calendar</span></span>

<span data-ttu-id="97278-112">Abrufen aller Ereignisse im Standardkalender, den Garth für John freigegeben hat:</span><span class="sxs-lookup"><span data-stu-id="97278-112">Get all the events in the default calendar that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

<span data-ttu-id="97278-113">Bei erfolgreichem Abschluss erhalten Sie HTTP 200 OK und eine Sammlung von [Ereignis](../api-reference/v1.0/resources/event.md)-Instanzen in Garths Standardkalender.</span><span class="sxs-lookup"><span data-stu-id="97278-113">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/event.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-calendar"></a><span data-ttu-id="97278-114">Abrufen des freigegebenen Kalenders</span><span class="sxs-lookup"><span data-stu-id="97278-114">Get the shared folder</span></span>

<span data-ttu-id="97278-115">Abrufen des Standardkalenders, den Garth für John freigegeben hat.</span><span class="sxs-lookup"><span data-stu-id="97278-115">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

<span data-ttu-id="97278-116">Bei erfolgreichem Abschluss erhalten Sie HTTP 200 OK und eine [Kalender](../api-reference/v1.0/resources/calendar.md)-Instanz, die Garths Standardordner darstellt.</span><span class="sxs-lookup"><span data-stu-id="97278-116">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/calendar.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="97278-117">Dieselben GET-Funktionen würden gelten, wenn Garth an John weiteren Zugriff auf Garths Standardkalender delegiert hätte oder wenn Garth sein gesamtes Postfach an John delegiert hätte.</span><span class="sxs-lookup"><span data-stu-id="97278-117">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="97278-118">Wenn Garth weder seinen Standardkalender für John freigegeben noch sein Postfach an John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97278-118">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="97278-119">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="97278-119">Next steps</span></span>

<span data-ttu-id="97278-120">Weitere Informationen:</span><span class="sxs-lookup"><span data-stu-id="97278-120">Find out more about:</span></span>

- [<span data-ttu-id="97278-121">Vorteile der Integration mit dem Outlook-Kalender</span><span class="sxs-lookup"><span data-stu-id="97278-121">Why integrate with Outlook calendar?</span></span>](outlook-calendar-concept-overview.md)
- <span data-ttu-id="97278-122">Die [Kalender-API](../api-reference/v1.0/resources/calendar.md) in Microsoft Graph v1. 0.</span><span class="sxs-lookup"><span data-stu-id="97278-122">The [calendar API](../api-reference/v1.0/resources/calendar.md) in Microsoft Graph v1.0.</span></span>