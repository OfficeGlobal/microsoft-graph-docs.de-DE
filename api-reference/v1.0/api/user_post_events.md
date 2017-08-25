# <a name="create-event"></a><span data-ttu-id="e98ee-101">Ereignis erstellen</span><span class="sxs-lookup"><span data-stu-id="e98ee-101">Create Event</span></span>

<span data-ttu-id="e98ee-102">Erstellen eines [Ereignisses](../resources/event.md) im Standardkalender des Benutzers oder in einem angegebenen Kalender.</span><span class="sxs-lookup"><span data-stu-id="e98ee-102">Create an [event](../resources/event.md) in the user's default calendar or specified calendar.</span></span>

<span data-ttu-id="e98ee-103">Sie können die Zeitzone für alle Start- und Endzeiten des Ereignisses als Teil dieser Werte angeben, da die **start**- und **end**-Eigenschaft vom Typ [dateTimeTimeZone](../resources/datetimetimezone.md) sind.</span><span class="sxs-lookup"><span data-stu-id="e98ee-103">You can specify the time zone for each of the start and end times of the event as part of these values, as the **start** and **end** properties are of [dateTimeTimeZone](../resources/datetimetimezone.md) type.</span></span> 

<span data-ttu-id="e98ee-104">Wenn das Ereignis erstellt wird, sendet der Server Einladungen an alle Teilnehmer.</span><span class="sxs-lookup"><span data-stu-id="e98ee-104">When the event is created, the server send invitations to all attendees.</span></span>


## <a name="permissions"></a><span data-ttu-id="e98ee-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e98ee-105">Permissions</span></span>
<span data-ttu-id="e98ee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e98ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e98ee-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e98ee-108">Permission type</span></span>      | <span data-ttu-id="e98ee-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e98ee-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="e98ee-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e98ee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e98ee-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e98ee-111">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="e98ee-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e98ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e98ee-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e98ee-113">Calendars.ReadWrite</span></span>    | 
|<span data-ttu-id="e98ee-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e98ee-114">Application</span></span> | <span data-ttu-id="e98ee-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e98ee-115">Calendars.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e98ee-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e98ee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/events
POST /users/{id | userPrincipalName}/events

POST /me/calendar/events
POST /users/{id | userPrincipalName}/calendar/events

POST /me/calendars/{id}/events
POST /users/{id | userPrincipalName}/calendars/{id}/events
```
## <a name="request-headers"></a><span data-ttu-id="e98ee-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e98ee-117">Request headers</span></span>
| <span data-ttu-id="e98ee-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e98ee-118">Header</span></span>       | <span data-ttu-id="e98ee-119">Wert</span><span class="sxs-lookup"><span data-stu-id="e98ee-119">Value</span></span> |
|:-----------|:------|
| <span data-ttu-id="e98ee-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e98ee-120">Authorization</span></span>  | <span data-ttu-id="e98ee-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e98ee-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e98ee-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e98ee-123">Content-Type</span></span>  | <span data-ttu-id="e98ee-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="e98ee-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e98ee-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e98ee-126">Request body</span></span>
<span data-ttu-id="e98ee-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e98ee-127">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

<span data-ttu-id="e98ee-128">Da die **event**-Ressource [Erweiterungen](../../../concepts/extensibility_overview.md) unterstützt, können Sie den `POST`-Vorgang verwenden und während der Erstellung des Ereignisses benutzerdefinierte Eigenschaften mit Ihren eigenen Daten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="e98ee-128">Since the **event** resource supports [extensions](../../../concepts/extensibility_overview.md), you can use the `POST` operation and add custom properties with your own data to the event while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="e98ee-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e98ee-129">Response</span></span>

<span data-ttu-id="e98ee-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und ein [event](../resources/event.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e98ee-130">If successful, this method returns `201, Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e98ee-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e98ee-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e98ee-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e98ee-132">Request</span></span>
<span data-ttu-id="e98ee-p104">Nachfolgend sehen Sie ein Beispiel der Anforderung. Es verwendet den `Prefer: outlook.timezone`-Anforderungsheader, um die **Start**- und **End**zeiten in der Antwort anzugeben, die in dieser Zeitzone verwendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="e98ee-p104">Here is an example of the request. It uses the `Prefer: outlook.timezone` request header to specify the **start** and **end** times in the response should use that time zone.</span></span>
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
        "address":"fannyd@contoso.onmicrosoft.com",
        "name": "Fanny Downs"
      },
      "type": "required"
    }
  ]
}
```
<span data-ttu-id="e98ee-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [event](../resources/event.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e98ee-135">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e98ee-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="e98ee-136">Response</span></span>
<span data-ttu-id="e98ee-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e98ee-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
                "name":"Fanny Downs",
                "address":"fannyd@contoso.onmicrosoft.com"
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
## <a name="see-also"></a><span data-ttu-id="e98ee-140">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="e98ee-140">See also</span></span>

- [<span data-ttu-id="e98ee-141">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="e98ee-141">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="e98ee-142">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="e98ee-142">Add custom data to users using open extensions (preview)</span></span>](../../../concepts/extensibility_open_users.md)
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
