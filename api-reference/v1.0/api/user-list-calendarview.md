---
title: calendarView auflisten
description: 'Abrufen der vorkommen, Ausnahmen und einzelne Instanzen von Ereignissen in einer Kalenderansicht durch ein Zeitbereich, von dem Benutzer Standardkalender definiert, '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2f90f1f5d3af6da0e84919128b362777268f4e0e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984227"
---
# <a name="list-calendarview"></a>calendarView auflisten

Mit dieser API können Sie Vorkommen, Ausnahmen und einzelnen Instanzen von Ereignissen in einer durch einen Zeitbereich definierten Kalenderansicht aus dem Standardkalender des Benutzers oder aus einem seiner anderen Kalender abrufen.
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Calendars.Read, Calendars.ReadWrite    |
|Delegiert (persönliches Microsoft-Konto) | Calendars.Read, Calendars.ReadWrite    |
|Anwendung | Calendars.Read, Calendars.ReadWrite |

## <a name="http-request"></a>HTTP-Anforderung

Der standardmäßige [Kalender](../resources/calendar.md) eines Benutzers:
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendar/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

Der [Kalender](../resources/calendar.md) eines Benutzers in der standardmäßigen [CalendarGroup](../resources/calendargroup.md).
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

Der [Kalender](../resources/calendar.md) eines Benutzers in einer bestimmten [CalendarGroup](../resources/calendargroup.md).
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
```

## <a name="query-parameters"></a>Abfrageparameter

Stellen Sie in der URL der Anforderung die folgenden Funktionsparameter mit Werten bereit.

| Parameter    | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|startDateTime|Zeichenfolge|Startdatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Beispielsweise „2015-11-08T19:00:00.0000000“.|
|endDateTime|Zeichenfolge|Enddatum und -uhrzeit des Zeitraums, dargestellt im ISO 8601-Format. Z. B. „2015-11-08T20:00:00.0000000“.|

Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung |
|:---------------|:--------|:--------|
| Authorization  | string | Bearer {token}. Erforderlich.  |
| Prefer: outlook.timezone  | string | Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben. Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben. Optional. |
| Besser: outlook.body-content-type | string | Das Format, in der die **body**-Eigenschaft zurückgegeben werden soll. Werte können „Text“ oder „html“ sein. Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist. Wenn die Kopfzeile nicht angegeben ist, wird die **body**-Eigenschaft im HTML-Format zurückgegeben. Optional. |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Event](../resources/event.md)-Objekten im Antworttext zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_calendarview"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView?startDateTime=2016-01-01T19:00:00.0000000&endDateTime=2016-10-01T19:00:00.0000000 
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "",
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
