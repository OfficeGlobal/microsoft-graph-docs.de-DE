# <a name="get-event"></a><span data-ttu-id="6c6c2-101">Ereignis abrufen</span><span class="sxs-lookup"><span data-stu-id="6c6c2-101">Get event</span></span>

<span data-ttu-id="6c6c2-102">Dient zum Abrufen der Eigenschaften und Beziehungen des angegebenen [event](../resources/event.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-102">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="6c6c2-103">Zurzeit gibt dieser Vorgang Ereignistext nur im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-103">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="6c6c2-104">Da die **event**-Ressource [Erweiterungen](../../../concepts/extensibility_overview.md) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **event**-Instanzen abrufen.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-104">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>

### <a name="support-various-time-zones"></a><span data-ttu-id="6c6c2-105">Unterstützen verschiedener Zeitzonen</span><span class="sxs-lookup"><span data-stu-id="6c6c2-105">Support various time zones</span></span>

<span data-ttu-id="6c6c2-106">Für alle GET-Vorgänge, die Ereignisse zurückgeben, können Sie den `Prefer: outlook.timezone`-Header zum Angeben der Zeitzone für die Anfangs- und Endzeit des Ereignisses in der Antwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-106">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="6c6c2-107">Mit dem folgenden `Prefer: outlook.timezone`-Header werden zum Beispiel die Anfangs- und Endzeiten in der Antwort auf EST festgelegt.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-107">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="6c6c2-p101">Wenn das Ereignis in einer anderen Zeitzone erstellt wurde, werden die Anfangs- und Endzeiten an die in diesem `Prefer`-Header angegebene Zeitzone angepasst. Die unterstützten Zeitzonen finden Sie in dieser [Liste](../resources/datetimetimezone.md). Wenn der `Prefer: outlook.timezone`-Header nicht angegeben ist, werden die Anfangs- und Endzeiten in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-p101">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="6c6c2-111">Sie können die **OriginalStartTimeZone**- und **OriginalEndTimeZone**-Eigenschaften für die **event**-Ressource verwenden, um die beim Erstellen des Ereignisses verwendete Zeitzone abzurufen.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-111">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>


## <a name="permissions"></a><span data-ttu-id="6c6c2-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6c6c2-112">Permissions</span></span>
<span data-ttu-id="6c6c2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6c6c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6c6c2-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6c6c2-115">Permission type</span></span>      | <span data-ttu-id="6c6c2-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6c6c2-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c6c2-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6c6c2-117">Delegated (work or school account)</span></span> | <span data-ttu-id="6c6c2-118">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6c6c2-118">Calendars.Read</span></span>    |
|<span data-ttu-id="6c6c2-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6c6c2-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c6c2-120">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6c6c2-120">Calendars.Read</span></span>    |
|<span data-ttu-id="6c6c2-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6c6c2-121">Application</span></span> | <span data-ttu-id="6c6c2-122">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6c6c2-122">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c6c2-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c6c2-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}
GET /users/{id | userPrincipalName}/events/{id}
GET /groups/{id}/events/{id}

GET /me/calendar/events/{id}
GET /users/{id | userPrincipalName}/calendar/events/{id}
GET /groups/{id}/calendar/events/{id}

GET /me/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}

GET /me/calendargroup/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6c6c2-124">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6c6c2-124">Optional query parameters</span></span>
<span data-ttu-id="6c6c2-125">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-125">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6c6c2-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6c6c2-126">Request headers</span></span>
| <span data-ttu-id="6c6c2-127">Name</span><span class="sxs-lookup"><span data-stu-id="6c6c2-127">Name</span></span>       | <span data-ttu-id="6c6c2-128">Typ</span><span class="sxs-lookup"><span data-stu-id="6c6c2-128">Type</span></span> | <span data-ttu-id="6c6c2-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6c6c2-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6c6c2-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c6c2-130">Authorization</span></span>  | <span data-ttu-id="6c6c2-131">string</span><span class="sxs-lookup"><span data-stu-id="6c6c2-131">string</span></span>  | <span data-ttu-id="6c6c2-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6c6c2-134">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="6c6c2-134">Prefer: outlook.timezone</span></span> | <span data-ttu-id="6c6c2-135">string</span><span class="sxs-lookup"><span data-stu-id="6c6c2-135">string</span></span> | <span data-ttu-id="6c6c2-136">Die Standardzeitzone für Ereignisse in der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-136">The default time zone for events in the response.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c6c2-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6c6c2-137">Request body</span></span>
<span data-ttu-id="6c6c2-138">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c6c2-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c6c2-139">Response</span></span>

<span data-ttu-id="6c6c2-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [event](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-140">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6c6c2-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6c6c2-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6c6c2-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6c6c2-142">Request</span></span>
<span data-ttu-id="6c6c2-p104">Im erste Beispiel wird das angegebene Ereignis abgerufen. Es gibt Folgendes an:</span><span class="sxs-lookup"><span data-stu-id="6c6c2-p104">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="6c6c2-145">Einen `Prefer: outlook.timezone`-Header zum Abrufen von Datums- und Uhrzeitwerten in 	Pacific Normalzeit.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-145">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="6c6c2-p105">Einen `$select`-Abfrageparameter zum Zurückgeben bestimmter Eigenschaften. Ohne `$select`-Parameter werden alle Ereigniseigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-p105">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_event"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGIAAAoZDOFAAA=')?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```

##### <a name="response"></a><span data-ttu-id="6c6c2-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="6c6c2-148">Response</span></span>

<span data-ttu-id="6c6c2-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Die **body**-Eigenschaft wird im HTML-Standardformat zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6c6c2-p106">Here is an example of the response. The **body** property is returned in the default format of HTML.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-length: 1928

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events(subject,body,bodyPreview,organizer,attendees,start,end,location)/$entity",
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
```

## <a name="see-also"></a><span data-ttu-id="6c6c2-151">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="6c6c2-151">See also</span></span>

- [<span data-ttu-id="6c6c2-152">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="6c6c2-152">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="6c6c2-153">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="6c6c2-153">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
