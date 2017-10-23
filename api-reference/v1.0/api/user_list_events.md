# <a name="list-events"></a><span data-ttu-id="3aacc-101">Ereignisse auflisten</span><span class="sxs-lookup"><span data-stu-id="3aacc-101">List events</span></span>

<span data-ttu-id="3aacc-p101">Dient zum Abrufen einer Liste der [event](../resources/event.md)-Objekte im Postfach des Benutzers. Die Liste enthält einzelne Instanzen von Besprechungen und Serienmaster.</span><span class="sxs-lookup"><span data-stu-id="3aacc-p101">Get a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="3aacc-104">Zurzeit gibt dieser Vorgang Ereignistext nur im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="3aacc-104">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="3aacc-105">Um erweiterte Ereignisinstanzen abzurufen, können Sie [die Kalenderansicht abrufen](calendar_list_calendarview.md) oder [die Instanzen eines Ereignisses abrufen](event_list_instances.md).</span><span class="sxs-lookup"><span data-stu-id="3aacc-105">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>


### <a name="get-events-in-another-users-calendar"></a><span data-ttu-id="3aacc-106">Abrufen von Ereignissen aus dem Kalender eines anderen Benutzers</span><span class="sxs-lookup"><span data-stu-id="3aacc-106">Get events in another user's calendar</span></span>

<span data-ttu-id="3aacc-107">Wenn Sie über Anwendungsberechtigungen oder die entsprechenden delegierten [Berechtigungen](#permissions) eines Benutzers verfügen, können Sie Ereignisse aus dem Kalender eines anderen Benutzers anzeigen.</span><span class="sxs-lookup"><span data-stu-id="3aacc-107">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get events from another user's calendar.</span></span> <span data-ttu-id="3aacc-108">Dieser Abschnitt enthält Szenarien zu delegierten Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="3aacc-108">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="3aacc-109">Beispiel: Ihre App besitzt delegierte Berechtigungen des Benutzers John.</span><span class="sxs-lookup"><span data-stu-id="3aacc-109">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="3aacc-110">Der Benutzer Garth hat einen Kalender für John freigegeben.</span><span class="sxs-lookup"><span data-stu-id="3aacc-110">Suppose another user, Garth, has shared a calendar with John.</span></span> <span data-ttu-id="3aacc-111">Sie können die Ereignisse aus dem freigegebenen Kalender aufrufen, indem Sie Garths Benutzer-ID (oder den Benutzerprinzipalnamen) in der unten gezeigten Beispielabfrage angeben.</span><span class="sxs-lookup"><span data-stu-id="3aacc-111">You can get the events in that shared calendar by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/events
```

<span data-ttu-id="3aacc-112">Diese Funktion gilt für alle unterstützten GET-Ereignisvorgänge für einen einzelnen Benutzer (siehe Abschnitt [HTTP-Anforderung](#http-request) unten).</span><span class="sxs-lookup"><span data-stu-id="3aacc-112">This capability applies to all the supported GET events operations for an individual user, as listed in the [HTTP request](#http-request) section below.</span></span> <span data-ttu-id="3aacc-113">Sie gilt auch, wenn Garth sein gesamtes Postfach an John delegiert hat.</span><span class="sxs-lookup"><span data-stu-id="3aacc-113">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="3aacc-114">Wenn Garth weder seinen Kalender für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3aacc-114">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="3aacc-115">In solchen Fällen funktioniert die Angabe einer Benutzer-ID oder eines Benutzerprinzipalnamens nur, um Ereignisse aus dem Kalender eines angemeldeten Benutzers abzurufen, und die Abfrage entspricht der Verwendung der Verknüpfung the /me:</span><span class="sxs-lookup"><span data-stu-id="3aacc-115">In such cases, specifying a user ID or user principal name only works for getting events in the signed-in user’s own calendars, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/events
```

<span data-ttu-id="3aacc-116">Diese Funktion ist nur in GET-Vorgängen verfügbar für:</span><span class="sxs-lookup"><span data-stu-id="3aacc-116">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="3aacc-117">Freigegebene Kontaktordner</span><span class="sxs-lookup"><span data-stu-id="3aacc-117">Shared contact folders</span></span>
- <span data-ttu-id="3aacc-118">Freigegebene Kalender</span><span class="sxs-lookup"><span data-stu-id="3aacc-118">Shared calendars</span></span>
- <span data-ttu-id="3aacc-119">Kontakte und Ereignisse in freigegebenen Ordnern</span><span class="sxs-lookup"><span data-stu-id="3aacc-119">Contacts and events in shared folders</span></span>
- <span data-ttu-id="3aacc-120">Die oben aufgeführten Ressourcen in delegierten Postfächern</span><span class="sxs-lookup"><span data-stu-id="3aacc-120">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="3aacc-121">Diese Funktion steht in anderen Vorgängen für Kontakte, Ereignisse und deren Ordner nicht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="3aacc-121">This capability is not available in other operations for contacts, events, and their folders.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="3aacc-122">Unterstützen verschiedener Zeitzonen</span><span class="sxs-lookup"><span data-stu-id="3aacc-122">Support various time zones</span></span>

<span data-ttu-id="3aacc-123">Für alle GET-Vorgänge, die Ereignisse zurückgeben, können Sie den `Prefer: outlook.timezone`-Header zum Angeben der Zeitzone für die Anfangs- und Endzeit des Ereignisses in der Antwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="3aacc-123">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="3aacc-124">Mit dem folgenden `Prefer: outlook.timezone`-Header werden zum Beispiel die Anfangs- und Endzeiten in der Antwort auf EST festgelegt.</span><span class="sxs-lookup"><span data-stu-id="3aacc-124">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="3aacc-p106">Wenn das Ereignis in einer anderen Zeitzone erstellt wurde, werden die Anfangs- und Endzeiten an die in diesem `Prefer`-Header angegebene Zeitzone angepasst. Die unterstützten Zeitzonen finden Sie in dieser [Liste](../resources/datetimetimezone.md). Wenn der `Prefer: outlook.timezone`-Header nicht angegeben ist, werden die Anfangs- und Endzeiten in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3aacc-p106">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="3aacc-128">Sie können die **OriginalStartTimeZone**- und **OriginalEndTimeZone**-Eigenschaften für die **event**-Ressource verwenden, um die beim Erstellen des Ereignisses verwendete Zeitzone abzurufen.</span><span class="sxs-lookup"><span data-stu-id="3aacc-128">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="3aacc-129">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3aacc-129">Permissions</span></span>
<span data-ttu-id="3aacc-p107">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3aacc-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3aacc-132">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3aacc-132">Permission type</span></span>      | <span data-ttu-id="3aacc-133">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3aacc-133">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3aacc-134">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3aacc-134">Delegated (work or school account)</span></span> | <span data-ttu-id="3aacc-135">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3aacc-135">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="3aacc-136">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3aacc-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3aacc-137">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3aacc-137">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="3aacc-138">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3aacc-138">Application</span></span> | <span data-ttu-id="3aacc-139">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3aacc-139">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3aacc-140">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3aacc-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events
GET /users/{id | userPrincipalName}/events

GET /me/calendar/events
GET /users/{id | userPrincipalName}/calendar/events

GET /me/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendars/{id}/events

GET /me/calendargroup/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events

GET /me/calendargroups/{id}/calendars/{id}/events
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3aacc-141">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3aacc-141">Optional query parameters</span></span>
<span data-ttu-id="3aacc-142">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3aacc-142">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3aacc-143">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3aacc-143">Request headers</span></span>
| <span data-ttu-id="3aacc-144">Name</span><span class="sxs-lookup"><span data-stu-id="3aacc-144">Name</span></span>       | <span data-ttu-id="3aacc-145">Typ</span><span class="sxs-lookup"><span data-stu-id="3aacc-145">Type</span></span> | <span data-ttu-id="3aacc-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3aacc-146">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3aacc-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="3aacc-147">Authorization</span></span>  | <span data-ttu-id="3aacc-148">string</span><span class="sxs-lookup"><span data-stu-id="3aacc-148">string</span></span>  | <span data-ttu-id="3aacc-p108">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3aacc-p108">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3aacc-151">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="3aacc-151">Prefer: outlook.timezone</span></span> | <span data-ttu-id="3aacc-152">string</span><span class="sxs-lookup"><span data-stu-id="3aacc-152">string</span></span> | <span data-ttu-id="3aacc-p109">Die Standardzeitzone für Ereignisse in der Antwort. Optional.</span><span class="sxs-lookup"><span data-stu-id="3aacc-p109">The default time zone for events in the response. Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3aacc-155">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3aacc-155">Request body</span></span>
<span data-ttu-id="3aacc-156">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3aacc-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3aacc-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="3aacc-157">Response</span></span>

<span data-ttu-id="3aacc-158">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3aacc-158">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3aacc-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3aacc-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3aacc-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3aacc-160">Request</span></span>
<span data-ttu-id="3aacc-p110">Nachfolgend sehen Sie ein Beispiel der Anforderung. Es gibt Folgendes an:</span><span class="sxs-lookup"><span data-stu-id="3aacc-p110">Here is an example of the request. It specifies the following:</span></span>

- <span data-ttu-id="3aacc-163">Einen `Prefer: outlook.timezone`-Header zum Abrufen von Datums- und Uhrzeitwerten in 	Pacific Normalzeit.</span><span class="sxs-lookup"><span data-stu-id="3aacc-163">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="3aacc-p111">Einen `$select`-Abfrageparameter zum Zurückgeben bestimmter Eigenschaften. Ohne `$select`-Parameter werden alle Ereigniseigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3aacc-p111">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response"></a><span data-ttu-id="3aacc-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="3aacc-166">Response</span></span>
<span data-ttu-id="3aacc-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Die **body**-Eigenschaft wird im HTML-Standardformat zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3aacc-p112">Here is an example of the response. The **body** property is returned in the default HTML format.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-length: 1932

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)",
    "value":[
        {
            "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAAKGWwbw==\"",
            "id":"AAMkAGIAAAoZDOFAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"html",
                "content":"<html><head></head><body><p>Dana, this is the time you selected for our orientation. Please bring the notes I sent you.</p></body></html>"
            },
            "start":{
                "dateTime":"2017-04-21T10:00:00.0000000",
                "timeZone":"Pacific Standard Time"
            },
            "end":{
                "dateTime":"2017-04-21T12:00:00.0000000",
                "timeZone":"Pacific Standard Time"
            },
            "location":{
                "displayName":"Assembly Hall"
            },
            "attendees":[
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Samantha Booth",
                        "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
                    }
                },
                {
                    "type":"required",
                    "status":{
                        "response":"none",
                        "time":"0001-01-01T00:00:00Z"
                    },
                    "emailAddress":{
                        "name":"Dana Swope",
                        "address":"danas@a830edad905084922E17020313.onmicrosoft.com"
                    }
                }
            ],
            "organizer":{
                "emailAddress":{
                    "name":"Samantha Booth",
                    "address":"samanthab@a830edad905084922E17020313.onmicrosoft.com"
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
