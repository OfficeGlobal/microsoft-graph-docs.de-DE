# <a name="update-event"></a>Ereignis aktualisieren

Mit dieser API können Sie die Eigenschaften eines Ereignisobjekts aktualisieren.
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Calendars.ReadWrite    |
|Delegiert (persönliches Microsoft-Konto) | Calendars.ReadWrite    |
|Anwendung | Calendars.ReadWrite |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/events/{id}
PATCH /users/{id | userPrincipalName}/events/{id}
PATCH /groups/{id}/events/{id}

PATCH /me/calendar/events/{id}
PATCH /users/{id | userPrincipalName}/calendar/events/{id}
PATCH /groups/{id}/calendar/events/{id}

PATCH /me/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendars/{id}/events/{id}

PATCH /me/calendargroup/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}

PATCH /me/calendargroups/{id}/calendars/{id}/events/{id}
PATCH /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|attendees|[Teilnehmer](../resources/attendee.md)|Die Sammlung der Teilnehmer für das Ereignis.|
|body|[ItemBody](../resources/itembody.md)|Der Text der Nachricht, die mit diesem Ereignis verknüpft ist.|
|categories|String|Die Kategorien, die mit dem Ereignis verknüpft sind.|
|end|[DateTimeTimeZone](../resources/datetimetimezone.md)|Datum und Uhrzeit für das Ende des Ereignisses.<br/><br/>Standardmäßig ist die Endzeit in UTC angegeben. Sie können eine optionale Zeitzone in EndTimeZone angeben, die Endzeit in dieser Zeitzone angeben und einen Zeitunterschied zur UTC-Zeitzone angeben. Beachten Sie, dass bei Verwendung von EndTimeZone auch ein Wert für StartTimeZone angegeben werden muss.<br/><br/>In diesem Beispiel wird der 25. Februar 2015 21:34 in PST angegeben: „2015-02-25T21:34:00-08:00“. |
|Wichtigkeit|String|Die Wichtigkeit des Ereignisses. Niedrig = 0, Normal = 1, Hoch = 2. Mögliche Werte: `Low`, `Normal`, `High`.|
|isAllDay|Boolean|True, wenn das Ereignis den ganzen Tag andauert.|
|isReminderOn|Boolean|True, wenn eine Benachrichtigung den Benutzer an das Ereignis erinnern soll.|
|location|[Ort](../resources/location.md)|Der Ort des Ereignisses.|
|onlineMeetingUrl|String|Eine URL für eine Onlinebesprechung.|
|recurrence|[PatternedRecurrence](../resources/patternedrecurrence.md)|Das Serienmuster für das Ereignis.|
|reminderMinutesBeforeStart|Int32|Festlegung, wie viele Minuten vor Beginn des Ereignisses die Erinnerung angezeigt werden soll|
|responseRequested|Boolean|Legen Sie „True“ fest, wenn der Absender eine Antwort erhalten soll, wenn das Ereignis akzeptiert oder abgelehnt wird.|
|sensitivity|String| Mögliche Werte: `Normal`, `Personal`, `Private`, `Confidential`.|
|showAs|Zeichenfolge|Der anzuzeigende Status. Mögliche Werte: `Free`, `Tentative`, `Busy`, `Oof`, `WorkingElsewhere`, `Unknown`.|
|start|[DateTimeTimeZone](../resources/datetimetimezone.md)|Die Startzeit des Ereignisses. <br/><br/>Standardmäßig ist die Startzeit in UTC angegeben. Sie können eine optionale Zeitzone in StartTimeZone angeben, die Startzeit in dieser Zeitzone angeben und einen Zeitunterschied zur UTC-Zeitzone angeben. Beachten Sie, dass bei Verwendung von StartTimeZone auch ein Wert für EndTimeZone angegeben werden muss.<br/><br/>In diesem Beispiel wird 25. Februar 2015 19:34 in PST angegeben: „2015-02-25T19:34:00-08:00“.  |
|subject|String|Der Text der Betreffzeile des Ereignisses|

Da die **event**-Ressource [Erweiterungen](../../../concepts/extensibility_overview.md) unterstützt, erlaubt der `PATCH`-Vorgang das Hinzufügen, Aktualisieren oder Löschen eigener App-spezifischer Daten in den benutzerdefinierten Eigenschaften von Erweiterungen in vorhandenen **event**-Instanzen.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [vent](../resources/event.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "datetime-value"
  },
  "recurrence": null,
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
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
  "recurrence": null,  
  "iCalUId": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
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
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
