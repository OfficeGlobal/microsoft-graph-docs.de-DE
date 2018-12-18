---
title: Wesentliche Dienste und Features in Microsoft Graph
description: 'Mit Microsoft Graph können Sie mithilfe von REST-APIs und Clientbibliotheken die besten Funktionen aus Office 365, Windows 10 und Enterprise Mobility and Security Services in Microsoft 365 integrieren. Darüber hinaus bietet es Sicherheitsinformationen und Informationen aus sozialen Netzwerken, mit denen Sie die Produktivität der Benutzer, die Kreativität und die Zusammenarbeit im Team steigern und Unternehmensressourcen sowie Benutzerdaten schützen können. '
author: jthake-msft
ms.openlocfilehash: 6f4403db3179afadb39dfb20613f284381650112
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353550"
---
# <a name="major-services-and-features-in-microsoft-graph"></a>Wesentliche Dienste und Features in Microsoft Graph

Mit Microsoft Graph können Sie mithilfe von REST-APIs und Clientbibliotheken die besten Funktionen aus Office 365, Windows 10 und Enterprise Mobility and Security Services in Microsoft 365 integrieren. Darüber hinaus bietet es Sicherheitsinformationen und Informationen aus sozialen Netzwerken, mit denen Sie die Produktivität der Benutzer, die Kreativität und die Zusammenarbeit im Team steigern und Unternehmensressourcen sowie Benutzerdaten schützen können. 

## <a name="users-and-groups"></a>Benutzer und Gruppen

Den Kern von Microsoft Graph bilden die Konzepte „Benutzer“ und „Gruppe“. 

Ein _Benutzer_ in Microsoft Graph ist einer der Millionen Benutzer, die die Microsoft 365-Clouddienste nutzen. Der Benutzer ist der Fokus, dessen Identität stets gut geschützt und dessen Zugriff optimal verwaltet wird. Die Daten des Benutzers treiben das Unternehmen voran. Die Dienste von Microsoft Graph stellen diese Daten Unternehmen in umfangreichen Kontexten, in Echtzeitaktualisierungen und tiefgehenden Einblicken bereit, und das immer nur mit den entsprechenden Berechtigungen.

In Office 365 ist eine _Gruppe_ die grundlegende Entität, die die Zusammenarbeit der Benutzer ermöglicht. Sie kann mit anderen Diensten integriert werden und ermöglicht so umfassendere Szenarien für die Aufgabenplanung, Teamarbeit, Bildungseinrichtungen und vieles mehr. 

|Feature     |Unterstützende Dienste  |Beschreibung |Weitere Informationen |
|:-----------|:--------------------|:-----------|:----------------|
| Benutzer | Azure AD und die meisten Dienste für Produktivität, Zusammenarbeit, Intelligence und Bildung | Der Benutzer ist in Microsoft Graph von zentraler Bedeutung, und viele Dienste von Microsoft Graph sind um Benutzerfunktionen herum aufgebaut. | [Überblick über Benutzer in Microsoft Graph](azuread-users-concept-overview.md)|
|Gruppen | Azure AD, OneDrive, OneNote, Outlook, Planner | Eine Office 365-Gruppe stellt die grundlegende Einheit zur Zusammenarbeit dar, in der Benutzer Unterhaltungen, Dateien, Kalender, Notizen, Kalender, Pläne und vieles mehr gemeinsam nutzen. | [Überblick über Office 365-Gruppen in Microsoft Graph](office365-groups-concept-overview.md) |

## <a name="connecting-users-data-microsoft-365-services-and-your-apps"></a>Verbinden von Benutzerdaten, Microsoft 365-Diensten und Ihren Apps

Mit den Benutzern und Gruppen als Basis bildet Microsoft Graph ein Netzwerk von Microsoft 365-Diensten und -Features, die Daten verwalten, schützen und extrahieren und so eine breite Palette von Szenarien unterstützen. Mit Microsoft Graph können Sie auf diese Fülle von Benutzerdaten zugreifen und dabei immer die ordnungsgemäße Autorisierung berücksichtigen.

![Microsoft Graph stellt die Verbindung zu den Benutzerdaten her](images/microsoft-graph-connects-users-data.png)

### <a name="services-and-features"></a>Dienste und Features

Einige Dienste werden in Microsoft Graph erstmal zur Verfügung gestellt, andere sind bereits länger als eigenständige Dienste bekannt und sind nun Bestandteil von Microsoft Graph. Die API-Sätze folgen einem optimierten Design, wie in den [Microsoft-REST-API-Richtlinien](https://github.com/Microsoft/api-guidelines) dargelegt. Auf sie kann nun über einen einzelnen Microsoft Graph-REST-Endpunkt zugegriffen werden`https://graph.microsoft.com`. Im restlichen Teil dieses Artikels sind die wichtigsten Dienste und Features nach Kategorie aufgelistet. 


## <a name="identity-and-access-management"></a>Identitäts- und Zugriffsverwaltung

|Feature     |Unterstützende Dienste  |Beschreibung |Weitere Informationen |
|:-----------|:--------------------|:-----------|:----------------|
| Identitäts- und Zugriffsverwaltung | Azure AD | Erstellt und verwaltet Directory-Ressourcen wie Benutzer, Gruppen und Anwendungen. Verwaltet den Zugriff auf Ressourcen und Daten. Bietet Kunden Zugriff auf Anmeldungs- und Kontorisikodaten in Azure AD.| [Überblick über die Azure AD-Identitäts- und Zugriffsverwaltung](azuread-identity-access-management-concept-overview.md)  |


## <a name="productivity"></a>Produktivität

|Feature     |Unterstützende Dienste  |Beschreibung |Weitere Informationen |
|:-----------|:--------------------|:-----------|:----------------|
| Kalender | Outlook  | Ermöglicht Benutzern, Termine und Besprechungen im Web, auf mobilen Geräten und Desktops zu planen. Teil des Outlook-Hubs für Messaging-Kommunikation in Office 365, das Benutzer die Verwaltung von E-Mails und Kontakten ermöglicht. | [Übersicht über den Outlook-Kalender](outlook-calendar-concept-overview.md)  |
| Dateien | OneDrive und SharePoint | Verwaltet Benutzerdateien in OneDrive und SharePoint und gibt Benutzerdateien frei. | [Übersicht über den OneDrive-Dateispeicher](onedrive-concept-overview.md) |
| E-Mail | Outlook | Ermöglicht Benutzern die Kommunikation, das Organisieren von Nachrichten und die Verwaltung von Prioritäten in ihren Workflows im Web, auf mobilen Geräten und Desktops. Teil des Outlook-Hubs für die Kommunikation in Office 365, das Benutzer die Verwaltung von Kontakten und das Planen von Besprechungen ermöglicht. | [Übersicht über Outlook-Mail](outlook-mail-concept-overview.md) |
| Anmerkungen | OneNote | Ermöglicht Benutzern das Planen und Organisieren von Ideen und Informationen. | [Übersicht über OneNote-Notizen](integrate-with-onenote.md) |
| Persönliche Kontakte | Outlook | Kontakteverwaltung im Web, auf mobilen Geräten und auf Desktops. Teil des Outlook-Hubs für Messaging-Kommunikation in Office 365, das Benutzer die Verwaltung von E-Mails und die Planung von Besprechungen ermöglicht.  | [Übersicht über persönliche Kontakte in Outlook](outlook-contacts-concept-overview.md) |
| Arbeitsmappen und Diagramme | Excel | Ermöglicht Benutzern die Verwendung von Excel-Tabellen zum Durchführen von komplexen Berechnungen, zum Nachverfolgen, Analysieren und Visualisieren von Daten und zum Erstellen von professionellen Berichten. | [Übersicht über Excel-Arbeitsmappen und die Diagramme](excel-concept-overview.md) |


## <a name="collaboration"></a>Zusammenarbeit

<!-- Want to update links to concept overviews as they are created over time. 
-->
|Feature     |Unterstützende Dienste  |Beschreibung |Weitere Informationen |
|:-----------|:--------------------|:-----------|:----------------|
| Websites und Listen  | SharePoint | Webbasierte Plattform für Benutzer und Office 365-Gruppen, um Inhalte zu teilen, organisieren, verwalten und zu ermitteln (einschließlich Listen, Dateien und Notizen). | [Übersicht über SharePoint-Websites und die -Inhalte](sharepoint-concept-overview.md) | 
|Aufgaben und Pläne | Planner | Ermöglicht Benutzern in Office 365-Gruppen, Pläne zu erstellen, Aufgaben zuzuweisen und den Fortschritt zu verfolgen. | [Übersicht über Pläne und Aufgaben in Planner](planner-concept-overview.md) |
|Teamarbeit |  Microsoft Teams | Digitaler Hub und Chat-basierter Arbeitsbereich für Teams zum Freigeben von Dateien, Notizen, Kalendern und Plänen. | [Überblick über die Teamarbeit in Microsoft Teams](teams-concept-overview.md) |


## <a name="social-intelligence-and-analytics"></a>Intelligence aus sozialen Netzwerken und Analysen

|Feature     |Unterstützende Dienste  |Beschreibung |Weitere Informationen |
|:-----------|:--------------------|:-----------|:----------------|
| Intelligence aus sozialen Netzwerken | Azure AD, Outlook, SharePoint und mehr | Ruft Informationen über Personen geordnet nach Relevanz für den Benutzer ab. Die Relevanz wird anhand der Kommunikations- und Zusammenarbeitsmuster des Benutzers und seiner Geschäftsbeziehungen ermittelt.  | [Intelligence aus sozialen Netzwerken in Microsoft Graph](social-intel-concept-overview.md) |
| Intelligence aus sozialen Netzwerken: Einblicke dokumentieren (Vorschau) | Delve, OneDrive, Outlook, SharePoint | Nutzt erweiterte Analysemethoden und maschinelles Lernen, um die Dokumente zu ermitteln, die für den Benutzer im Trend liegen, von ihm angezeigt, geändert oder geteilt wurden.  | [Intelligence aus sozialen Netzwerken in Microsoft Graph](social-intel-concept-overview.md)  |


## <a name="device-management"></a>Geräteverwaltung

|Feature     |Unterstützende Dienste  |Beschreibung |Weitere Informationen |
|:-----------|:--------------------|:-----------|:----------------|
|Geräte und Apps | Intune | Registriert und konfiguriert Geräte und verwaltet mobile Anwendungen in Ihrem Unternehmen. | [Überblick über Intune-Geräte und -Apps](intune-concept-overview.md) |


## <a name="security"></a>Sicherheit

|Feature     |Unterstützende Dienste  |Beschreibung |Weitere Informationen |
|:-----------|:--------------------|:-----------|:----------------|
| Sicherheitsintegration | Azure AD Identity Protection, Azure Information Protection, Azure Security Center, Microsoft Cloud-Anwendungssicherheit, Windows Defender Advanced Threat Protection und [weitere](/graph/api/resources/security-api-overview?view=graph-rest-1.0) | Stellt einen einheitlichen Zugang zu Sicherheitseinblicken und -aktionen bei Microsoft und seinen Partnern im Ökosystem bereit. | [Sicherheit in Microsoft Graph](security-concept-overview.md) |



## <a name="cross-device-experiences"></a>Geräteübergreifende Oberfläche

|Feature     |Unterstützende Dienste  |Beschreibung |Weitere Informationen |
|:-----------|:--------------------|:-----------|:----------------|
| Geräteübergreifende Oberfläche | Aktivitätsfeed, Geräte-Relay | Ermöglicht App-Funktionen, die über ein einzelnes Gerät hinausgehen und stattdessen mit dem Benutzer von Gerät zu Gerät wechseln, unabhängig von dessen Typ und Plattform. | [Übersicht über die geräteübergreifende Oberfläche](cross-device-concept-overview.md) |


## <a name="usage-reports"></a>Verwendungsberichte

|Feature     |Unterstützende Dienste  |Beschreibung |Weitere Informationen |
|:-----------|:--------------------|:-----------|:----------------|
| Berichte | Microsoft Teams, OneDrive, Outlook, SharePoint, Skype for Business, Yammer | Ruft Informationen zur Aktivität und Nutzung eines unterstützenden Diensts ab. | [Übersicht über Verwendungsberichte](reportroot-concept-overview.md) |


## <a name="education"></a>Schulung und Weiterbildung

|Feature     |Unterstützende Dienste  |Beschreibung |Weitere Informationen |
|:-----------|:--------------------|:-----------|:----------------|
| Schulung und Weiterbildung | Azure AD, Education | Bietet Informationen, die für Bildungsszenarien relevant sind, einschließlich Bildungseinrichtungen, Kurse, Schüler/Studenten, Lehrkräfte und Aufgaben. Ermöglicht ISVs das Erstellen von Anwendungen für Kurse, mit denen die Lehrkräfte Zeit sparen und die Zusammenarbeit im Team gefördert wird.  | [Übersicht über Education](education-concept-overview.md) |


## <a name="business-applications"></a>Geschäftsanwendungen

|Feature     |Unterstützende Dienste  |Beschreibung |Weitere Informationen |
|:-----------|:--------------------|:-----------|:----------------|
| Kundenterminvereinbarung (Vorschau) | Microsoft Bookings | Richtet sich an kleine Unternehmen, um ihren Kunden zu ermöglichen, Dienstleistungen direkt im Web oder über Facebook zu vereinbaren. Ermöglicht Betreibern von Unternehmen die Verwaltung von Kundenwünschen, Dienstleistungen und Preisen, Mitarbeiterlisten und Terminplänen sowie anderen allgemeinen Geschäftsinformationen. | [Übersicht über die Microsoft Bookings-API](booking-concept-overview.md) |


## <a name="next-steps"></a>Nächste Schritte

<!-- Need to update the destination page titles and URLs as Matt's v-team finalize on the examples and featured scenarios content 
-->

- Kreative Lösungen, die auf den Diensten in Microsoft Graph aufbauen und reale Kundenprobleme lösen, finden Sie in den [Beispielen](https://developer.microsoft.com/graph/examples).
- Sehen Sie im Inhaltsverzeichnis unter **Lernen** nach, um mehr über die Dienste und Features zu erfahren, die _Sie_ in Ihren Szenarien verwenden können.
- Starten Sie eine Beispielanforderung im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer).
- Nutzen Sie den [Schnellstart](https://developer.microsoft.com/graph/quick-start), um eine sofort ausführbare Beispiel-App einzurichten.
