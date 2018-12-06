---
title: Übersicht über die Microsoft Bookings-API (Vorschau)
description: Microsoft Bookings bietet Online- und Mobilgeräte-Apps, die das Planen von Terminen für kleine Unternehmen und ihre Kunden vereinfachen. Kleine Unternehmen, die ihre Services auf Terminbasis anbieten, wie z. B. Autowerkstätten, Frisörsalons und Anwaltskanzleien, können von der Verwaltung ihrer Terminvereinbarungen profitieren, da sie so ihre Zeit mit wichtigeren Aufgaben verbringen können, um ihr Geschäft voranzutreiben. Microsoft Bookings steht für Unternehmen mit einem Office 365 Business Premium-Abonnement zur Verfügung.
ms.openlocfilehash: 334b26b5f02e7060b0fddfe8264e138e9d3a2bdc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092286"
---
# <a name="microsoft-bookings-api-overview-preview"></a>Übersicht über die Microsoft Bookings-API (Vorschau)

Microsoft Bookings bietet Online- und Mobilgeräte-Apps, die das Planen von Terminen für kleine Unternehmen und ihre Kunden vereinfachen. Kleine Unternehmen, die ihre Services auf Terminbasis anbieten, wie z. B. Autowerkstätten, Frisörsalons und Anwaltskanzleien, können von der Verwaltung ihrer Terminvereinbarungen profitieren, da sie so ihre Zeit mit wichtigeren Aufgaben verbringen können, um ihr Geschäft voranzutreiben. Microsoft Bookings steht für Unternehmen mit einem Office 365 Business Premium-Abonnement zur Verfügung.

## <a name="why-integrate-with-microsoft-bookings-using-microsoft-graph"></a>Vorteile der Integration von Microsoft Bookings mit Microsoft Graph

### <a name="streamline-appointment-booking"></a>Optimieren Terminvereinbarung
Der Betreiber eines Unternehmens verpasst keinen Kundentermin mehr, wenn er sich nicht in der Nähe des Telefons befindet oder das Geschäft geschlossen ist. Kunden können jederzeit direkt auf der Webseite für die Terminvereinbarung, auf der Webseite der Firma oder auf Facebook [die angebotenen Dienstleistungen sehen](/graph/api/bookingbusiness-list-services?view=graph-rest-beta) und [einen Termin vereinbaren](/graph/api/bookingbusiness-post-appointments?view=graph-rest-beta). 

Der Betreiber des Unternehmens kann jederzeit Termin vereinbaren, ob über das Internet, in der Mobilgeräte-App, persönlich oder telefonisch. Er kann einen Termin [neu vereinbaren](/graph/api/bookingappointment-update?view=graph-rest-beta), [absagen](/graph/api/bookingappointment-cancel?view=graph-rest-beta) oder einem verfügbaren Mitarbeiter [neu zuweisen](/graph/api/bookingappointment-update?view=graph-rest-beta). 

### <a name="reduce-no-shows-and-increase-productivity-of-the-staff"></a>Keine verpassten Termine mehr und höhere Produktivität der Mitarbeiter
Der Betreiber eines Unternehmens kann [Richtlinien für die Terminvergabe](/graph/api/resources/bookingschedulingpolicy?view=graph-rest-beta) festlegen, die eine Mindestvorlaufzeit für Terminvereinbarungen und -absagen beinhalten, sodass Kunden ihre Termine eigenständig planen und umplanen können. Automatisierte Terminbestätigungen und Erinnerungen verringern die Anzahl nicht eingehaltener Termine und ermöglichen den Mitarbeitern, ihren Arbeitsstunden besser zu nutzen. 

### <a name="manage-customer-information-and-relationships-from-anywhere"></a>Verwalten der Kundeninformationen und -beziehungen von überall
Nach dem Termin wird automatisch überprüft, ob der Kunden bereits in der [Kundenliste](/graph/api/bookingbusiness-list-customers?view=graph-rest-beta) vorhanden ist. Gegebenenfalls werden der Name des Kunden und die E-Mail-Adresse der Liste [hinzugefügt](/graph/api/bookingbusiness-post-customers?view=graph-rest-beta). Auf diese Weise kann der Betreiber eines Unternehmens einfache mit seinen Kunden in Kontakt bleiben und regelmäßig Newsletter oder andere Werbematerialien senden.

### <a name="integrate-with-productivity-and-team-collaboration-services-in-microsoft-graph"></a>Integration mit Diensten für die Produktivität und Teamzusammenarbeit in Microsoft Graph
Mit dem gleichen, einheitlichen Microsoft Graph-REST-Endpunkt können Sie auf die Bookings-API zugreifen und [eine Integration mit den besten Funktionen von Microsoft 365](overview-major-services.md) vornehmen, damit Sie noch umfangreichere Szenarien unterstützen können. Sie können beispielsweise [Excel](excel-concept-overview.md#generate-reports-and-analyze-results) verwenden, um die Finanzdaten des Unternehmens zu verfolgen, zu analysieren und professionelle Berichte zu erstellen, oder Sie können [SharePoint](sharepoint-concept-overview.md) oder [Microsoft Teams](teams-concept-overview.md) verwenden, um die Zusammenarbeit zu verbessern.

## <a name="api-reference"></a>API-Referenz
Suchen Sie die API-Referenz für diesen Dienst?

Weitere Informationen finden Sie unter [Microsoft Bookings-API in Microsoft Graph, Betaversion](/graph/api/resources/booking-api-overview?view=graph-rest-beta).


## <a name="next-steps"></a>Nächste Schritte

Weitere Informationen:

- 
  [Microsoft Bookings](https://support.office.com/de-DE/article/Publish-your-business-calendar-online-with-Microsoft-Bookings-47403d64-a067-4754-9ae9-00157244c27d) und andere [Office 365-Apps für Unternehmen](https://support.office.com/de-DE/article/manage-your-business-apps-in-the-business-center-47eca808-cf96-42ba-83e8-55daf18e49dc?ui=en-US&rs=en-US&ad=US).
- [Verwenden der Bookings-API](/graph/api/resources/booking-api-overview?view=graph-rest-beta) in Microsoft Graph.

