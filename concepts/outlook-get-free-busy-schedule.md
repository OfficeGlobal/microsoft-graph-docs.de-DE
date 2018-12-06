---
title: Abrufen des Frei/Gebucht-Zeitplans für Benutzer und Ressourcen (Vorschau)
description: Ein häufiges Szenario in einer Arbeits- oder Schulumgebung besteht darin, anzuzeigen, wann ein Benutzer für eine Besprechung verfügbar ist, oder die Verfügbarkeit eines Teams, Raums oder Geräts für einen Zeitraum zu durchsuchen.
ms.openlocfilehash: 8a2dd9318bdd806c99d525ee41f46d78d1963b47
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092304"
---
# <a name="get-freebusy-schedule-of-users-and-resources-preview"></a>Abrufen des Frei/Gebucht-Zeitplans für Benutzer und Ressourcen (Vorschau)

Ein häufiges Szenario in einer Arbeits- oder Schulumgebung besteht darin, anzuzeigen, wann ein Benutzer für eine Besprechung verfügbar ist, oder die Verfügbarkeit eines Teams, Raums oder Geräts für einen Zeitraum zu durchsuchen.

Mit der [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta)-Aktion können Sie die Verfügbarkeitsinformationen einer oder mehrerer Entitäten (Benutzer, Verteilerlisten oder Ressourcen) für einen bestimmten Zeitraum abrufen. 

## <a name="example"></a>Beispiel

Ein einfach Beispiel ist das Suchen des Frei/Gebucht-Zeitplans eines Mitarbeiters Alex an einem bestimmten Tag von 9 Uhr bis 18 Uhr, Pacific Standard Time:

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

**getSchedule** gibt zwei Zeitplanelemente zurück, die vorhandenen Ereignissen in dem Standardkalender von Alex entsprechen; es werden die Start- und Endzeiten der einzelnen Ereignisse sowie der Frei/Gebucht-Status angezeigt. Sie können davon ausgehen, dass Alex die verbleibende Zeit in diesem Datums-/Uhrzeitbereich verfügbar ist.

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

Unabhängig vom Frei/Gebucht-Zeitplan und den Arbeitszeiten von Alex gibt **getSchedule** auch **availabilityView** zurück, eine zusammengeführte Ansicht der Verfügbarkeit von Alex an diesem Tag. Die zusammengeführte Ansicht ist eine Zeichenfolge, die aus Zeitfenstern für diesen Tag besteht; jedes Zeitfenster gibt dabei die Verfügbarkeit von Alex mithilfe der folgenden Konvention an: 

- `0`= frei
- `1`= mit Vorbehalt
- `2`= gebucht
- `3`= abwesend
- `4`= an anderem Ort tätig. 

Standardmäßig beträgt die Länge der einzelnen Zeitfenster 30 Minuten. Dieses Beispiel verwendet die **availabilityViewInterval**-Eigenschaft, um das Zeitfenster auf 15 Minuten zu ändern.

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a>Inwiefern unterscheidet sich getSchedule von FindMeetingTimes?

Die [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0)-Aktion ist dahingehend vergleichbar mit **getSchedule**, dass beide Aktionen den Frei/Gebucht-Status und die Arbeitszeiten der angegebenen Benutzer und Ressourcen lesen. Die beiden Aktionen unterscheiden sich in einigen anderen wichtigen Aspekten.

### <a name="application"></a>Anwendung

**findMeetingTimes** wendet eine bestimmte Geschäftslogik an, um Besprechungszeiten und Orte vorzuschlagen, z. B.:

- Optionale oder obligatorische Teilnahme der einzelnen Entitäten.
- Die Art der angeforderten Aktivität für die Uhrzeit.
- Die Mindestteilnehmeranzahl, die für ein Quorum für eine Besprechung erforderlich ist.

Dies eignet sich für Szenarien, die von [einer optimierten Terminbuchung](findmeetingtimes-example.md) abhängig sind.

**getSchedule** gibt einfach der Frei/Gebucht-Status der vorhandenen Ereignisse in jedem der angeforderten Kalender für einen bestimmten Zeitraum zurück und geht davon aus, dass die verbleibende Zeit in diesem Zeitraum frei ist. Dann wird weitere Geschäftslogik angewendet, um diese Daten zur Vervollständigung Ihres Szenarios zu nutzen.

### <a name="app-only-support"></a>Nur-App-Support

**findmeetingtimes** unterstützt nur delegierte Szenarien, in denen sich ein Benutzer bei der App angemeldet haben muss. Die App kann Ereignisse nur in den Kalendern lesen, auf die der angemeldete Benutzer zugreifen kann. Dazu zählen Kalender, die andere Benutzer delegiert oder für den angemeldeten Benutzer freigegeben haben.

**getSchedule** unterstützt sowohl delegierte als auch Nur-App-Szenarien. Bei letzterem stimmt ein Administrator zu, dass die App auf alle Kalender ohne einen angemeldeten Benutzer zugreift.


### <a name="version-support"></a>Versionsunterstützung

**findmeetingtimes** ist allgemein für alle Apps verfügbar. 

**getSchedule** ist derzeit im [Vorschaustatus](versioning-and-support.md#beta-version) verfügbar und ist daher nicht zur Verwendung in Produktions-Apps geeignet.


## <a name="permissions"></a>Berechtigungen
Calendar.Read ist die niedrigste Berechtigung, die Sie zum Abrufen von Frei/Gebucht-Informationen benötigen. Je nach App-Szenario kann der angemeldete Benutzer oder der Administrator zustimmen.
Neben dem Frei/Gebucht-Status und den Arbeitszeiten der angeforderten Entitäten kann **getSchedule** unter den folgenden Voraussetzungen auch den Betreff und den Ort eines Ereignisses zurückgeben:

- Wenn das Ereignis mit geringer Vertraulichkeitsstufe markiert ist: `normal` oder `personal`, UND eine oder mehrere der folgenden Bedingungen treffen zu:

- Die Kalendereinstellungen des angeforderten Benutzers ermöglichen allen Benutzern in der Organisation, Titel und Orte anzuzeigen.
- Der Kalender des angeforderten Benutzers ist für den angemeldeten Benutzer freigegeben.
- Der angemeldete Benutzer ist ein Administrator derselben Organisation wie der angeforderte Benutzer.

## <a name="time-zone-representation"></a>Zeitzonendarstellung
Standardmäßig werden die Start- und Endzeiten der zurückgegebenen Zeitplanelemente in UTC dargestellt. Sie können eine `Prefer`-Kopfzeile verwenden, um eine für Ihre App geeignete Zeitzone anzugeben. Beispiel: 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a>Beschränkungen und Fehlerursachen
Beachten Sie die folgenden Beschränkungen und Fehlerbedingungen:

- **getSchedule** kann das Nachschlagen von Frei/Gebucht-Informationen für bis zu 20 Entitäten gleichzeitig unterstützen. Dieser Grenzwert gilt für die Anzahl von Benutzern, die einzeln oder als Mitglieder einer Verteilerliste identifiziert wurden, und auch für die Anzahl von Ressourcen.
- Der Zeitraum zum Nachschlagen muss weniger als 42 Tage betragen.
- Wenn **getSchedule** keinen angegebenen Benutzer oder keine angegebene Ressource identifizieren kann, wird ein einzelnes Zeitplanelement zurückgegeben und der Fehler angezeigt. 

## <a name="see-also"></a>Siehe auch
- [Berechtigungsreferenz](permissions-reference.md#calendars-permissions)
- [Suchen nach möglichen Besprechungszeiten im Outlook-Kalender](findmeetingtimes-example.md)
