# <a name="get-freebusy-schedule-for-users-and-resources-preview"></a>Abrufen von Frei/Gebucht-Informationen für Benutzer und Ressourcen (Preview)

In einer Arbeits- oder Schulumgebung ist es üblich, zu schauen, wann ein Benutzer für eine Besprechung frei ist oder die Verfügbarkeit eines Teams, eines Raums oder einer Ausrüstung für einen bestimmten Zeitraum zu überprüfen.

Mit der Aktion [getSchedule](../api-reference/beta/api/calendar_getschedule.md) erhalten Sie die Verfügbarkeitsinformationen einer oder mehrerer Entitäten - Benutzer, Verteilerlisten oder Ressourcen - für einen bestimmten Zeitraum. 

## <a name="example"></a>Beispiel

Ein einfaches Beispiel ist der Frei/Gebucht-Zeitplan eines Mitarbeiters, Alex, an einem bestimmten Tag, von 9 bis 18 Uhr, Pacitfic Standard Time:

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule_concept"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/getschedule 
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{        
    "Schedules": ["AlexW@contoso.OnMicrosoft.com"],
    "StartTime": {
        "dateTime": "2018-08-06T09:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "EndTime": {
        "dateTime": "2018-08-06T18:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "availabilityViewInterval": "15"
}
```

**getSchedule** gibt zwei Zeitplaneinträge zurück, die mit den vorhandenen Ereignissen im Standardkalender von Alex übereinstimmen und die Start- und Endzeiten der einzelnen Ereignisse sowie deren Frei/Gebucht-Status anzeigen. Sie können davon ausgehen, dass Alex für die verbleibende Zeit in diesem Datums-/Zeitbereich frei ist.

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.scheduleInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value":[
        {
            "scheduleId":"AlexW@contoso.OnMicrosoft.com",
            "availabilityView":"111111002222222200000000000000000000",
            "scheduleItems":[
                {
                    "isPrivate":false,
                    "status":"Tentative",
                    "start":{
                        "dateTime":"2018-08-06T09:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T10:30:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                },
                {
                    "isPrivate":false,
                    "status":"Busy",
                    "start":{
                        "dateTime":"2018-08-06T11:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T13:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                }
            ],
            "workingHours":{
                "daysOfWeek":[
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime":"08:00:00.0000000",
                "endTime":"17:00:00.0000000",
                "timeZone":{
                    "@odata.type":"#microsoft.graph.customTimeZone",
                    "bias":480,
                    "name":"Customized Time Zone",
                    "standardOffset":{
                        "time":"02:00:00.0000000",
                        "dayOccurrence":1,
                        "dayOfWeek":"sunday",
                        "month":11,
                        "year":0
                    },
                    "daylightOffset":{
                        "daylightBias":-60,
                        "time":"02:00:00.0000000",
                        "dayOccurrence":2,
                        "dayOfWeek":"sunday",
                        "month":3,
                        "year":0
                    }
                }
            }
        }
    ]
}

```

Abgesehen von dem Frei/Gebucht-Zeitplan und den Arbeitszeiten von Alex gibt **getSchedule** auch **AvailabilityView** zurück. Dabei handelt es sich um eine zusammengefasste Ansicht der Verfügbarkeit von Alex für diesen Tag. Die zusammengeführte Ansicht ist eine Zeichenkette, die aus Zeitfenstern besteht, die diesen Tag abdecken, wobei jedes Zeitfenster die Verfügbarkeit von Alex gemäß der folgenden Konvention anzeigt: 

- `0`= Frei
- `1`= mit Vorbehalt
- `2`= Gebucht
- `3`= Abwesend
- `4`= an anderer Stelle arbeiten. 

Standardmäßig beträgt die Länge der einzelnen Zeitfenster 30 Minuten. Dieses Beispiel verwendet die Eigenschaft **availabilityViewInterval**, um das Zeitfenster auf 15 Minuten einzustellen.

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a>Wie unterscheidet sich getSchedule von findMeetingTimes

Die Aktion [findMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) ähnelt der Aktion **getSchedule**, da sowohl der Frei/Gebucht-Status als auch die Arbeitszeiten der angegebenen Benutzer und Ressourcen ausgelesen werden. Die beiden Aktionen unterscheiden sich in einigen wesentlichen Punkten.

### <a name="application"></a>Anwendung

**findMeetingTimes** wendet bestimmte Geschäftslogiken an, um Besprechungszeiten und -orte vorzuschlagen, wie zum Beispiel:

- Optionale oder obligatorische Teilnahme jeder Entität
- Die Art der gewünschten Aktivität zur Tageszeit
- Die für die Beschlussfähigkeit einer Besprechung erforderliche Mindestteilnehmerzahl

Sie empfiehlt sich für Szenarien, die von der [Optimierung der Terminbuchung](findmeetingtimes_example.md) abhängig sind.

**getSchedule** gibt lediglich den Frei/Gebucht-Status vorhandener Ereignisse in jedem der angeforderten Kalender für einen bestimmten Zeitraum zurück und nimmt an, dass die restliche Zeit in diesem Zeitraum TP frei ist. Um diese Daten zur Vervollständigung Ihres Szenarios zu nutzen, wenden Sie weitere Geschäftslogiken an.

### <a name="app-only-support"></a>Nur-App-Support

**findmeetingtimes** unterstützt nur solche delegierten Szenarien, bei denen ein Benutzer sich in der App angemeldet haben muss. Die App kann Ereignisse nur in den Kalendern lesen, auf die der angemeldete Benutzer zugreifen kann. Dies kann Kalender beinhalten, die andere Benutzer delegiert oder mit dem angemeldeten Benutzer geteilt haben.

**getSchedule** unterstützt sowohl delegierte als auch Nur-App-Szenarien. Im letzteren Fall erteilt ein Administrator der App die Erlaubnis, den Zugriff auf alle Kalender ohne angemeldeten Benutzer.


### <a name="version-support"></a>Versionsunterstützung

**findmeetingtimes** ist in der Regel für alle Apps verfügbar. 

**getSchedule** ist derzeit [in der Vorschauversion](versioning_and_support.md#beta-version) verfügbar und daher nicht für den Einsatz in Produktivanwendungen geeignet.


## <a name="permissions"></a>Berechtigungen
Die niedrigste Berechtigung, die Sie benötigen, um Frei/Gebucht-Informationen zu erhalten, ist Calendar.Read. Abhängig von Ihrem App-Szenario kann dies vom angemeldeten Benutzer oder Administrator genehmigt werden.
Abgesehen vom Frei/Gebucht-Status und den Arbeitszeiten der angeforderten Entitäten kann **getSchedule** auch den Inhalt und den Ort eines Ereignisses unter folgenden Bedingungen zurückgeben:

- Wenn das Ereignis mit niedriger Vertraulichkeitsstufe gekennzeichnet ist - `normal` oder `personal` UND eine oder mehrere der folgenden Bedingungen zutrifft/zutreffen:

- Die Kalendereinstellungen des angeforderten Benutzers erlauben es allen Benutzern in der Organisation, Titel und Orte anzuzeigen
- Der Kalender des angeforderten Benutzers wird mit dem angemeldeten Benutzer geteilt
- Der angemeldete Benutzer ist ein Administrator der gleichen Organisation wie der angeforderte Benutzer.

## <a name="time-zone-representation"></a>Zeitzonendarstellung
Standardmäßig werden die Anfangs- und Endzeiten der zurückgegebenen Elemente des Zeitplans in UTC dargestellt. Sie können einen `Prefer` Header verwenden, um eine für Ihre App passende Zeitzone anzugeben. Dazu folgendes Beispiel: 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a>Grenzwerte und Fehlerzustände
Beachten Sie die folgenden Grenzwerte und Fehlerzustände:

- **getSchedule** unterstützt die Suche nach Frei/Gebucht-Informationen für bis zu 20 Objekte gleichzeitig. Diese Begrenzung gilt sowohl für die Anzahl der einzeln oder als Mitglieder einer Verteilerliste identifizierten Benutzer als auch für die Anzahl der Ressourcen.
- Der Suchzeitraum muss weniger als 42 Tage betragen.
- Wenn **getSchedule** einen bestimmten Benutzer oder eine bestimmte Ressource nicht identifizieren kann, wird ein einzelnes Zeitplan-Element zurückgegeben und der Fehler angezeigt. 

## <a name="see-also"></a>Siehe auch
- [Verweis auf Berechtigungen](permissions_reference.md#calendars-permissions)
- [Suchen nach möglichen Besprechungszeiten im Outlook-Kalender](findmeetingtimes_example.md)
