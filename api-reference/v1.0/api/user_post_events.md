# <a name="create-event"></a><span data-ttu-id="d2ab0-101">Ereignis erstellen</span><span class="sxs-lookup"><span data-stu-id="d2ab0-101">Create Event</span></span>

<span data-ttu-id="d2ab0-102">Erstellen eines [Ereignisses](../resources/event.md) im Standardkalender des Benutzers oder in einem angegebenen Kalender.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-102">Create an [event](../resources/event.md) in the user's default calendar or specified calendar.</span></span>

<span data-ttu-id="d2ab0-103">Sie können die Zeitzone für alle Start- und Endzeiten des Ereignisses als Teil dieser Werte angeben, da die **start**- und **end**-Eigenschaft vom Typ [dateTimeTimeZone](../resources/datetimetimezone.md) sind.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-103">You can specify the time zone for each of the start and end times of the event as part of these values, as the **start** and **end** properties are of [dateTimeTimeZone](../resources/datetimetimezone.md) type.</span></span> 

<span data-ttu-id="d2ab0-104">Wenn ein Ereignis gesendet wird, sendet der Server Einladungen an alle Teilnehmer.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-104">When an event is sent, the server sends invitations to all the attendees.</span></span>

<span data-ttu-id="d2ab0-105">**Festlegen des Ortes in einer Einladung**</span><span class="sxs-lookup"><span data-stu-id="d2ab0-105">**Setting the location in an event**</span></span>

<span data-ttu-id="d2ab0-106">Ein Exchange-Administrator kann ein Postfach und eine E-Mail-Adresse für eine Ressource, z. B. einen Besprechungsraum, oder Geräte, z B. einen Projektor, einrichten.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-106">An Exchange administrator can set up a mailbox and an email address for a resource such as a meeting room, or equipment like a projector.</span></span> <span data-ttu-id="d2ab0-107">Benutzer können die Ressource als Teilnehmer zu einer Besprechung einladen.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-107">Users can then invite the resource as an attendee to a meeting.</span></span> <span data-ttu-id="d2ab0-108">Der Server akzeptiert im Auftrag der Ressource die Besprechungsanfrage basierend auf dem Frei/Gebucht-Zeitplan der Ressource oder lehnt diese ab.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-108">On behalf of the resource, the server accepts or rejects the meeting request based on the free/busy schedule of the resource.</span></span> <span data-ttu-id="d2ab0-109">Wenn der Server eine Besprechung für die Ressource akzeptiert, wird ein Ereignis für die Besprechung im Kalender der Ressource erstellt.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-109">If the server accepts a meeting for the resource, it creates an event for the meeting in the resource's calendar.</span></span> <span data-ttu-id="d2ab0-110">Wenn die Besprechung neu geplant wird, aktualisiert der Server das Ereignis im Kalender der Ressource automatisch.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-110">If the meeting is rescheduled, the server automatically updates the event in the resource's calendar.</span></span>

<span data-ttu-id="d2ab0-111">Ein weiterer Vorteil beim Einrichten eines Postfachs für eine Ressource ist das Steuern des Zeitplans der Ressource derart, dass z. B. nur Führungskräfte oder deren Stellvertretungen einen privaten Besprechungsraum buchen können.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-111">Another advantage of setting up a mailbox for a resource is to control scheduling of the resource, for example, only executives or their delegates can book a private meeting room.</span></span>

<span data-ttu-id="d2ab0-112">Gehen Sie folgendermaßen vor, wenn Sie ein Ereignis organisieren, bei dem ein Besprechungsort vorhanden ist:</span><span class="sxs-lookup"><span data-stu-id="d2ab0-112">If you're organizing an event that involves a meeting location:</span></span>

1. <span data-ttu-id="d2ab0-113">Legen Sie die **location**-Eigenschaft des **Ereignisses** entsprechend fest.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-113">Set the **location** property of the **event** accordingly.</span></span> 
2. <span data-ttu-id="d2ab0-114">Legen Sie die optionale **locationEmailAddress**-Eigenschaft fest, wenn der Besprechungsort eine E-Mail-Adresse aufweist.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-114">Set the optional **locationEmailAddress** property if the meeting location has an email address.</span></span>

<span data-ttu-id="d2ab0-115">Führen Sie die folgenden zusätzlichen Schritte aus, wenn der Besprechungsort als Ressource eingerichtet wurde oder wenn das Ereignis Geräte umfasst, die als Ressource eingerichtet wurden:</span><span class="sxs-lookup"><span data-stu-id="d2ab0-115">Additionally, if the meeting location has been set up as a resource, or if the event involves some equipment that has been set up as a resource:</span></span>

3. <span data-ttu-id="d2ab0-116">Laden Sie die Ressource als [Teilnehmer](../resources/attendee.md) ein.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-116">Invite the resource as an [attendee](../resources/attendee.md).</span></span>
4. <span data-ttu-id="d2ab0-117">Legen Sie die **type**-Eigenschaft des Teilnehmers auf `resource` fest.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-117">Set the attendee **type** property as `resource`.</span></span>
5. <span data-ttu-id="d2ab0-118">Legen Sie die **emailAddress** des Teilnehmers als E-Mail-Adresse der Ressource fest.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-118">Set the attendee **emailAddress** as the resource email address.</span></span>



## <a name="permissions"></a><span data-ttu-id="d2ab0-119">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d2ab0-119">Permissions</span></span>
<span data-ttu-id="d2ab0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d2ab0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d2ab0-122">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d2ab0-122">Permission type</span></span>      | <span data-ttu-id="d2ab0-123">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d2ab0-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2ab0-124">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d2ab0-124">Delegated (work or school account)</span></span> | <span data-ttu-id="d2ab0-125">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2ab0-125">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d2ab0-126">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d2ab0-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2ab0-127">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2ab0-127">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="d2ab0-128">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d2ab0-128">Application</span></span> | <span data-ttu-id="d2ab0-129">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d2ab0-129">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2ab0-130">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d2ab0-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="d2ab0-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d2ab0-131">Request headers</span></span>
| <span data-ttu-id="d2ab0-132">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d2ab0-132">Header</span></span>       | <span data-ttu-id="d2ab0-133">Wert</span><span class="sxs-lookup"><span data-stu-id="d2ab0-133">Value</span></span> |
|:-----------|:------|
| <span data-ttu-id="d2ab0-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2ab0-134">Authorization</span></span>  | <span data-ttu-id="d2ab0-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d2ab0-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2ab0-137">Content-Type</span></span>  | <span data-ttu-id="d2ab0-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="d2ab0-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2ab0-140">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d2ab0-140">Request body</span></span>
<span data-ttu-id="d2ab0-141">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-141">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

<span data-ttu-id="d2ab0-142">Da die **event**-Ressource [Erweiterungen](../../../concepts/extensibility_overview.md) unterstützt, können Sie den `POST`-Vorgang verwenden und während der Erstellung des Ereignisses benutzerdefinierte Eigenschaften mit Ihren eigenen Daten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-142">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="d2ab0-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="d2ab0-143">Response</span></span>

<span data-ttu-id="d2ab0-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [event](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-144">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2ab0-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d2ab0-145">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="d2ab0-146">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="d2ab0-146">Request 1</span></span>
<span data-ttu-id="d2ab0-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-147">Here is an example of the request.</span></span> <span data-ttu-id="d2ab0-148">Es verwendet den `Prefer: outlook.timezone`-Anforderungsheader, um die **Start**- und **End**zeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-148">It uses the `Prefer: outlook.timezone` request header to specify the time zone for the **start** and **end** times in the response.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 600

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
  },
  "start": {
      "dateTime": "2017-04-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-04-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"samanthab@contoso.onmicrosoft.com",
        "name": "Samantha Booth"
      },
      "type": "required"
    }
  ]
}
```
<span data-ttu-id="d2ab0-149">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-149">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-1"></a><span data-ttu-id="d2ab0-150">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="d2ab0-150">Response 1</span></span>
<span data-ttu-id="d2ab0-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2197

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/events/$entity",
    "@odata.etag":"W/\"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==\"",
    "id":"AAMkAGI1AAAt9AHjAAA=",
    "createdDateTime":"2017-04-15T03:00:50.7579581Z",
    "lastModifiedDateTime":"2017-04-15T03:00:51.245372Z",
    "changeKey":"ZlnW4RIAV06KYYwlrfNZvQAALfZeRQ==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "iCalUId":"040000008200E00074C5B7101A82E00800000000DA2B357D94B5D201000000000000000010000000EC4597557F0CB34EA4CC2887EA7B17C3",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "subject":"Let's go brunch",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"singleInstance",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkAGI1AAAt9AHjAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html><head></head><body>Does late morning work for you?</body></html>"
    },
    "start":{
        "dateTime":"2017-04-15T11:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-04-15T12:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location":{
        "displayName":"Harry's Bar"
    },
    "recurrence":null,
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Samantha Booth",
                "address":"samanthab@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Dana Swope",
            "address":"danas@contoso.onmicrosoft.com"
        }
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="d2ab0-154">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="d2ab0-154">Request 2</span></span>
<span data-ttu-id="d2ab0-155">Das zweite Beispiel zeigt, wie ein wiederkehrendes Ereignis erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-155">The second example shows how to create a recurring event.</span></span> <span data-ttu-id="d2ab0-156">Das Ereignis findet jeden Montag von 10:00 Uhr bis 11:00 Uhr beginnend am 4 September 2017 bis zum Jahresende statt.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-156">The event occurs from 10:00am to 11:00am, every Monday starting September 4, 2017, through the end of the year.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_event_recurring"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events
Content-type: application/json

{
  "subject": "Let's go for coffee",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
  },
  "start": {
      "dateTime": "2017-09-04T10:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2017-09-04T11:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "recurrence": {
    "pattern": {
      "type": "weekly",
      "interval": 1,
      "daysOfWeek": [ "Monday" ]
    },
    "range": {
      "type": "endDate",
      "startDate": "2017-09-04",
      "endDate": "2017-12-31"
    }
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"AdeleV@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ]
}
```
<span data-ttu-id="d2ab0-157">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-157">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response-2"></a><span data-ttu-id="d2ab0-158">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="d2ab0-158">Response 2</span></span>
<span data-ttu-id="d2ab0-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d2ab0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "create_event_recurring",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('919717da-0460-4cca-a6be-d25382429896')/events/$entity",
    "@odata.etag":"W/\"+T8RDneHMkKe2BGYEaQZ4wAA7WsvGQ==\"",
    "id":"AAMkADQwMDI5YT",
    "createdDateTime":"2017-10-14T07:37:39.0083072Z",
    "lastModifiedDateTime":"2017-10-14T07:37:40.0239406Z",
    "changeKey":"+T8RDneHMkKe2BGYEaQZ4wAA7WsvGQ==",
    "categories":[

    ],
    "originalStartTimeZone":"Pacific Standard Time",
    "originalEndTimeZone":"Pacific Standard Time",
    "iCalUId":"040000008200E00074C5B7101A82E008000000000068AD4FBF44D301000000000000000010000000CA802EEBDE19CB4AB552714F48C7EEFB",
    "reminderMinutesBeforeStart":15,
    "isReminderOn":true,
    "hasAttachments":false,
    "subject":"Let's go for coffee",
    "bodyPreview":"Does late morning work for you?",
    "importance":"normal",
    "sensitivity":"normal",
    "isAllDay":false,
    "isCancelled":false,
    "isOrganizer":true,
    "responseRequested":true,
    "seriesMasterId":null,
    "showAs":"busy",
    "type":"seriesMaster",
    "webLink":"https://outlook.office365.com/owa/?itemid=AAMkADQwMDI5YT&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl":null,
    "responseStatus":{
        "response":"organizer",
        "time":"0001-01-01T00:00:00Z"
    },
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes late morning work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start":{
        "dateTime":"2017-09-04T10:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "end":{
        "dateTime":"2017-09-04T11:00:00.0000000",
        "timeZone":"Pacific Standard Time"
    },
    "location":{
        "displayName":"Harry's Bar"
    },
    "recurrence":{
        "pattern":{
            "type":"weekly",
            "interval":1,
            "month":0,
            "dayOfMonth":0,
            "daysOfWeek":[
                "monday"
            ],
            "firstDayOfWeek":"sunday",
            "index":"first"
        },
        "range":{
            "type":"endDate",
            "startDate":"2017-09-04",
            "endDate":"2017-12-31",
            "recurrenceTimeZone":"Pacific Standard Time",
            "numberOfOccurrences":0
        }
    },
    "attendees":[
        {
            "type":"required",
            "status":{
                "response":"none",
                "time":"0001-01-01T00:00:00Z"
            },
            "emailAddress":{
                "name":"Adele Vance",
                "address":"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer":{
        "emailAddress":{
            "name":"Alex Wilber",
            "address":"AlexW@contoso.onmicrosoft.com"
        }
    }
}
```


## <a name="see-also"></a><span data-ttu-id="d2ab0-162">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="d2ab0-162">See also</span></span>

- [<span data-ttu-id="d2ab0-163">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="d2ab0-163">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="d2ab0-164">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="d2ab0-164">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
