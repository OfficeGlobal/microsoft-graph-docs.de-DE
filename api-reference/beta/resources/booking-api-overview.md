---
title: Verwenden der Microsoft Bookings-API in Microsoft Graph
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Priority
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 7fc58a4fe0fb616963fd91d83a401d4ad8e1c43e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529859"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a>Verwenden der Microsoft Bookings-API in Microsoft Graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Mit Microsoft Bookings können Kleinunternehmer mit geringem Aufwand Kundenbuchungen und -informationen verwalten. Ein Geschäftsinhaber kann ein oder mehrere Unternehmen erstellen, wobei jedes Unternehmen ein eigenes Angebot an Diensten beinhaltet. Der Geschäftsinhaber kann Mitarbeiter einrichten und Dienste angeben, die jeder Mitarbeiter ausführt. Ein Kunde kann einen Termin für einen bestimmten Dienst in diesem Unternehmen entweder online oder über eine mobile App buchen. Mit Bookings wird sichergestellt, dass der Termin für das Unternehmen, die Mitarbeiter und die jeweils involvierten Kunden auf dem neuesten Stand ist.

Ein [bookingBusiness](bookingbusiness.md)-Objekt umfasst programmgesteuert in der Bookings-API die folgenden Objekte:
 
- Ein oder mehrere [bookingStaffMember](bookingstaffmember.md)-Objekte
- Ein oder mehrere [bookingservice](bookingservice.md)-Objekte
- Mehrere [bookingAppointment](bookingappointment.md)-Instanzen
- Mehrere [bookingCustomer](bookingcustomer.md)-Objekte

## <a name="using-the-bookings-rest-api"></a>Verwenden der Bookings-REST-API

Führen Sie die folgenden Schritte aus, bevor Sie zum ersten Mal Kundentermine für ein Unternehmen buchen. Stellen Sie sicher, dass Sie die entsprechenden [Zugriffstoken](/graph/auth-overview) für die entsprechenden Vorgänge bereitstellen.

1. Stellen Sie sicher, dass das Unternehmen über ein [Office 365 Business Premium](https://products.office.com/de-DE/business/office-365-business-premium)-Abonnement verfügt.
2. Erstellen Sie ein neues **bookingBusiness**-Objekt, indem Sie einen POST-Vorgang an die Entitätenmenge senden. Sie sollten mindestens einen Namen für das neue Unternehmen angeben, das Kunden angezeigt wird: <!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
Verwenden Sie die **id**-Eigenschaft des neuen **bookingBusiness**-Objekts, das in der POST-Antwort zurückgegeben wurde, um mit dem [Anpassen](../api/bookingbusiness-update.md) der Unternehmenseinstellungen fortzufahren, und fügen Sie Mitarbeiter und Dienste für das Unternehmen hinzu.

3. Fügen Sie einzelne Mitarbeiter für das Unternehmen hinzu: <!-- { "blockType": "ignored" } -->
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
4. Definieren Sie jeden Dienst, der vom Unternehmen angeboten wird: <!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. Veröffentlichen Sie die Seite für die Terminvergabe für das Unternehmen, damit Kunden und Betreiber des Unternehmens Termine buchen können: <!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

So können Sie generell alle Unternehmen mit Bookings im Office 365-Mandanten auflisten: <!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a>Allgemeine Anwendungsfälle 

Die folgende Tabelle enthält die allgemeinen Vorgänge für ein Unternehmen in der Bookings-API.

| Anwendungsfälle        | REST-Ressourcen | Siehe auch |
|:---------------|:--------|:----------|
| Erstellen, Abrufen, Aktualisieren oder Löschen eines Unternehmens | [bookingBusiness](bookingbusiness.md) | [Methoden von bookingBusiness](bookingbusiness.md#methods) |
| Aktualisieren der Richtlinie für die Terminvergabe | [bookingSchedulingPolicy](bookingschedulingpolicy.md) | [Aktualisieren von bookingBusiness](../api/bookingbusiness-update.md) |
| Hinzufügen, Abrufen, Aktualisieren oder Löschen von Mitarbeitern | [bookingStaffMember](bookingstaffmember.md) | [Methoden von bookingStaffMember](bookingstaffmember.md#methods)  |
| Hinzufügen, Abrufen, Aktualisieren oder Löschen von Diensten | [bookingService](bookingservice.md) | [Methoden von bookingService](bookingservice.md#methods)  |
| Veröffentlichen oder Aufheben der Veröffentlichung der Seite für die Terminvergabe | [bookingBusiness](bookingbusiness.md) | [publish](../api/bookingbusiness-publish.md) <br> [unpublish](../api/bookingbusiness-unpublish.md) |
| Erstellen, Abrufen, Aktualisieren, Löschen oder Absagen von Terminen | [bookingAppointment](bookingappointment.md) | [Methoden von bookingAppointment](bookingappointment.md#methods)  |
| Abrufen von Terminen in einem Datumsbereich | [bookingBusiness](bookingbusiness.md) | [Auflisten von Bookings für calendarView](../api/bookingbusiness-list-calendarview.md) |
| Abrufen der Währung | [bookingCurrency](bookingcurrency.md) | [Methoden von bookingCurrency](bookingcurrency.md#methods) |


## <a name="see-also"></a>Siehe auch

- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.
- Sehen Sie sich an, [wie unsere Partner Microsoft Graph verwenden](https://developer.microsoft.com/graph/graph/examples#partners).
- Erfahren Sie, wie [Berechtigungen](/graph/permissions-reference) in Microsoft Graph ausgewählt werden können.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/booking-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
