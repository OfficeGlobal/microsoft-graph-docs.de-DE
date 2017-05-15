# <a name="list-events"></a>Ereignisse auflisten

Dient zum Abrufen einer Liste der [event](../resources/event.md)-Objekte im Postfach des Benutzers. Die Liste enthält einzelne Instanzen von Besprechungen und Serienmaster.

Zurzeit gibt dieser Vorgang Ereignistext nur im HTML-Format zurück.

Um erweiterte Ereignisinstanzen abzurufen, können Sie [die Kalenderansicht abrufen](calendar_list_calendarview.md) oder [die Instanzen eines Ereignisses abrufen](event_list_instances.md).

### <a name="support-various-time-zones"></a>Unterstützen verschiedener Zeitzonen

Für alle GET-Vorgänge, die Ereignisse zurückgeben, können Sie den `Prefer: outlook.timezone`-Header zum Angeben der Zeitzone für die Anfangs- und Endzeit des Ereignisses in der Antwort verwenden. 

Mit dem folgenden `Prefer: outlook.timezone`-Header werden zum Beispiel die Anfangs- und Endzeiten in der Antwort auf EST festgelegt.
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

Wenn das Ereignis in einer anderen Zeitzone erstellt wurde, werden die Anfangs- und Endzeiten an die in diesem `Prefer`-Header angegebene Zeitzone angepasst. Die unterstützten Zeitzonen finden Sie in dieser [Liste](../resources/datetimetimezone.md). Wenn der `Prefer: outlook.timezone`-Header nicht angegeben ist, werden die Anfangs- und Endzeiten in UTC zurückgegeben.

Sie können die **OriginalStartTimeZone**- und **OriginalEndTimeZone**-Eigenschaften für die **event**-Ressource verwenden, um die beim Erstellen des Ereignisses verwendete Zeitzone abzurufen.

## <a name="prerequisites"></a>Voraussetzungen
Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Calendars.Read; Calendars.ReadWrite*
## <a name="http-request"></a>HTTP-Anforderung
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
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer <token>. Required. |
| Prefer: outlook.timezone | string | Die Standardzeitzone für Ereignisse in der Antwort. Optional. | 

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.
## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung. Es gibt Folgendes an:

- Einen `Prefer: outlook.timezone`-Header zum Abrufen von Datums- und Uhrzeitwerten in 	Pacific Normalzeit. 
- Einen `$select`-Abfrageparameter zum Zurückgeben bestimmter Eigenschaften. Ohne `$select`-Parameter werden alle Ereigniseigenschaften zurückgegeben.

<!-- {
  "blockType": "request",
  "name": "get_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events?$select=subject,body,bodyPreview,organizer,attendees,start,end,location
Prefer: outlook.timezone="Pacific Standard Time"
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Die **body**-Eigenschaft wird im HTML-Standardformat zurückgegeben.
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
