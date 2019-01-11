---
title: Ressourcentyp bookingAppointment
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: aed5f26d69835c69021e8c3c8c5e27f5180d6c69
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856112"
---
# <a name="bookingappointment-resource-type"></a>Ressourcentyp bookingAppointment

 > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.
 
Stellt einen Termin Kunden für eine [BookingService](bookingservice.md), durch eine Reihe von Mitarbeitern von Microsoft Bookings Unternehmen bereitgestellten ausgeführt.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste Termine](../api/bookingbusiness-list-appointments.md) |  [BookingAppointment](bookingappointment.md) -Auflistung | Rufen Sie eine Liste der **BookingAppointment** -Objekte in der angegebenen [Bookingbusiness](../resources/bookingbusiness.md). |
|[Erstellen von bookingAppointment](../api/bookingbusiness-post-appointments.md) |  [bookingAppointment](bookingappointment.md) | Erstellen Sie eine neue **BookingAppointment** für die angegebene [Bookingbusiness](../resources/bookingbusiness.md). |
|[Abrufen von bookingAppointment](../api/bookingappointment-get.md) | [bookingAppointment](bookingappointment.md) |Lesen Sie die Eigenschaften und Beziehungen des **BookingAppointment** -Objekts.|
|[Update](../api/bookingappointment-update.md) | [bookingAppointment](bookingappointment.md)    |Aktualisieren eines **BookingAppointment** -Objekts. |
|[Delete](../api/bookingappointment-delete.md) | Keine |Löscht ein Objekt **BookingAppointment** . |
|[Abbrechen](../api/bookingappointment-cancel.md)|Keine| Abbrechen eines **BookingAppointment** -Objekts.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|customerEmailAddress|String|Die SMTP-Adresse von der [BookingCustomer](bookingcustomer.md) , die den Termin buchungs-ist.|
|customerId|String|Die ID des der [BookingCustomer](bookingcustomer.md) für diesen Termin. Wenn keine ID angegeben wird, wenn ein Termin erstellt wird, wird ein neues **BookingCustomer** -Objekt erstellt. Einmal festlegen möchten, sollten Sie die **CustomerId** unveränderlich berücksichtigen.|
|customerLocation|[location](location.md)|Stellt die Standortinformationen für die [BookingCustomer](bookingcustomer.md) , die den Termin buchungs-ist.|
|Kundenname|String|Der Kunde seinen Namen.|
|customerNotes|String|Die Notizen aus der Kunde diesen Termin zugeordnet. Sie können den Wert nur beim Lesen dieses **BookingAppointment** anhand seiner ID abrufen. <br> Sie können diese Eigenschaft festlegen, nur, wenn Sie einen Termin zunächst mit einem neuen Kunden zu erstellen. Nach diesem Punkt ist der Wert des Kunden durch **CustomerId**dargestellten berechnet.|
|customerPhone|String|Telefonnummer des Kunden.|
|duration|Duration|Die Länge des Termins, im Format [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) gekennzeichnet. |
|end|[dateTimeTimeZone](datetimetimezone.md)|Das Datum, Uhrzeit und Zeitzone, das Ende des Termins.|
|id|String| Die ID des der **BookingAppointment**. Schreibgeschützt.|
|invoiceAmount|Gleitkommawert mit doppelter Genauigkeit|Die berechneter Betrag der Rechnung.|
|invoiceDate|[dateTimeTimeZone](datetimetimezone.md)|Das Datum, Uhrzeit und Zeitzone der Rechnung für diesen Termin.|
|invoiceId|String|Die ID der Rechnung.|
|invoiceStatus|string| Der Status der Rechnung. Mögliche Werte sind: `draft`, `reviewing`, `open`, `canceled`, `paid` und `corrective`.|
|invoiceUrl|String|Die URL der Rechnung in Microsoft Bookings.|
|optOutOfCustomerEmail|Boolean|True gibt an, dass die [BookingCustomer](bookingcustomer.md) für diesen Termin nicht möchte einer Bestätigung für diesen Termin.|
|postBuffer|Duration|Der Zeitraum, nach den Termin enden, für die Bereinigung als Beispiel zu reservieren. Der Wert wird im Format [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) ausgedrückt. |
|preBuffer|Duration|Die Zeitspanne, vor dem Beginn des Termins für die Vorbereitung, als Beispiel zu reservieren. Der Wert wird im Format [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) ausgedrückt.|
|Preis|Gleitkommawert mit doppelter Genauigkeit|Die regulären Preis für einen Termin für die angegebene [BookingService](bookingservice.md).|
|priceType|string| Eine Einstellung für die pricing Struktur von Diensten Flexibilität. Mögliche Werte sind: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs` und `notSet`.|
|Erinnerungen|[BookingReminder](bookingreminder.md) -Auflistung|Die Auflistung von Kunden Erinnerungen für diesen Termin gesendet. Der Wert dieser Eigenschaft ist nur bei dieser **BookingAppointment** anhand seiner ID Lesen verfügbar|
|selfServiceAppointmentId|String|Eine zusätzliche Tracking-ID für den Termin, wenn der Termin direkt vom Kunden auf der Seite scheduling im Gegensatz zur durch ein Mitarbeiter in den Namen des Kunden erstellt wurde.|
|ServiceID|String|Die ID des der [BookingService](bookingservice.md) , die diesen Termin zugeordnet ist.|
|serviceLocation|[location](location.md)|Der Speicherort, in dem der Dienst übermittelt wird.|
|Dienstname|String|Der Name des der **BookingService** , die diesen Termin zugeordnet ist.<br>Diese Eigenschaft ist optional, wenn Sie einen neuen Termin zu erstellen. Wenn nicht angegeben, wird es aus dem Dienst, der den Termin zugeordnet, von der **ServiceId** -Eigenschaft berechnet.|
|serviceNotes|String|Notizen aus einer [BookingStaffMember](bookingstaffmember.md). Der Wert dieser Eigenschaft ist nur bei dieser **BookingAppointment** anhand seiner ID Lesen verfügbar|
|staffMemberIds|Collection von Objekten des Typs „String“|Die ID der einzelnen [BookingStaffMember](bookingstaffmember.md) , die diesem Termin geplant ist.|
|start|[dateTimeTimeZone](datetimetimezone.md)|Das Datum, Uhrzeit und Zeitzone, die Beginn des Termins.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingAppointment"
}-->

```json
{
  "customerEmailAddress": "String",
  "customerId": "String",
  "customerLocation": {"@odata.type": "microsoft.graph.location"},
  "customerName": "String",
  "customerNotes": "String",
  "customerPhone": "String",
  "duration": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "id": "String (identifier)",
  "invoiceAmount": 1024,
  "invoiceDate": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "invoiceId": "String",
  "invoiceStatus": "string",
  "invoiceUrl": "String",
  "optOutOfCustomerEmail": true,
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "price": 1024,
  "priceType": "string",
  "reminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "selfServiceAppointmentId": "String",
  "serviceId": "String",
  "serviceLocation": {"@odata.type": "microsoft.graph.location"},
  "serviceName": "String",
  "serviceNotes": "String",
  "staffMemberIds": ["String"],
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingAppointment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
