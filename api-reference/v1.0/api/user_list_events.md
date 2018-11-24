# <a name="list-events"></a><span data-ttu-id="12550-101">Ereignisse auflisten</span><span class="sxs-lookup"><span data-stu-id="12550-101">List events</span></span>

<span data-ttu-id="12550-p101">Dient zum Abrufen einer Liste der [event](../resources/event.md)-Objekte im Postfach des Benutzers. Die Liste enthält einzelne Instanzen von Besprechungen und Serienmaster.</span><span class="sxs-lookup"><span data-stu-id="12550-p101">Get a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>

<span data-ttu-id="12550-104">Um erweiterte Ereignisinstanzen abzurufen, können Sie [die Kalenderansicht abrufen](calendar_list_calendarview.md) oder [die Instanzen eines Ereignisses abrufen](event_list_instances.md).</span><span class="sxs-lookup"><span data-stu-id="12550-104">To get expanded event instances, you can [get the calendar view](calendar_list_calendarview.md), or [get the instances of an event](event_list_instances.md).</span></span>

<span data-ttu-id="12550-105">Zurzeit gibt dieser Vorgang Ereignistext nur im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="12550-105">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="12550-106">Es gibt zwei Szenarien, in dem eine app Ereignisse im Kalender des Benutzers abzurufen:</span><span class="sxs-lookup"><span data-stu-id="12550-106">There are two scenarios where an app can get events in another user's calendar:</span></span>

* <span data-ttu-id="12550-107">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="12550-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="12550-108">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer der Benutzer einen Kalender freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="12550-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a calendar with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="12550-109">Finden Sie [ausführliche Informationen und ein Beispiel](../../../concepts/outlook-get-shared-events-calendars.md).</span><span class="sxs-lookup"><span data-stu-id="12550-109">See [details and an example](../../../concepts/outlook-get-shared-events-calendars.md).</span></span>

### <a name="support-various-time-zones"></a><span data-ttu-id="12550-110">Unterstützen verschiedener Zeitzonen</span><span class="sxs-lookup"><span data-stu-id="12550-110">Support various time zones</span></span>

<span data-ttu-id="12550-111">Für alle GET-Vorgänge, die Ereignisse zurückgeben, können Sie den `Prefer: outlook.timezone`-Header zum Angeben der Zeitzone für die Anfangs- und Endzeit des Ereignisses in der Antwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="12550-111">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="12550-112">Mit dem folgenden `Prefer: outlook.timezone`-Header werden zum Beispiel die Anfangs- und Endzeiten in der Antwort auf EST festgelegt.</span><span class="sxs-lookup"><span data-stu-id="12550-112">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="12550-p103">Wenn das Ereignis in einer anderen Zeitzone erstellt wurde, werden die Anfangs- und Endzeiten an die in diesem `Prefer`-Header angegebene Zeitzone angepasst. Die unterstützten Zeitzonen finden Sie in dieser [Liste](../resources/datetimetimezone.md). Wenn der `Prefer: outlook.timezone`-Header nicht angegeben ist, werden die Anfangs- und Endzeiten in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12550-p103">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="12550-116">Sie können die **OriginalStartTimeZone**- und **OriginalEndTimeZone**-Eigenschaften für die **event**-Ressource verwenden, um die beim Erstellen des Ereignisses verwendete Zeitzone abzurufen.</span><span class="sxs-lookup"><span data-stu-id="12550-116">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>

## <a name="permissions"></a><span data-ttu-id="12550-117">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="12550-117">Permissions</span></span>
<span data-ttu-id="12550-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="12550-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="12550-120">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="12550-120">Permission type</span></span>      | <span data-ttu-id="12550-121">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="12550-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12550-122">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="12550-122">Delegated (work or school account)</span></span> | <span data-ttu-id="12550-123">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12550-123">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="12550-124">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="12550-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12550-125">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12550-125">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="12550-126">Anwendung</span><span class="sxs-lookup"><span data-stu-id="12550-126">Application</span></span> | <span data-ttu-id="12550-127">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12550-127">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="12550-128">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="12550-128">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="12550-129">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="12550-129">Optional query parameters</span></span>
<span data-ttu-id="12550-130">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="12550-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="12550-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="12550-131">Request headers</span></span>
| <span data-ttu-id="12550-132">Name</span><span class="sxs-lookup"><span data-stu-id="12550-132">Name</span></span>       | <span data-ttu-id="12550-133">Typ</span><span class="sxs-lookup"><span data-stu-id="12550-133">Type</span></span> | <span data-ttu-id="12550-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12550-134">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="12550-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="12550-135">Authorization</span></span>  | <span data-ttu-id="12550-136">string</span><span class="sxs-lookup"><span data-stu-id="12550-136">string</span></span> | <span data-ttu-id="12550-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="12550-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="12550-139">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="12550-139">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="12550-140">string</span><span class="sxs-lookup"><span data-stu-id="12550-140">string</span></span> | <span data-ttu-id="12550-141">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="12550-141">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="12550-142">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12550-142">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="12550-143">Optional.</span><span class="sxs-lookup"><span data-stu-id="12550-143">Optional.</span></span> |
| <span data-ttu-id="12550-144">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="12550-144">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="12550-145">string</span><span class="sxs-lookup"><span data-stu-id="12550-145">string</span></span> | <span data-ttu-id="12550-146">Das Format, in der die **body**-Eigenschaft zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="12550-146">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="12550-147">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="12550-147">Values can be "text" or "html".</span></span> <span data-ttu-id="12550-148">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="12550-148">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="12550-149">Wenn die Kopfzeile nicht angegeben ist, wird die **body**-Eigenschaft im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12550-149">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="12550-150">Optional.</span><span class="sxs-lookup"><span data-stu-id="12550-150">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12550-151">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="12550-151">Request body</span></span>
<span data-ttu-id="12550-152">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="12550-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12550-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="12550-153">Response</span></span>

<span data-ttu-id="12550-154">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12550-154">If successful, this method returns a `200 OK` response code and collection of [event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="12550-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="12550-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12550-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="12550-156">Request</span></span>
<span data-ttu-id="12550-p108">Nachfolgend sehen Sie ein Beispiel der Anforderung. Es gibt Folgendes an:</span><span class="sxs-lookup"><span data-stu-id="12550-p108">Here is an example of the request. It specifies the following:</span></span>

- <span data-ttu-id="12550-159">Einen `Prefer: outlook.timezone`-Header zum Abrufen von Datums- und Uhrzeitwerten in 	Pacific Normalzeit.</span><span class="sxs-lookup"><span data-stu-id="12550-159">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="12550-p109">Einen `$select`-Abfrageparameter zum Zurückgeben bestimmter Eigenschaften. Ohne `$select`-Parameter werden alle Ereigniseigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12550-p109">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response"></a><span data-ttu-id="12550-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="12550-162">Response</span></span>
<span data-ttu-id="12550-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Die **body**-Eigenschaft wird im HTML-Standardformat zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="12550-p110">Here is an example of the response. The **body** property is returned in the default HTML format.</span></span>
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
            "location": {
                "displayName": "Assembly Hall",
                "locationType": "default",
                "uniqueId": "Assembly Hall",
                "uniqueIdType": "private"
            },
            "locations": [
                {
                    "displayName": "Assembly Hall",
                    "locationType": "default",
                    "uniqueIdType": "unknown"
                }
            ],
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
