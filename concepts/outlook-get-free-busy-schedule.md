---
title: Abrufen des Frei/Gebucht-Zeitplans für Benutzer und Ressourcen,
description: Ein häufiges Szenario in einer Arbeits- oder Schulumgebung besteht darin, anzuzeigen, wann ein Benutzer für eine Besprechung verfügbar ist, oder die Verfügbarkeit eines Teams, Raums oder Geräts für einen Zeitraum zu durchsuchen.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 8ecf31ec74327d4f5fbd9d585eef24fcaec60709
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869197"
---
# <a name="get-freebusy-schedule-of-users-and-resources"></a>Abrufen des Frei/Gebucht-Zeitplans für Benutzer und Ressourcen,

Ein häufiges Szenario in einer Arbeits- oder Schulumgebung besteht darin, anzuzeigen, wann ein Benutzer für eine Besprechung verfügbar ist, oder die Verfügbarkeit eines Teams, Raums oder Geräts für einen Zeitraum zu durchsuchen.

Mit der [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0)-Aktion können Sie die Verfügbarkeitsinformationen einer oder mehrerer Entitäten (Benutzer, Verteilerlisten oder Ressourcen) für einen bestimmten Zeitraum abrufen. 

## <a name="example"></a>Beispiel

Ein einfach Beispiel ist das Suchen des Frei/Gebucht-Zeitplans eines Mitarbeiters Alex an einem bestimmten Tag von 9 Uhr bis 18 Uhr, Pacific Standard Time:

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule_concept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendar/getschedule 
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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value":[
        {
            "scheduleId":"AlexW@contoso.OnMicrosoft.com",
            "availabilityView":"111111002222222200000000000000000000",
            "scheduleItems":[
                {
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

## <a name="how-does-getschedule-compare-with-findmeetingtimes"></a>Worin unterscheiden sich getSchedule und findMeetingTimes?

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

### <a name="permissions"></a>Berechtigungen
"Calendars.Read.Shared" ist die niedrigste Berechtigung, die von **findmeetingtimes** benötigt wird.

"Calendar.Read" ist die niedrigste Berechtigung, die von **getSchedule** benötigt wird. 

### <a name="version-support"></a>Versionsunterstützung

**findmeetingtimes** und **getSchedule** sind sowohl allgemein verfügbar als auch für den Einsatz in Produktionsanwendungen geeignet.


## <a name="event-data-returned"></a>Zurückgegebene Ereignisdaten
"Calendar.Read" ist die niedrigste Berechtigung, die von **getSchedule** zum Abrufen von Frei/Gebucht-Informationen durch eine App benötigt wird. Je nach App-Szenario kann der angemeldete Benutzer oder der Administrator zustimmen.

Während die genehmigte Berechtigung es einer App erlaubt, **getSchedule** auf den Kalendern der angeforderten Benutzer über Outlook zu verwenden, steuert der angeforderte Benutzer, welche Ereignisdaten, falls vorhanden, von **getSchedule** zurückgegeben werden. 

Beispielsweise kann **getSchedule** den Frei/Belegt-Status und die Arbeitszeiten der angeforderten Benutzer oder auch die Eigenschaften **subject**, **location** und **isPrivate** eines Ereignisses zurückgeben, vorausgesetzt, dass:

- Das Ereignis mit geringer Vertraulichkeitsstufe markiert ist (`normal` oder `personal`) UND eine oder mehrere der folgenden Bedingungen zutreffen:

   - Die Kalendereinstellungen des angeforderten Benutzers erlauben es dem angemeldeten Benutzer, Betreffzeilen und Orte anzuzeigen.
   - Der Kalender des angeforderten Benutzers ist für den angemeldeten Benutzer freigegeben.

Diese Bedingungen gelten unabhängig davon, ob der angemeldete Benutzer ein Administrator in der Organisation ist. Der angeforderte Benutzer hat die Kontrolle über die zurückgegebenen Ereignisdaten.

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
