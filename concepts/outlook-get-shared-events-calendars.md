# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a>Abrufen von Outlook-Ereignissen in einem freigegebenen oder delegierten Kalender

Kunden können in Outlook einen Kalender für andere Benutzer freigeben und diese Benutzer dadurch berechtigen, Ereignisse in diesem Kalender abzurufen oder zu ändern. Kunden können auch die Berechtigung delegieren, an ihrer statt Besprechungsanfragen zu empfangen oder auf diese zu antworten oder Änderungen im Kalender vorzunehmen.

Calendar Microsoft Graph unterstützt programmgesteuert das Abrufen von Ereignissen in Kalendern, die von anderen Benutzern freigegeben wurden, sowie Zugriff auf die freigegebenen Kalender. Die Unterstützung gilt auch für Kalender, die delegiert wurden.

Zum Beispiel hat Garth seinen Standardkalender für John freigegeben und John Lesezugriff gewährt. Wenn John sich in Ihrer App angemeldet und delegierte Berechtigungen (Calendars.Read.Shared or Calendars.ReadWrite.Shared) bereitgestellt hat, kann Ihre App auf Garths Kalender sowie auf Ereignisse in diesem Kalender zugreifen, wie nachstehend beschrieben.

## <a name="get-an-event-in-the-shared-calendar"></a>Abrufen eines Ereignisses in dem freigegebenen Kalender

Sie können ein bestimmtes Ereignis in Garths freigegebenem Kalender abrufen:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

Bei erfolgreichem Abschluss erhalten Sie HTTP 200 OK und die [Ereignis](../api-reference/v1.0/resources/event.md)-Instanz mit der ID `{id}` aus Garths Standardkalender.

## <a name="get-all-the-events-in-the-shared-calendar"></a>Alle Ereignisse in dem freigegebenen Kalender abrufen

Abrufen aller Ereignisse im Standardkalender, den Garth für John freigegeben hat:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

Bei erfolgreichem Abschluss erhalten Sie HTTP 200 OK und eine Sammlung von [Ereignis](../api-reference/v1.0/resources/event.md)-Instanzen in Garths Standardkalender.

## <a name="get-the-shared-calendar"></a>Abrufen des freigegebenen Kalenders

Abrufen des Standardkalenders, den Garth für John freigegeben hat.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

Bei erfolgreichem Abschluss erhalten Sie HTTP 200 OK und eine [Kalender](../api-reference/v1.0/resources/calendar.md)-Instanz, die Garths Standardordner darstellt.

Dieselben GET-Funktionen würden gelten, wenn Garth an John weiteren Zugriff auf Garths Standardkalender delegiert hätte oder wenn Garth sein gesamtes Postfach an John delegiert hätte.

Wenn Garth weder seinen Standardkalender für John freigegeben noch sein Postfach an John delegiert hat, wird bei der Angabe der Benutzer-ID oder des Benutzerprinzipalnamens von Garth in diesen GET-Vorgängen ein Fehler zurückgegeben. 


## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen:

- [Vorteile der Integration mit dem Outlook-Kalender](outlook-calendar-concept-overview.md)
- Die [Kalender-API](../api-reference/v1.0/resources/calendar.md) in Microsoft Graph v1. 0.