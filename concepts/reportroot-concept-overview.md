---
title: Übersicht über die Berichts-API von Microsoft Graph
description: Anhand von Nutzungsberichten im Microsoft 365-Administrationscenter können Administratoren die Nutzung von Office 365-Diensten in ihrem Unternehmen besser verstehen. Mit der Berichts-API in Microsoft Graph haben Sie die Möglichkeit der Integration mit Office 365-Nutzungsberichten.
ms.openlocfilehash: d923d0003a276be15620998c53693a9bab7116d5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092285"
---
# <a name="microsoft-graph-reports-api-overview"></a>Übersicht über die Berichts-API von Microsoft Graph

Anhand von Nutzungsberichten im Microsoft 365-Administrationscenter können Administratoren die Nutzung von Office 365-Diensten in ihrem Unternehmen besser verstehen. Mit der Berichts-API in Microsoft Graph haben Sie die Möglichkeit der Integration mit Office 365-Nutzungsberichten.

## <a name="why-use-the-reports-api"></a>Warum sollte ich die Berichts-API verwenden?

### <a name="integrate-office-365-usage-reporting-into-your-organizations-existing-reporting-solution"></a>Integrieren von Office 365-Nutzungsberichten in die bestehende Berichterstellungslösung Ihres Unternehmens
Viele Unternehmen verfügen über bestehende Berichterstellungslösungen, die eine Anwendung oder ein Webportal zur Berichtserstellung nutzen. Mit der Berichts-API können Sie Office 365-Nutzungsdaten in die bestehende Berichterstellungslösung Ihres Unternehmens integrieren, sodass sich alle IT-Dienstberichte an einem zentralen Ort befinden.  

### <a name="retain-usage-reports-for-historical-analysis"></a>Aufbewahren von Nutzungsberichten für die Verlaufsanalyse
Mit der Berichts-API können Sie die Daten aus allen Nutzungsberichten abrufen, einschließlich Zusammenfassungen auf Unternehmensebene nach Dienst- und Entitätsebene (Benutzer, Sites, Konten) für die letzten 7/30/90/180 Tage sowie tägliche Aggregate. Auf diese Weise können Sie ältere Nutzungsdaten so lange wie erforderlich beibehalten.

## <a name="what-data-can-i-access-by-using-the-reports-api"></a>Auf welche Daten kann ich mit der Berichts-API zugreifen?

Mit der Berichts-API können Sie auf die in der folgenden Tabelle aufgeführten Datensätze zugreifen.

|Office 365-App|Datensatz|
|:--------|:--------|
|Microsoft Teams|[Gerätenutzung](/graph/api/resources/microsoft-teams-device-usage-reports?view=graph-rest-1.0)<br/>|[Benutzeraktivität](/graph/api/resources/microsoft-teams-user-activity-reports?view=graph-rest-1.0)|
|Office 365 (allgemein) |[Aktivierungen](/graph/api/resources/office-365-activations-reports?view=graph-rest-1.0)<br/>[Aktive Benutzer](/graph/api/resources/office-365-active-users-reports?view=graph-rest-1.0)<br/>[Gruppenaktivität](/graph/api/resources/office-365-groups-activity-reports?view=graph-rest-1.0)|
|OneDrive |[Aktivität](/graph/api/resources/onedrive-activity-reports?view=graph-rest-1.0)<br/>[Nutzung](/graph/api/resources/onedrive-usage-reports?view=graph-rest-1.0)|
|Outlook|[Aktivität](/graph/api/resources/email-activity-reports?view=graph-rest-1.0)<br/>[App-Nutzung](/graph/api/resources/email-app-usage-reports?view=graph-rest-1.0)<br/>[Postfachnutzung](/graph/api/resources/mailbox-usage-reports?view=graph-rest-1.0)|
|SharePoint |[Aktivität](/graph/api/resources/sharepoint-activity-reports?view=graph-rest-1.0)<br/>[Websiteverwendung](/graph/api/resources/sharepoint-site-usage-reports?view=graph-rest-1.0)|
|Skype for Business |[Aktivität](/graph/api/resources/skype-for-business-activity-reports?view=graph-rest-1.0)<br/>[Gerätenutzung](/graph/api/resources/skype-for-business-device-usage-reports?view=graph-rest-1.0)<br/>[Gerätenutzung](/graph/api/resources/skype-for-business-device-usage-reports?view=graph-rest-1.0)<br/>[Teilnehmeraktivität](/graph/api/resources/skype-for-business-participant-activity-reports?view=graph-rest-1.0)<br/>[Peer-to-Peer-Aktivität](/graph/api/resources/skype-for-business-peer-to-peer-activity?view=graph-rest-1.0)|
|Yammer |[Aktivität](/graph/api/resources/yammer-activity-reports?view=graph-rest-1.0)<br/>[Gerätenutzung](/graph/api/resources/yammer-device-usage-reports?view=graph-rest-1.0)<br/>[Gruppenaktivität](/graph/api/resources/yammer-groups-activity-reports?view=graph-rest-1.0)|

## <a name="api-reference"></a>API-Referenz
Suchen Sie die API-Referenz für diesen Dienst?

- [API für Office 365-Verwendungsberichte in Microsoft Graph v1.0](/graph/api/resources/report?view=graph-rest-1.0)
- [API für Office 365-Verwendungsberichte in Microsoft Graph, Betaversion](/graph/api/resources/report?view=graph-rest-beta)

## <a name="next-steps"></a>Nächste Schritte

* Sehen Sie sich die APIs im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) an.
* Weitere Informationen über die [Verwendung der REST-API für Berichte](/graph/api/resources/report?view=graph-rest-1.0).
