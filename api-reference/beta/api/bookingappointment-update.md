---
title: Bookingappointment aktualisieren
description: Aktualisieren Sie die Eigenschaften eines BookingAppointment-Objekts in der angegebenen Bookingbusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cde8a309e3544f5ed5cdf84f7c50d33e95084526
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529236"
---
# <a name="update-bookingappointment"></a>Bookingappointment aktualisieren

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktualisieren Sie die Eigenschaften eines [BookingAppointment](../resources/bookingappointment.md) -Objekts in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md).
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) |  BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All   |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt   |
|Anwendung | Nicht unterstützt  |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-request-headers"></a>Optionale Anforderungsheader
| Name       | Beschreibung|
|:-----------|:-----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|customerEmailAddress|String|Die SMTP-Adresse von der [BookingCustomer](../resources/bookingcustomer.md) , die den Termin buchungs-ist.|
|customerId|String|Die ID des der [BookingCustomer](../resources/bookingcustomer.md) für diesen Termin. Wenn keine ID angegeben wird, wenn ein Termin erstellt wird, wird ein neues **BookingCustomer** -Objekt erstellt. Einmal festlegen möchten, sollten Sie die **CustomerId** unveränderlich berücksichtigen.|
|customerLocation|[location](../resources/location.md)|Stellt die Standortinformationen für die [BookingCustomer](../resources/bookingcustomer.md) , die den Termin buchungs-ist.|
|Kundenname|String|Der Kunde seinen Namen.|
|customerNotes|String|Die Notizen aus der Kunde diesen Termin zugeordnet. Sie können den Wert nur beim Lesen dieses **BookingAppointment** anhand seiner ID abrufen. <br> Sie können diese Eigenschaft festlegen, nur, wenn Sie einen Termin zunächst mit einem neuen Kunden zu erstellen. Nach diesem Punkt ist der Wert des Kunden durch **CustomerId**dargestellten berechnet.|
|customerPhone|String|Telefonnummer des Kunden.|
|duration|Dauer|Die Länge des Termins, im Format [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) gekennzeichnet. |
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|Das Datum, Uhrzeit und Zeitzone, das Ende des Termins.|
|invoiceAmount|Gleitkommawert mit doppelter Genauigkeit|Die berechneter Betrag der Rechnung.|
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)|Das Datum, Uhrzeit und Zeitzone der Rechnung für diesen Termin.|
|invoiceId|String|Die ID der Rechnung.|
|invoiceStatus|string| Der Status der Rechnung. Mögliche Werte sind: `draft`, `reviewing`, `open`, `canceled`, `paid` und `corrective`.|
|invoiceUrl|String|Die URL der Rechnung in Microsoft Bookings.|
|optOutOfCustomerEmail|Boolescher Wert|True gibt an, dass die [BookingCustomer](../resources/bookingcustomer.md) für diesen Termin nicht möchte einer Bestätigung für diesen Termin.|
|postBuffer|Dauer|Der Zeitraum, nach den Termin enden, für die Bereinigung als Beispiel zu reservieren. Der Wert wird im Format [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) ausgedrückt. |
|preBuffer|Dauer|Die Zeitspanne, vor dem Beginn des Termins für die Vorbereitung, als Beispiel zu reservieren. Der Wert wird im Format [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) ausgedrückt.|
|Price|Gleitkommawert mit doppelter Genauigkeit|Die regulären Preis für einen Termin für die angegebene [BookingService](../resources/bookingservice.md).|
|priceType|string| Eine Einstellung für die pricing Struktur von Diensten Flexibilität. Mögliche Werte sind: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs` und `notSet`.|
|Erinnerungen|[BookingReminder](../resources/bookingreminder.md) -Auflistung|Die Auflistung von Kunden Erinnerungen für diesen Termin gesendet. Der Wert dieser Eigenschaft ist nur bei dieser **BookingAppointment** anhand seiner ID Lesen verfügbar|
|selfServiceAppointmentId|String|Eine zusätzliche Tracking-ID für den Termin, wenn der Termin direkt vom Kunden auf der Seite scheduling im Gegensatz zur durch ein Mitarbeiter in den Namen des Kunden erstellt wurde.|
|ServiceID|String|Die ID des der [BookingService](../resources/bookingservice.md) , die diesen Termin zugeordnet ist.|
|serviceLocation|[location](../resources/location.md)|Der Speicherort, in dem der Dienst übermittelt wird.|
|Dienstname|String|Der Name des der **BookingService** , die diesen Termin zugeordnet ist.<br>Diese Eigenschaft ist optional, wenn Sie einen neuen Termin zu erstellen. Wenn nicht angegeben, wird es aus dem Dienst, der den Termin zugeordnet, von der **ServiceId** -Eigenschaft berechnet.|
|serviceNotes|String|Notizen aus einer [BookingStaffMember](../resources/bookingstaffmember.md). Der Wert dieser Eigenschaft ist nur bei dieser **BookingAppointment** anhand seiner ID Lesen verfügbar|
|staffMemberIds|Zeichenfolgenauflistung|Die ID der einzelnen [BookingStaffMember](../resources/bookingstaffmember.md) , die diesem Termin geplant ist.|
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)|Das Datum, Uhrzeit und Zeitzone, die Beginn des Termins.|


## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204, No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Im folgenden Beispiel wird das Datum des Diensts durch einen Tag geändert, und aktualisiert sowie das Rechnungsdatum.
<!-- {
  "blockType": "request",
  "name": "update_bookingappointment"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingAppointment",
    "end":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceDate":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "start":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-06T12:00:00.0000000+00:00",
        "timeZone":"UTC"
    }
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingappointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingappointment-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
