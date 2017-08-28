# <a name="list-events"></a><span data-ttu-id="45f27-101">Ereignisse auflisten</span><span class="sxs-lookup"><span data-stu-id="45f27-101">List events</span></span>

<span data-ttu-id="45f27-p101">Dient zum Abrufen einer Liste der [event](../resources/event.md)-Objekte im Postfach des Benutzers. Die Liste enthält einzelne Instanzen von Besprechungen und Serienmaster.</span><span class="sxs-lookup"><span data-stu-id="45f27-p101">Get a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="45f27-104">Zurzeit gibt dieser Vorgang Ereignistext nur im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="45f27-104">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="45f27-105">Um erweiterte Ereignisinstanzen abzurufen, können Sie [die Kalenderansicht abrufen](calendar_list_calendarview.md) oder [die Instanzen eines Ereignisses abrufen](event_list_instances.md).</span><span class="sxs-lookup"><span data-stu-id="45f27-105">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>

### <a name="support-various-time-zones"></a><span data-ttu-id="45f27-106">Unterstützen verschiedener Zeitzonen</span><span class="sxs-lookup"><span data-stu-id="45f27-106">Support various time zones</span></span>

<span data-ttu-id="45f27-107">Für alle GET-Vorgänge, die Ereignisse zurückgeben, können Sie den `Prefer: outlook.timezone`-Header zum Angeben der Zeitzone für die Anfangs- und Endzeit des Ereignisses in der Antwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="45f27-107">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="45f27-108">Mit dem folgenden `Prefer: outlook.timezone`-Header werden zum Beispiel die Anfangs- und Endzeiten in der Antwort auf EST festgelegt.</span><span class="sxs-lookup"><span data-stu-id="45f27-108">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="45f27-p102">Wenn das Ereignis in einer anderen Zeitzone erstellt wurde, werden die Anfangs- und Endzeiten an die in diesem `Prefer`-Header angegebene Zeitzone angepasst. Die unterstützten Zeitzonen finden Sie in dieser [Liste](../resources/datetimetimezone.md). Wenn der `Prefer: outlook.timezone`-Header nicht angegeben ist, werden die Anfangs- und Endzeiten in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="45f27-p102">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="45f27-112">Sie können die **OriginalStartTimeZone**- und **OriginalEndTimeZone**-Eigenschaften für die **event**-Ressource verwenden, um die beim Erstellen des Ereignisses verwendete Zeitzone abzurufen.</span><span class="sxs-lookup"><span data-stu-id="45f27-112">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="45f27-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="45f27-113">Permissions</span></span>
<span data-ttu-id="45f27-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="45f27-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="45f27-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="45f27-116">Permission type</span></span>      | <span data-ttu-id="45f27-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="45f27-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45f27-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="45f27-118">Delegated (work or school account)</span></span> | <span data-ttu-id="45f27-119">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45f27-119">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="45f27-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="45f27-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45f27-121">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45f27-121">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="45f27-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="45f27-122">Application</span></span> | <span data-ttu-id="45f27-123">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45f27-123">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="45f27-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="45f27-124">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="45f27-125">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="45f27-125">Optional query parameters</span></span>
<span data-ttu-id="45f27-126">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="45f27-126">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="45f27-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="45f27-127">Request headers</span></span>
| <span data-ttu-id="45f27-128">Name</span><span class="sxs-lookup"><span data-stu-id="45f27-128">Name</span></span>       | <span data-ttu-id="45f27-129">Typ</span><span class="sxs-lookup"><span data-stu-id="45f27-129">Type</span></span> | <span data-ttu-id="45f27-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="45f27-130">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="45f27-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="45f27-131">Authorization</span></span>  | <span data-ttu-id="45f27-132">string</span><span class="sxs-lookup"><span data-stu-id="45f27-132">string</span></span>  | <span data-ttu-id="45f27-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="45f27-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="45f27-135">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="45f27-135">Prefer: outlook.timezone</span></span> | <span data-ttu-id="45f27-136">string</span><span class="sxs-lookup"><span data-stu-id="45f27-136">string</span></span> | <span data-ttu-id="45f27-p105">Die Standardzeitzone für Ereignisse in der Antwort. Optional.</span><span class="sxs-lookup"><span data-stu-id="45f27-p105">The default time zone for events in the response. Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45f27-139">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="45f27-139">Request body</span></span>
<span data-ttu-id="45f27-140">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="45f27-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45f27-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="45f27-141">Response</span></span>

<span data-ttu-id="45f27-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="45f27-142">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="45f27-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="45f27-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45f27-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="45f27-144">Request</span></span>
<span data-ttu-id="45f27-p106">Nachfolgend sehen Sie ein Beispiel der Anforderung. Es gibt Folgendes an:</span><span class="sxs-lookup"><span data-stu-id="45f27-p106">Here is an example of the request. It specifies the following:</span></span>

- <span data-ttu-id="45f27-147">Einen `Prefer: outlook.timezone`-Header zum Abrufen von Datums- und Uhrzeitwerten in 	Pacific Normalzeit.</span><span class="sxs-lookup"><span data-stu-id="45f27-147">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="45f27-p107">Einen `$select`-Abfrageparameter zum Zurückgeben bestimmter Eigenschaften. Ohne `$select`-Parameter werden alle Ereigniseigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="45f27-p107">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response"></a><span data-ttu-id="45f27-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="45f27-150">Response</span></span>
<span data-ttu-id="45f27-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Die **body**-Eigenschaft wird im HTML-Standardformat zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="45f27-p108">Here is an example of the response. The **body** property is returned in the default HTML format.</span></span>
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
                        "name":"Fanny Downs",
                        "address":"fannyd@a830edad905084922E17020313.onmicrosoft.com"
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
                    "name":"Fanny Downs",
                    "address":"fannyd@a830edad905084922E17020313.onmicrosoft.com"
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
