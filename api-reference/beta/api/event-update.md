---
title: Ereignis aktualisieren
description: Aktualisieren Sie die Eigenschaften des Event-Objekts.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b3f101c14a69c6dc2b3687e9d4a1509e6ac7a531
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524975"
---
# <a name="update-event"></a>Ereignis aktualisieren

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktualisieren Sie die Eigenschaften des [Event](../resources/event.md) -Objekts.
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

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

| Eigenschaft       | Typ    | Beschreibung |
|:---------------|:--------|:------------|
| attendees|Teilnehmer|Die Sammlung der Teilnehmer des Ereignisses|
| body|ItemBody|Der Text der Nachricht, die mit diesem Ereignis verknüpft ist.|
| categories|String|Die Kategorien, die mit dem Ereignis verknüpft sind.|
| end|DateTimeTimeZone|Datum und Uhrzeit für das Ende des Ereignisses.<br/><br/>Standardmäßig ist die Endzeit in UTC angegeben. Sie können eine optionale Zeitzone in EndTimeZone angeben, die Endzeit in dieser Zeitzone angeben und einen Zeitunterschied zur UTC-Zeitzone angeben. Beachten Sie, dass bei Verwendung von EndTimeZone auch ein Wert für StartTimeZone angegeben werden muss.<br/><br/>In diesem Beispiel wird der 25. Februar 2015 21:34 in PST angegeben: „2015-02-25T21:34:00-08:00“. |
| Wichtigkeit|String|Die Wichtigkeit des Ereignisses. Mögliche Werte sind: `low`, `normal` und `high`.|
| isAllDay|Boolescher Wert|True, wenn das Ereignis den ganzen Tag andauert.|
| isReminderOn|Boolean|True, wenn eine Benachrichtigung den Benutzer an das Ereignis erinnern soll.|
| location|Ort|Der Ort des Ereignisses.|
|locations|[Standort](../resources/location.md) -Auflistung|Die Orte, an denen die Veranstaltung stattfindet. Die Eigenschaften **location** und **locations** entsprechen sich immer gegenseitig. Wenn Sie die **location**-Eigenschaft aktualisieren, werden alle früheren Orte in der **locations**-Sammlung entfernt und durch den neuen **location**-Wert ersetzt. |
| recurrence|PatternedRecurrence|Das Serienmuster für das Ereignis.|
| reminderMinutesBeforeStart|Int32|Festlegung, wie viele Minuten vor Beginn des Ereignisses die Erinnerung angezeigt werden soll|
| responseRequested|Boolean|Legen Sie „True“ fest, wenn der Absender eine Antwort erhalten soll, wenn das Ereignis akzeptiert oder abgelehnt wird.|
| sensitivity|Zeichenfolge| Mögliche Werte: `normal`, `personal`, `private`, `confidential`.|
| showAs|Zeichenfolge|Der anzuzeigende Status. Mögliche Werte sind: `free` , `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
| start|DateTimeTimeZone|Die Startzeit des Ereignisses. <br/><br/>Standardmäßig ist die Startzeit in UTC angegeben. Sie können eine optionale Zeitzone in StartTimeZone angeben, die Startzeit in dieser Zeitzone angeben und einen Zeitunterschied zur UTC-Zeitzone angeben. Beachten Sie, dass bei Verwendung von StartTimeZone auch ein Wert für EndTimeZone angegeben werden muss.<br/><br/>In diesem Beispiel wird 25. Februar 2015 19:34 in PST angegeben: „2015-02-25T19:34:00-08:00“.  |
| subject|String|Der Text der Betreffzeile des Ereignisses|

Da die Ressource **Ereignis** [Extensions](/graph/extensibility-overview)unterstützt, können Sie mithilfe der `PATCH` Vorgang hinzufügen, aktualisieren oder Löschen von Ihren eigenen app-spezifischen Daten in benutzerdefinierten Eigenschaften einer Erweiterung in einer vorhandenen Instanz **Ereignis** .

Wenn das **Ereignis** sind Sie aktualisieren das master-Ereignis einer Terminserie ist, mehrere Teilnehmer und enthält Instanzen, die separat aktualisiert wurden, mehrere Benachrichtigung-e-Mails gesendet werden: einen für die master-Serie und jeweils eine pro Instanz, die hat aktualisiert wurde.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [vent](../resources/event.md)-Objekt im Antworttext zurückgegeben.

>**Hinweis:** Diese Methode kann eine HTTP-400-Bad Request Antwort mit den Fehlercode zurückgeben `ErrorOccurrenceCrossingBoundary` und die folgende Fehlermeldung angezeigt: geändertes Serienelement crossing oder überlappende benachbarten Serienelement ist. Dies gibt an, dass das Update die folgenden Outlook-Einschränkung auf Serienausnahmen verletzt: das auftreten ein Serientermins kann nicht verschoben werden, auf oder vor dem Tag des vorherigen Vorkommens und kann nicht an oder nach dem Tag des folgenden Vorkommens verschoben werden.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_event"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/events/{id}
Content-type: application/json
Content-length: 285

{
  "originalStartTimeZone": "originalStartTimeZone-value",
  "originalEndTimeZone": "originalEndTimeZone-value",
  "responseStatus": {
    "response": "",
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
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
    "time": "2016-10-19T10:37:00Z"
  },
  "recurrence": null,
  "uid": "iCalUId-value",
  "reminderMinutesBeforeStart": 99,
  "isReminderOn": true
}
```


## <a name="see-also"></a>Siehe auch

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)](/graph/extensibility-open-users)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
