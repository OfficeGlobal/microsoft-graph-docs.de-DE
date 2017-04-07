# <a name="user-reminderview"></a>user: reminderView
Gibt eine Liste von Kalendererinnerungen innerhalb der angegebenen Start- und Endzeiten zurück. 

## <a name="prerequisites"></a>Voraussetzungen
Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Calendars.Read; Calendars.ReadWrite*
## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/reminderView(startDateTime=startDateTime-value,endDateTime=endDateTime-value)
```

## <a name="function-parameters"></a>Funktionsparameter
Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.

| Parameter       | Typ    |Beschreibung|
|:---------------|:--------|:----------|
|startDateTime|String|Das Startdatum und die Uhrzeit des Ereignisses, für das die Erinnerung eingerichtet ist. Der Wert wird im ISO 8601-Format dargestellt, z. B. „2015-11-08T19:00:00.0000000“.|
|endDateTime|String|Das Enddatum und die Uhrzeit des Ereignisses, für das die Erinnerung eingerichtet ist. Der Wert wird im ISO 8601-Format dargestellt, z. B. „2015-11-08T20:00:00.0000000“.|


## <a name="request-headers"></a>Anforderungsheader
| Kopfzeile       | Wert|
|:-----------|:------|
| Authorization  | Bearer <token>. Required.  |
| Content-Type   | application/json |
| Prefer | <Zeitzone>. Optional. Falls kein Wert vorhanden, wird UTC angenommen.| 

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200, OK` und das [reminder](../resources/reminder.md)-Sammlungsobjekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel
Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "user_reminderview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/reminderView?startDateTime=startDateTime-value&endDateTime=endDateTime-value
```

##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.reminder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 673

{
  "value": [
    {
      "eventId": "eventId-value",
      "eventStartTime": {
        "dateTime": "dateTime-value",
        "timeZone": "timeZone-value"
      },
      "eventEndTime": {
        "dateTime": "dateTime-value",
        "timeZone": "timeZone-value"
      },
      "changeKey": "changeKey-value",
      "eventSubject": "eventSubject-value",
      "eventLocation": {
        "displayName": "displayName-value",
        "address": {
          "street": "street-value",
          "city": "city-value",
          "state": "state-value",
          "countryOrRegion": "countryOrRegion-value",
          "postalCode": "postalCode-value"
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
  "description": "user: reminderView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
