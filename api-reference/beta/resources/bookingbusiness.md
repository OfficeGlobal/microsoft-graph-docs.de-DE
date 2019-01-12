---
title: Ressourcentyp bookingBusiness
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cf00239802cec9a705c24548649e38f3022383a0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986215"
---
# <a name="bookingbusiness-resource-type"></a>Ressourcentyp bookingBusiness

 > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.
 
Stellt ein Unternehmen in Microsoft Bookings dar. Dies ist das Objekt der obersten Ebene in der Microsoft-Buchungen-API. Es enthält Unternehmensinformationen und verwandte Geschäftsobjekte wie Termine, Kunden, Dienste und Mitarbeiter.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste bookingBusinesses](../api/bookingbusiness-list.md) | [BookingBusiness](bookingbusiness.md) -Auflistung |Rufen Sie eine Auflistung von Bookingbusiness-Objekten im Mandanten. |
|[Erstellen von bookingBusiness](../api/bookingbusiness-post-bookingbusinesses.md) | [bookingBusiness](bookingbusiness.md) | Erstellen einer neuen Microsoft Bookings Business an. |
|[Abrufen von bookingBusiness](../api/bookingbusiness-get.md) | [bookingBusiness](bookingbusiness.md) |Lesen Sie Eigenschaften und Beziehungen des BookingBusiness-Objekts.|
|[Update](../api/bookingbusiness-update.md) | [bookingBusiness](bookingbusiness.md) |Aktualisieren von Eigenschaften in einem **BookingBusiness** -Objekt. |
|[Delete](../api/bookingbusiness-delete.md) | Keine |Löscht ein Objekt **BookingBusiness** . |
|[Erstellen von bookingAppointment](../api/bookingbusiness-post-appointments.md) |[bookingAppointment](bookingappointment.md)| Erstellen Sie eine neue BookingAppointment, indem Sie das Veröffentlichen in der Auflistung Termine.|
|[Liste Termine](../api/bookingbusiness-list-appointments.md) |[BookingAppointment](bookingappointment.md) -Auflistung| Rufen Sie eine Auflistung der BookingAppointment-Objekts.|
|[Erstellen von bookingCustomer](../api/bookingbusiness-post-customers.md) |[bookingCustomer](bookingcustomer.md)| Erstellen Sie eine neue BookingCustomer, durch die Veröffentlichung auf der Customers-Auflistung.|
|[Liste von Kunden](../api/bookingbusiness-list-customers.md) |[BookingCustomer](bookingcustomer.md) -Auflistung| Rufen Sie eine Auflistung der BookingCustomer-Objekts.|
|[Erstellen von bookingService](../api/bookingbusiness-post-services.md) |[bookingService](bookingservice.md)| Erstellen Sie eine neue BookingService, indem Sie das Veröffentlichen in der Auflistung der Dienste.|
|[Liste Dienste](../api/bookingbusiness-list-services.md) |[BookingService](bookingservice.md) -Auflistung| Rufen Sie eine Auflistung der BookingService-Objekts.|
|[Erstellen von bookingStaffMember](../api/bookingbusiness-post-staffmembers.md) |[bookingStaffMember](bookingstaffmember.md)| Erstellen Sie eine neue BookingStaffMember, durch die Veröffentlichung auf der StaffMembers-Auflistung.|
|[Liste staffMembers](../api/bookingbusiness-list-staffmembers.md) |[BookingStaffMember](bookingstaffmember.md) -Auflistung| Rufen Sie eine Auflistung der BookingStaffMember-Objekts.|
|[calendarView auflisten](../api/bookingbusiness-list-calendarview.md)|[BookingAppointment](bookingappointment.md) -Auflistung|Rufen Sie die Auflistung von **BookingAppointment** -Objekten, die in der angegebene Datumsbereich auftritt.|
|[Veröffentlichen](../api/bookingbusiness-publish.md)|Keines|Stellen Sie die Terminplan Seite dieses Unternehmens externen Kunden zur Verfügung. **IsPublished** -Eigenschaft auf True festgelegt, und **PublicUrl** -Eigenschaft, um die URL der Seite planen.|
|[Aufheben der Veröffentlichung](../api/bookingbusiness-unpublish.md)|Keines| Stellen Sie die Terminplan Seite dieses Unternehmens externen Kunden nicht zur Verfügung. **IsPublished** -Eigenschaft auf False und **PublicUrl** -Eigenschaft auf null festgelegt.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|address|[physicalAddress](physicaladdress.md)|Die Straße des Unternehmens. Die **Address** -Eigenschaft zusammen mit **Telefon-** und **WebSiteUrl**, in der Fußzeile eines Unternehmens planen Seite angezeigt werden.|
|businessHours|[BookingWorkHours](bookingworkhours.md) -Auflistung|Die Betriebszeiten für das Unternehmen.|
|businessType|Zeichenfolge|Der Typ des Unternehmens.|
|defaultCurrencyIso|Zeichenfolge|Der Code für die Währung, die das Unternehmen in für Microsoft Bookings ausgeführt wird.|
|displayName|Zeichenfolge|Der Name des Unternehmens, welche mit Kunden Schnittstellen. Dieser Name wird im oberen Bereich des Unternehmens planen Seite angezeigt.|
|E-Mail|Zeichenfolge|Die e-Mail-Adresse für das Unternehmen.|
|id|Zeichenfolge|Ein eindeutiger programmgesteuerten Bezeichner für das Unternehmen. Schreibgeschützt.|
|isPublished|Boolescher Wert|Die Seite scheduling wurde an externen Kunden zur Verfügung gestellt. Verwenden Sie die Aktionen **Veröffentlichen** und **Aufheben der Veröffentlichung** , um diese Eigenschaft festzulegen. Schreibgeschützt.|
|phone|String|Die Telefonnummer für das Unternehmen. Die **Telefon** -Eigenschaft zusammen mit der **Adresse** und **WebSiteUrl**, in der Fußzeile eines Unternehmens planen Seite angezeigt werden.|
|publicUrl|Zeichenfolge|Die URL für die Planung Seite, die nach dem Sie [Veröffentlichen](../api/bookingbusiness-publish.md) oder [Aufheben der Veröffentlichung](../api/bookingbusiness-unpublish.md) die Seite festgelegt ist. Schreibgeschützt.|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|Gibt an, wie die Buchungen für dieses Unternehmen erstellt werden können.|
|webSiteUrl|Zeichenfolge|Die URL der Website für die Business. Die **WebSiteUrl** -Eigenschaft zusammen mit der **Adresse**, **Telefon**, in der Fußzeile einer scheduling Business-Seite angezeigt werden.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Termine|[BookingAppointment](bookingappointment.md) -Auflistung| Alle Termine in Unternehmen. Schreibgeschützt. Lässt Nullwerte zu.|
|calendarView|[BookingAppointment](bookingappointment.md) -Auflistung| Der Satz von Terminen dieses Unternehmens in einem bestimmten Zeitraum. Schreibgeschützt. Lässt Nullwerte zu.|
|Kunden|[BookingCustomer](bookingcustomer.md) -Auflistung| Alle Kunden in Unternehmen. Schreibgeschützt. Lässt Nullwerte zu.|
|Dienste|[BookingService](bookingservice.md) -Auflistung| Alle Dienste dieses Unternehmen angeboten. Schreibgeschützt. Lässt Nullwerte zu.|
|staffMembers|[BookingStaffMember](bookingstaffmember.md) -Auflistung| Alle die Mitarbeiter, die in dieser Dienste bereitstellen. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingBusiness"
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "businessHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}],
  "businessType": "String",
  "defaultCurrencyIso": "String",
  "displayName": "String",
  "email": "String",
  "id": "String (identifier)",
  "isPublished": true,
  "phone": "String",
  "publicUrl": "String",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "webSiteUrl": "String"
}

```

## <a name="see-also"></a>Siehe auch


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingBusiness resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
