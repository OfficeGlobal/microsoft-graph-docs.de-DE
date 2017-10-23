# <a name="get-event"></a><span data-ttu-id="fd25e-101">Ereignis abrufen</span><span class="sxs-lookup"><span data-stu-id="fd25e-101">Get event</span></span>

<span data-ttu-id="fd25e-102">Dient zum Abrufen der Eigenschaften und Beziehungen des angegebenen [event](../resources/event.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="fd25e-102">Get the properties and relationships of the specified [event](../resources/event.md) object.</span></span>

<span data-ttu-id="fd25e-103">Zurzeit gibt dieser Vorgang Ereignistext nur im HTML-Format zurück.</span><span class="sxs-lookup"><span data-stu-id="fd25e-103">Currently, this operation returns event bodies in only HTML format.</span></span>

<span data-ttu-id="fd25e-104">Da die **event**-Ressource [Erweiterungen](../../../concepts/extensibility_overview.md) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **event**-Instanzen abrufen.</span><span class="sxs-lookup"><span data-stu-id="fd25e-104">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can also use the `GET` operation to get custom properties and extension data in an **event** instance.</span></span>


### <a name="get-events-in-another-users-calendar"></a><span data-ttu-id="fd25e-105">Abrufen von Ereignissen aus dem Kalender eines anderen Benutzers</span><span class="sxs-lookup"><span data-stu-id="fd25e-105">Get events in another user's calendar</span></span>

<span data-ttu-id="fd25e-106">Wenn Sie über Anwendungsberechtigungen oder die entsprechenden delegierten [Berechtigungen](#permissions) eines Benutzers verfügen, können Sie Ereignisse aus dem Kalender eines anderen Benutzers anzeigen.</span><span class="sxs-lookup"><span data-stu-id="fd25e-106">If you have application permissions, or if you have the appropriate delegated [permissions](#permissions) from one user, it's possible to get events from another user's calendar.</span></span> <span data-ttu-id="fd25e-107">Dieser Abschnitt enthält Szenarien zu delegierten Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="fd25e-107">This section focuses on scenarios that involve delegated permissions.</span></span>

<span data-ttu-id="fd25e-108">Beispiel: Ihre App besitzt delegierte Berechtigungen des Benutzers John.</span><span class="sxs-lookup"><span data-stu-id="fd25e-108">For example, your app has acquired delegated permissions from the user, John.</span></span> <span data-ttu-id="fd25e-109">Der Benutzer Garth hat einen Kalender für John freigegeben.</span><span class="sxs-lookup"><span data-stu-id="fd25e-109">Suppose another user, Garth, has shared a calendar with John.</span></span> <span data-ttu-id="fd25e-110">Sie können ein Ereignis aus dem freigegebenen Kalender aufrufen, indem Sie Garths Benutzer-ID (oder den Benutzerprinzipalnamen) in der unten gezeigten Beispielabfrage angeben.</span><span class="sxs-lookup"><span data-stu-id="fd25e-110">You can get an event in that shared calendar by specifying Garth’s user ID (or user principal name) in the example query shown below.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/events/{id}
```

<span data-ttu-id="fd25e-111">Diese Funktion gilt für alle unterstützten GET-Ereignisvorgänge für einen einzelnen Benutzer (siehe Abschnitt [HTTP-Anforderung](#http-request) unten).</span><span class="sxs-lookup"><span data-stu-id="fd25e-111">This capability applies to all the supported GET events operations for an individual user, as listed in the [HTTP request](#http-request) section below .</span></span> <span data-ttu-id="fd25e-112">Sie gilt auch, wenn Garth sein gesamtes Postfach an John delegiert hat.</span><span class="sxs-lookup"><span data-stu-id="fd25e-112">It also applies if Garth has delegated his entire mailbox to John.</span></span>

<span data-ttu-id="fd25e-113">Wenn Garth weder seinen Kalender für John freigegeben noch sein Postfach für John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd25e-113">If Garth has not shared his calendar with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> <span data-ttu-id="fd25e-114">In solchen Fällen funktioniert die Angabe einer Benutzer-ID oder eines Benutzerprinzipalnamens nur, um ein Ereignis aus dem Kalender eines angemeldeten Benutzers abzurufen, und die Abfrage entspricht der Verwendung der Verknüpfung the /me:</span><span class="sxs-lookup"><span data-stu-id="fd25e-114">In such cases, specifying a user ID or user principal name only works for getting an event in the signed-in user’s own calendars, and the query is equivalent to using the /me shortcut:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}
```

<span data-ttu-id="fd25e-115">Diese Funktion ist nur in GET-Vorgängen verfügbar für:</span><span class="sxs-lookup"><span data-stu-id="fd25e-115">This capability is available in only GET operations of:</span></span>

- <span data-ttu-id="fd25e-116">Freigegebene Kontaktordner</span><span class="sxs-lookup"><span data-stu-id="fd25e-116">Shared contact folders</span></span>
- <span data-ttu-id="fd25e-117">Freigegebene Kalender</span><span class="sxs-lookup"><span data-stu-id="fd25e-117">Shared calendars</span></span>
- <span data-ttu-id="fd25e-118">Kontakte und Ereignisse in freigegebenen Ordnern</span><span class="sxs-lookup"><span data-stu-id="fd25e-118">Contacts and events in shared folders</span></span>
- <span data-ttu-id="fd25e-119">Die oben aufgeführten Ressourcen in delegierten Postfächern</span><span class="sxs-lookup"><span data-stu-id="fd25e-119">The above resources in delegated mailboxes</span></span>

<span data-ttu-id="fd25e-120">Diese Funktion steht in anderen Vorgängen für Kontakte, Ereignisse und deren Ordner nicht zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="fd25e-120">This capability is not available in other operations for contacts, events, and their folders.</span></span>


### <a name="support-various-time-zones"></a><span data-ttu-id="fd25e-121">Unterstützen verschiedener Zeitzonen</span><span class="sxs-lookup"><span data-stu-id="fd25e-121">Support various time zones</span></span>

<span data-ttu-id="fd25e-122">Für alle GET-Vorgänge, die Ereignisse zurückgeben, können Sie den `Prefer: outlook.timezone`-Header zum Angeben der Zeitzone für die Anfangs- und Endzeit des Ereignisses in der Antwort verwenden.</span><span class="sxs-lookup"><span data-stu-id="fd25e-122">For all GET operations that return events, you can use the `Prefer: outlook.timezone` header to specify the time zone for the event start and end times in the response.</span></span> 

<span data-ttu-id="fd25e-123">Mit dem folgenden `Prefer: outlook.timezone`-Header werden zum Beispiel die Anfangs- und Endzeiten in der Antwort auf EST festgelegt.</span><span class="sxs-lookup"><span data-stu-id="fd25e-123">For example, the following `Prefer: outlook.timezone` header sets the start and end times in the response to Eastern Standard Time.</span></span>
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

<span data-ttu-id="fd25e-p105">Wenn das Ereignis in einer anderen Zeitzone erstellt wurde, werden die Anfangs- und Endzeiten an die in diesem `Prefer`-Header angegebene Zeitzone angepasst. Die unterstützten Zeitzonen finden Sie in dieser [Liste](../resources/datetimetimezone.md). Wenn der `Prefer: outlook.timezone`-Header nicht angegeben ist, werden die Anfangs- und Endzeiten in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd25e-p105">If the event was created in a different time zone, the start and end times will be adjusted to the time zone specified in that `Prefer` header. See this [list](../resources/datetimetimezone.md) for the supported time zone names. If the `Prefer: outlook.timezone` header is not specified, the start and end times are returned in UTC.</span></span>

<span data-ttu-id="fd25e-127">Sie können die **OriginalStartTimeZone**- und **OriginalEndTimeZone**-Eigenschaften für die **event**-Ressource verwenden, um die beim Erstellen des Ereignisses verwendete Zeitzone abzurufen.</span><span class="sxs-lookup"><span data-stu-id="fd25e-127">You can use the **OriginalStartTimeZone** and **OriginalEndTimeZone** properties on the **event** resource to find out the time zone used when the event was created.</span></span>


## <a name="permissions"></a><span data-ttu-id="fd25e-128">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fd25e-128">Permissions</span></span>
<span data-ttu-id="fd25e-p106">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fd25e-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fd25e-131">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd25e-131">Permission type</span></span>      | <span data-ttu-id="fd25e-132">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd25e-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd25e-133">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd25e-133">Delegated (work or school account)</span></span> | <span data-ttu-id="fd25e-134">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fd25e-134">Calendars.Read</span></span>    |
|<span data-ttu-id="fd25e-135">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd25e-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd25e-136">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fd25e-136">Calendars.Read</span></span>    |
|<span data-ttu-id="fd25e-137">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd25e-137">Application</span></span> | <span data-ttu-id="fd25e-138">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fd25e-138">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd25e-139">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd25e-139">HTTP request</span></span>
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
## <a name="optional-query-parameters"></a><span data-ttu-id="fd25e-140">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fd25e-140">Optional query parameters</span></span>
<span data-ttu-id="fd25e-141">Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fd25e-141">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fd25e-142">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd25e-142">Request headers</span></span>
| <span data-ttu-id="fd25e-143">Name</span><span class="sxs-lookup"><span data-stu-id="fd25e-143">Name</span></span>       | <span data-ttu-id="fd25e-144">Typ</span><span class="sxs-lookup"><span data-stu-id="fd25e-144">Type</span></span> | <span data-ttu-id="fd25e-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd25e-145">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fd25e-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd25e-146">Authorization</span></span>  | <span data-ttu-id="fd25e-147">string</span><span class="sxs-lookup"><span data-stu-id="fd25e-147">string</span></span>  | <span data-ttu-id="fd25e-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fd25e-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fd25e-150">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="fd25e-150">Prefer: outlook.timezone</span></span> | <span data-ttu-id="fd25e-151">string</span><span class="sxs-lookup"><span data-stu-id="fd25e-151">string</span></span> | <span data-ttu-id="fd25e-152">Die Standardzeitzone für Ereignisse in der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fd25e-152">The default time zone for events in the response.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd25e-153">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd25e-153">Request body</span></span>
<span data-ttu-id="fd25e-154">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fd25e-154">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd25e-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd25e-155">Response</span></span>

<span data-ttu-id="fd25e-156">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [event](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd25e-156">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd25e-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd25e-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd25e-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd25e-158">Request</span></span>
<span data-ttu-id="fd25e-p108">Im erste Beispiel wird das angegebene Ereignis abgerufen. Es gibt Folgendes an:</span><span class="sxs-lookup"><span data-stu-id="fd25e-p108">The first example gets the specified event. It specifies the following:</span></span>

- <span data-ttu-id="fd25e-161">Einen `Prefer: outlook.timezone`-Header zum Abrufen von Datums- und Uhrzeitwerten in 	Pacific Normalzeit.</span><span class="sxs-lookup"><span data-stu-id="fd25e-161">A `Prefer: outlook.timezone` header to get date time values returned in Pacific Standard Time.</span></span> 
- <span data-ttu-id="fd25e-p109">Einen `$select`-Abfrageparameter zum Zurückgeben bestimmter Eigenschaften. Ohne `$select`-Parameter werden alle Ereigniseigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd25e-p109">A `$select` query parameter to return specific properties. Without a `$select` parameter, all of the event properties will be returned.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_event"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGIAAAoZDOFAAA=')?$select=subject,body,bodyPreview,organizer,attendees,start,end,location 
Prefer: outlook.timezone="Pacific Standard Time"
```

##### <a name="response"></a><span data-ttu-id="fd25e-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd25e-164">Response</span></span>

<span data-ttu-id="fd25e-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Die **body**-Eigenschaft wird im HTML-Standardformat zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd25e-p110">Here is an example of the response. The **body** property is returned in the default format of HTML.</span></span>

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
```

## <a name="see-also"></a><span data-ttu-id="fd25e-167">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="fd25e-167">See also</span></span>

- [<span data-ttu-id="fd25e-168">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="fd25e-168">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="fd25e-169">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="fd25e-169">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
