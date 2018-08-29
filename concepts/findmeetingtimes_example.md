# <a name="find-possible-meeting-times-on-the-outlook-calendar"></a>Suchen nach möglichen Besprechungszeiten im Outlook-Kalender

In einem Unternehmen oder einer Schule oder Universität ist die Suche nach einer gemeinsamen Zeit und einem Ort für eine Besprechung häufig mit Mehraufwand verbunden. Microsoft Graph-Anwendungen können [findMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) verwenden, um alle möglichen Besprechungszeiten zu ermitteln, die Einschränkungen bzgl. Uhrzeit, Ort und anderen Aspekten erfüllen.   

Mit der Aktion **findMeetingTimes** können Sie Bedingungen wie z. B. den Datums-/Uhrzeitbereich, die Dauer, optionale oder erforderliche Teilnehmer für die Besprechung und die Art der Aktivität (**activityDomain**) angeben. Die Aktion berücksichtigt die normalen Arbeitszeitpläne und den Frei-/Gebucht-Status der Teilnehmer und des Organisators und schlägt Zeiten vor, die für die Teilnehmer und den Typ der Aktivität geeignet sind. So beziehen sich Vorschläge für eine arbeitsbezogene Aktivität immer auf die Arbeitszeiten des Organisators und der Teilnehmer; außerdem werden vorgeschlagene Zeiten, zu denen die erforderlichen Teilnehmer verfügbar sind, weiter oben in der Liste mit Vorschlägen einsortiert.

In Office 365 können Arbeitszeiten und Zeitzonen für jedes Postfach konfiguriert werden. Die Aktion **findMeetingTimes** berücksichtigt auch Zeitzonenunterschiede zwischen Organisator und Teilnehmern. Standardmäßig gibt **findMeetingTimes** Vorschläge in UTC zurück. Sie können den folgenden Anforderungsheader verwenden, damit **findMeetingTimes** Vorschläge in einer bestimmten Zeitzone ausgedrückt zurückgibt.
```
Prefer: outlook.timezone="{time-zone-string}}"
```

Besonders hilfreich für größere Besprechungen ist, dass Sie einen Prozentsatz (**minimumAttendeePercentage**) für ein Quorum angeben können, sodass **findMeetingTimes** nur Vorschläge zurückgibt, wenn diese minimale Teilnehmerzahl verfügbar ist.

Wenn **findMeetingTimes** keine Besprechungszeiten vorgeschlagen kann, wird ein bestimmter Grund (**emptySuggestionsReason**) angegeben, z. B. dass der Organisator oder ein erforderlicher Teilnehmer nicht verfügbar ist. Ausgehend von diesem Wert können Sie die Parameter optimieren und **findMeetingTimes** erneut aufrufen.

>**Hinweis** Die Aktion **findMeetingTimes** ist derzeit für Office 365-Geschäfts-, -Schul- oder -Unipostfächer, aber nicht für persönliche outlook.com-Postfächer verfügbar.

## <a name="example"></a>Beispiel

Das folgende Beispiel zeigt, wie Sie **findMeetingTimes** verwenden, um mögliche Zeiten für eine zweistündige Besprechung von zwei Benutzern zurückzugeben, wobei der Frei-/Gebucht-Status und die Arbeitszeitpläne der Benutzer und die teilweise Abwesenheit des Teilnehmer berücksichtigt werden. Da nur zwei Benutzer an dieser Besprechung teilnehmen sollen, ist für Vorschläge eine Anwesenheit von 100 % erforderlich. Die folgende Abbildung zeigt den Frei-/Gebucht-Zeitplan der Benutzer.

### <a name="organizers-calendar"></a>Kalender des Organisators

![Der Arbeitskalender des Organisators für den 17. bis 21. April mit Frei-/Gebucht-Zeiten](./images/findmeetingtimes_organizer_free_busy.jpg "Der Arbeitskalender des Organisators für den 17. bis 21. April mit Frei/-Gebucht-Zeiten")

### <a name="attendees-calendar"></a>Kalender des Teilnehmers

![Der Arbeitskalender des Teilnehmers für den 17. bis 21. April mit Frei-/Gebucht-Zeiten](./images/findmeetingtimes_attendee_free_busy.jpg "Der Arbeitskalender des Teilnehmers für den 17. bis 21. April mit Frei-/Gebucht-Zeiten")

Im Beispiel wird **findMeetingTimes** zwei Mal aufgerufen:

1. Der erste Aufruf sucht im Datumsbereich vom 18. bis 20. April. Da der Teilnehmer am 18. und 19. April abwesend ist und es keine gemeinsame verfügbare Zeit am 20. April gibt, gibt der erste Aufruf keine Vorschläge zurück und begründet es damit, dass die Teilnehmer nicht verfügbar sind (**emptySuggestionsReason**).
2. Der zweite Aufruf sucht nach Verfügbarkeit am 21. April und gibt als Vorschlag den Zeitraum zwischen 14:00 und 16:00 Uhr zurück.

Die beiden Aufrufe von **findMeetingTimes** enthalten die folgenden Parameter. Alle [Parameter](../api-reference/v1.0/api/user_findmeetingtimes.md#request-body) für **findMeetingTimes** sind optional.

- **attendees**: ein Teilnehmer, Samantha Booth; die Eigenschaft **type** ist auf `required` festgelegt.
- **timeConstraint**: kein Ortsvorschlag erforderlich.
- **timeConstraint**: Der erste Aufruf sucht im Datums-/Uhrzeitbereich vom 18. April, 9:00 Uhr bis zum 20. April, 17:00 Uhr; nachdem der erste Aufruf keine Zeiten vorschlagen kann, untersucht der zweite Aufruf den 21. April zwischen 9:00 und 17:00 Uhr.
- **meetingDuration**: zwei Stunden.
- **returnSuggestionReasons**: In diesem Beispiel muss ein Grund für jeden Vorschlag angegeben werden.
- **minimumAttendeePercentage**: 100 %, da der Teilnehmer zu jeder vorgeschlagenen Zeit verfügbar sein muss.

### <a name="first-request"></a>Erste Anforderung

Nach einem freien, zweistündigen Zeitfenster für beide Benutzer zwischen dem 18. und 20. April suchen.

<!-- {
  "blockType": "ignored",
  "name": "findmeetingtimes_example_first"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/findMeetingTimes
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com" 
      } 
    }
  ],  
  "locationConstraint": { 
    "isRequired": false,  
    "suggestLocation": false,  
    "locations": [ 
      { 
        "resolveAvailability": false,
        "displayName": "Conf room Hood" 
      } 
    ] 
  },  
  "timeConstraint": {
    "activityDomain":"work", 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2017-04-18T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2017-04-20T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": true,
  "minimumAttendeePercentage": 100
}
```

### <a name="first-response"></a>Erste Antwort
Es gibt kein zweistündiges Zeitfenster während der Arbeitszeiten vom 18. bis 20. April, in dem beide Benutzer verfügbar sind.
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-Length: 184

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
    "emptySuggestionsReason":"AttendeesUnavailable",
    "meetingTimeSuggestions":[

    ]
}
```

### <a name="second-request"></a>Zweite Anforderung
Nach einem zweistündigen Zeitfenster am 21. April suchen.
<!-- {
  "blockType": "ignored",
  "name": "findmeetingtimes_example_second"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/findMeetingTimes
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com" 
      } 
    }
  ],  
  "locationConstraint": { 
    "isRequired": false,  
    "suggestLocation": false,  
    "locations": [ 
      { 
        "resolveAvailability": false,
        "displayName": "Conf room Hood" 
      } 
    ] 
  },  
  "timeConstraint": {
    "activityDomain":"work", 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2017-04-21T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2017-04-21T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": true,
  "minimumAttendeePercentage": 100
}
```

### <a name="second-response"></a>Zweite Antwort
Die zweite **findMeetingTimes**-Anforderung schlägt als Besprechungszeit für beide Benutzer den 21. April von 14:00 bis 16:00 Uhr vor.
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-Length: 714

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
    "emptySuggestionsReason":"",
    "meetingTimeSuggestions":[
        {
            "confidence":100.0,
            "organizerAvailability":"free",
            "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available.",
            "meetingTimeSlot":{
                "start":{
                    "dateTime":"2017-04-21T14:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                },
                "end":{
                    "dateTime":"2017-04-21T16:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                }
            },
            "attendeeAvailability":[
                {
                    "availability":"free",
                    "attendee":{
                        "type":"required",
                        "emailAddress":{
                            "address":"samanthab@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations":[
                {
                    "displayName":"Conf room Hood"
                }
            ]
        }
    ]
}
```



## <a name="next-steps"></a>Nächste Schritte

Es gibt Situationen, in denen nicht alle Teilnehmer an einer Besprechung teilnehmen können. Sie können festlegen, dass **findMeetingTimes** eine Zeit vorschlägt, wenn die _Konfidenz_ für die Anwesenheit einen bestimmten Prozentsatz erreicht, indem Sie den optionalen Parameter **minimumAttendeePercentage** angeben. Erfahren Sie mehr über die [Konfidenz eines Besprechungsvorschlags](../api-reference/v1.0/api/user_findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) und andere [Parameter](../api-reference/v1.0/api/user_findmeetingtimes.md#request-body), und wenden Sie sie nach Bedarf für größere Besprechungen an.

Nachdem Sie Vorschläge für Besprechungszeiten erhalten haben, haben Sie folgende Möglichkeiten:

1. [Termin erstellen und als Besprechungsanfrage senden](../api-reference/v1.0/api/user_post_events.md)
2. Dem Termin [eine Anlage hinzufügen](../api-reference/v1.0/api/event_post_attachments.md)

In diesem Artikel erfahren Sie mehr über die [Integration mit Outlook-Kalender](outlook-calendar-concept-overview.md).
