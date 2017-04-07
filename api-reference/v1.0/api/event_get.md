# <a name="get-event"></a>Ereignis abrufen

Dient zum Abrufen der Eigenschaften und der Beziehungen des angegebenen [event](../resources/event.md)-Objekts.

Für alle GET-Vorgänge, die Ereignisse zurückgeben, können Sie den `Prefer: outlook.timezone`-Header zum Angeben der Zeitzone für die Anfangs- und Endzeit des Ereignisses in der Antwort verwenden. 

Mit dem folgenden `Prefer: outlook.timezone`-Header werden zum Beispiel die Anfangs- und Endzeiten in der Antwort auf EST festgelegt.
```http
Prefer: outlook.timezone="Eastern Standard Time"
```

Wenn das Ereignis in einer anderen Zeitzone erstellt wurde, werden die Anfangs- und Endzeiten an die in diesem `Prefer`-Header angegebene Zeitzone angepasst. Die unterstützten Zeitzonen finden Sie in dieser [Liste](../resources/datetimetimezone.md). Wenn der `Prefer: outlook.timezone`-Header nicht angegeben ist, werden die Anfangs- und Endzeiten in UTC zurückgegeben.

Sie können die **OriginalStartTimeZone**- und **OriginalEndTimeZone**-Eigenschaften für die **event**-Ressource verwenden, um die beim Erstellen des Ereignisses verwendete Zeitzone abzurufen.

Da die **event**-Ressource [Erweiterungen](../../../concepts/extensibility_overview.md) unterstützt, können Sie über den `GET`-Vorgang auch benutzerdefinierte Eigenschaften und Erweiterungsdaten aus **event**-Instanzen abrufen.

## <a name="prerequisites"></a>Voraussetzungen
Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Calendars.Read*
## <a name="http-request"></a>HTTP-Anforderung
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
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer <token>. Required. |
| Prefer: | outlook.timezone | Die Standardzeitzone für Ereignisse in der Antwort. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.
## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [event](../resources/event.md)-Objekt im Antworttext zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_event"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/events/{id}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true,
  "start": {
    "dateTime": "datetime-value",
    "timeZone": "timezone-value"
  },
  "end": {
    "dateTime": "datetime-value",
    "timeZone": "timezone-value"
  },        
  "location": {
    "displayName": "displayName-value"
  },
  "organizer": {
    "emailAddress": {
      "address": "address-value",
      "name": "name-value"
    }
  }
}
```

## <a name="see-also"></a>Weitere Artikel

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](../../../concepts/extensibility_overview.md)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)](../../../concepts/extensibility_open_users.md)
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
