---
title: Verwenden Sie die Microsoft-Buchungen API in Microsoft Graph
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: 5e553e2814c6e5554ea7bb2f4daef8c62057aff3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062758"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a>Verwenden Sie die Microsoft-Buchungen API in Microsoft Graph

 > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.
 
Microsoft Bookings können Kleinunternehmen Besitzer Kunden Buchungen und Informationen mit minimalem Setup zu verwalten. Eigentümer eines Unternehmens kann eine oder mehrere Unternehmen mit jedem Business bietet eine Reihe von Diensten erstellen. Der Besitzer kann Einrichten von Mitarbeitern, und geben Sie die Dienste, die jeder Mitarbeiter durchführt. Ein Kunde kann einen Termin für einen bestimmten Dienst in dieses Unternehmen in einer app online oder mobilen Buch. Buchungen stellt sicher, dass, die die Zeit des Termins für die Business, Mitarbeitern und Kunden beteiligten aktualisiert wird.

Programmgesteuertes, umfasst eine [BookingBusiness](bookingbusiness.md) in der Buchungen API die folgenden Objekte:
 
- Ein oder mehrere [BookingStaffMember](bookingstaffmember.md) -Objekte
- Ein oder mehrere [BookingService](bookingservice.md) -Objekte
- Eine Reihe von [BookingAppointment](bookingappointment.md) Instanzen
- Eine Reihe von [BookingCustomer](bookingcustomer.md) -Objekten

## <a name="using-the-bookings-rest-api"></a>Verwenden die Buchungen REST-API

Lernen Sie die folgenden Schritte vor dem Buchen Kundenterminen für ein Unternehmen beim ersten. Stellen Sie sicher, dass Sie die entsprechenden [Zugriffstoken](/graph/auth-overview) für die entsprechenden Vorgänge angeben.

1. Stellen Sie sicher, dass das Unternehmen ein [Office 365 Business Premium](https://products.office.com/en-us/business/office-365-business-premium) -Abonnement verfügt.
2. Erstellen einer neuen **BookingBusiness** durch Senden einer POST-Operation auf die Entität. Mindestens sollten Sie einen Namen für die neue Business angeben, die Kunden angezeigt werden:<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
Verwenden Sie die **Id** -Eigenschaft des neuen **BookingBusiness** in der POST-Antwort zurückgegeben Business Einstellungen [Anpassen](../api/bookingbusiness-update.md) möchten, und fügen Sie Mitarbeiter und Dienste für das Unternehmen.

3. Fügen Sie einzelne Mitarbeiter für das Unternehmen:<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/staffMembers
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Dana Swope",
    "emailAddress": "danas@contoso.com",
    "role": "externalGuest"
}
```
4. Definieren Sie jeden Dienst, der vom Unternehmen angeboten:<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. Veröffentlichen der scheduling Seite für das Unternehmen zu Kunden und Unternehmer buchen Termine vornehmen zu lassen:<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

Im Allgemeinen so Listen Sie alle buchen Unternehmen in Office 365-Mandanten:<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a>Allgemeine Anwendungsfälle 

Die folgende Tabelle enthält die allgemeine Vorgänge für ein Unternehmen in der Buchungen-API.

| Anwendungsfälle        | REST-Ressourcen | Siehe auch |
|:---------------|:--------|:----------|
| Erstellen, abrufen, aktualisieren oder Löschen eines Unternehmens | [bookingBusiness](bookingbusiness.md) | [Methoden des bookingBusiness](bookingbusiness.md#methods) |
| Aktualisieren der scheduling-Richtlinie | [bookingSchedulingPolicy](bookingschedulingpolicy.md) | [Aktualisieren einer bookingBusiness](../api/bookingbusiness-update.md) |
| Hinzufügen, abrufen, aktualisieren oder Löschen von Mitarbeitern | [bookingStaffMember](bookingstaffmember.md) | [Methoden des bookingStaffMember](bookingstaffmember.md#methods)  |
| Hinzufügen, abrufen, aktualisieren oder Löschen von Diensten | [bookingService](bookingservice.md) | [Methoden des bookingService](bookingservice.md#methods)  |
| Veröffentlichen oder Aufheben der Veröffentlichung der Seite scheduling | [bookingBusiness](bookingbusiness.md) | [Veröffentlichen](../api/bookingbusiness-publish.md) <br> [Aufheben der Veröffentlichung](../api/bookingbusiness-unpublish.md) |
| Erstellen, abrufen, aktualisieren, löschen oder Abbrechen eines Termins | [bookingAppointment](bookingappointment.md) | [Methoden des bookingAppointment](bookingappointment.md#methods)  |
| Abrufen von Terminen in einen bestimmten Datumsbereich | [bookingBusiness](bookingbusiness.md) | [Liste Buchungen calendarView](../api/bookingbusiness-list-calendarview.md) |
| Währung abrufen | [bookingCurrency](bookingcurrency.md) | [Methoden des bookingCurrency](bookingcurrency.md#methods) |


## <a name="see-also"></a>Siehe auch

- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.
- Finden Sie unter [wie einige unsere Partner Microsoft Graph verwenden](https://developer.microsoft.com/graph/graph/examples#partners).
- Erfahren Sie, wie [Berechtigungen](/graph/permissions-reference) in Microsoft Graph entscheiden.