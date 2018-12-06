---
title: Microsoft-Teams-API (Übersicht)
description: 'Microsoft Teams ist der ultimative Hub für Zusammenarbeit und intelligente Kommunikation. '
ms.openlocfilehash: 1f210bf529769c96f22c2c7180d3736cdc9ed776
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092252"
---
# <a name="microsoft-teams-api-overview"></a>Microsoft-Teams-API (Übersicht)

[Microsoft-Teams,](https://products.office.com/microsoft-teams) ist der ultimative Hub für Zusammenarbeit und Kommunikation intelligent. Über 120 Millionen Benutzer auf die Stärke und Skalierung von [Office 365](https://products.office.com/) integriert, bietet Microsoft-Teams, Chat-basierte Zusammenarbeit, Besprechungen, Anrufe und Enterprise-VoIP-Funktionen.

## <a name="why-integrate-with-microsoft-teams"></a>Gründe für die Integration in Microsoft Teams

### <a name="automate-team-lifecycles"></a>Automatisieren von Teamlebenszyklen

Verwenden Sie Microsoft Graph zum [Erstellen eines neuen virtuellen Teams](/graph/api/team-put-teams?view=graph-rest-1.0) , wenn ein neues Problem Business, [Fügen Sie die richtigen Personen](/graph/api/group-post-members?view=graph-rest-1.0) , an das Team, tritt auf, und konfigurieren Sie das Team mit [Kanäle](/graph/api/channel-post?view=graph-rest-1.0), [Registerkarten](/graph/api/teamstab-add?view=graph-rest-1.0)und [apps](/graph/api/teamsappinstallation-add?view=graph-rest-1.0).
Wenn Sie das neue Team zusammen, um die Business-Problem, das Teamkalender [ein neues Ereignis hinzufügen](/graph/api/group-post-events?view=graph-rest-1.0) zu besprechen abrufen möchten.

![Automatisieren von Lebenszyklen Team durch Erstellen eines Teams, Hinzufügen von Mitgliedern und team-Besitzer, Konfigurieren von Einstellungen, Hinzufügen von Kanäle, Installieren von apps, Hinzufügen von Registerkarten, und archivieren oder Löschen von dem Team Zeitpunkt zu erfüllen.](images/teams-lifecycle.png)

Wenn das Unternehmen Problem behoben ist und das Team nicht mehr benötigen, verwenden Sie die Microsoft-Teams-API zum [archivieren](/graph/api/team-archive?view=graph-rest-1.0) oder [Löschen Sie](/graph/api/group-delete?view=graph-rest-1.0) das Team. Wenn Sie die maximale Dauer des Teams kennen bei der Erstellung, legen Sie eine [Ablaufrichtlinie für Office 365-Gruppe](https://support.office.com/en-us/article/office-365-group-expiration-policy-8d253fe5-0e09-4b3c-8b5e-f48def064733?ui=en-US&rs=en-US&ad=US) für das Team, mit das das Team gemäß der Richtlinie automatisch entfernt.

### <a name="get-work-done-even-when-no-one-is-around"></a>Arbeit in Ruhe erledigen, auch wenn niemand versehen ist.

Verwenden von [Anwendungsberechtigungen](permissions-reference.md) [Teams](/graph/api/resources/team?view=graph-rest-1.0), [Kanäle](/graph/api/resources/channel?view=graph-rest-1.0)und [Registerkarten](/graph/api/resources/teamstab?view=graph-rest-1.0) ohne Eingreifen entwickelt. Erstellen Sie einen neuen Kanal, wenn der Kunde einen Auftrag Dateien.
Automatisch Teams für Klassen am Anfang des Jahres Schule erstellen, und am Ende zu archivieren.

### <a name="create-teams-linked-to-your-app"></a>Erstellen von Teams, die an Ihrer app verknüpft

Lassen Sie Kunden um neue [Teams](/graph/api/resources/team?view=graph-rest-1.0) und [Kanäle](/graph/api/resources/channel?view=graph-rest-1.0)zu erstellen. 
[Installieren Sie](/graph/api/teamsappinstallation-add?view=graph-rest-1.0) Ihre [app Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/#pivot=home&panel=home-all) in die neue Teams. 
[Pin auf die Registerkarte an Ihrer app](/graph/api/teamstab-add?view=graph-rest-1.0) aus dem neuen Kanal. 
[Senden von Nachrichten](/graph/api/channel-post-chatthreads?view=graph-rest-beta) an den Kanal wieder auf Ihre Website verknüpfen.

### <a name="create-and-manage-multiple-teams-and-channels"></a>Erstellen und Verwalten von mehrere Teams und Kanäle

Microsoft Graph erleichtert die große Anzahl von Teams erstellen und Auffüllen mit Benutzern und Kanäle, erstellen und Verwalten von [Teams](/graph/api/resources/team?view=graph-rest-1.0), [Kanäle](/graph/api/resources/channel?view=graph-rest-1.0), [Registerkarten](/graph/api/resources/teamstab?view=graph-rest-1.0)und [apps](/graph/api/resources/teamsapp?view=graph-rest-1.0)automatisieren.
Microsoft Graph können Sie [Suchen](teams-list-all-teams.md) und [Archiv](/graph/api/team-archive?view=graph-rest-1.0) Teams, die Sie nicht mehr verwenden. Dies ist die gleiche API, die die [Microsoft-Teams Admin Center](https://docs.microsoft.com/en-us/microsoftteams/enable-features-office-365) und [Teams PowerShell-Cmdlets](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview) integriert sind.

### <a name="deploy-apps-to-teams"></a>Bereitstellen von apps für teams

[Auflisten der Teams in Ihrem Mandanten](teams-list-all-teams.md), und für diese [apps installieren](/graph/api/teamsappinstallation-add?view=graph-rest-1.0) . 
[Erstellen von Registerkarten](/graph/api/teamstab-add?view=graph-rest-1.0) in Kanäle Benutzern einfachen Zugriff auf apps gewähren können.

### <a name="use-microsoft-graph-in-any-kind-of-app"></a>Verwenden von Microsoft Graph in jeder Art von App

Microsoft-Teams, apps geben Arbeitsgruppen Sie ein neues Tool für die Zusammenarbeit eine produktivere und überzeugende Erfahrung vornehmen. Diese GruppenBenutzer arbeiten können apps Objekte freigeben, interagieren über Chat und Planen Sie Ereignisse im Kalender Team. Diese apps können auch Erstellen von Teams, Kanäle und Unterhaltungen, erweitern Sie den Wert der Microsoft-Teams von automatisieren.

Sie können Erstellen von Websites, Diensten und systemeigene Plattform-Anwendungen, die außerhalb der Benutzeroberfläche von Microsoft-Teams ausgeführt, und rufen die Teams-API zum Automatisieren von Teams Szenarien.

**Typen von Apps, die für Microsoft Teams aktiviert sind**

![Rufen Sie die Microsoft Teams-API von Registerkarten, Bots, Websites und Diensten auf.](images/teamsappendpoints.png)

Diese Tools für die Zusammenarbeit enthalten Microsoft Graph-aktivierten Registerkarten oder Bots, die innerhalb der Microsoft-Teams, apps. Sie können Microsoft Graph auch außerhalb einer Microsoft Teams-App aufrufen, z. B. von einer Website oder einem Webdienst aus. Wenn Sie Ihre Website bereits für Microsoft Graph aktiviert haben, können Sie die Funktionstüchtigkeit für Microsoft-Teams verwenden, verwenden Sie die [Microsoft-Teams, Developer-Plattform](https://docs.microsoft.com/en-us/microsoftteams/platform/#pivot=home&panel=home-all) zum [erstellen eine Registerkarte](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview) , die den vorhandenen Code für die Website verwendet.

Microsoft-Teams APIs können apps innerhalb und außerhalb von Teams verbessern:

|App-Typ|Szenariobeschreibung|
|:-------|:-------------------|
| [Tabs](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview) |Anzeigen des Inhalts im Microsoft-Teams.|
| [Bots](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/bots/bots-overview) |Helfen Sie Benutzern, Aufgaben in Unterhaltungen zu erledigen.|
| [Connectors](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/connectors/connectors) |Erstellen von Updates von externe Dienste für Kanäle.|
| [Aktionen fordernde Nachrichten](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/cards/cards) |Fügen Sie Ihren Connector-Karten verbesserte Interaktion hinzu.|
| [Messaging-Erweiterungen](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/messaging-extensions) |Ermöglicht es Benutzern, zum Abfragen und Freigeben von Informationen an Unterhaltungen.|
|Websites| Inhalte mit verbesserter Anzeige in Ihren Webseiten.|
|Dienste|Verbessern Sie Ihre Clientanwendungen mit Microsoft Graph-Daten über Ihren Webdienst.|
| [Aktivitätsfeed](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/activity-feed)|Benutzer über Feed-Benachrichtigungen einbeziehen.|
| [Aufrufen und online Meetings (Preview)](/graph/api/resources/calls-api-overview?view=graph-rest-beta) |Erstellen von Microsoft-Teams, apps mit Programmen, die initiieren und Audio/Videokonferenzen teilnehmen, Route/Übertragung basierend auf interactive Voice Response (IVR) fließt Anrufe und können an onlinebesprechungen teilnehmen.|

## <a name="api-reference"></a>API-Referenz

Suchen Sie nach der API-Referenz für diesen Dienst?

Finden Sie unter der [Teams-API in Microsoft Graph](/graph/api/resources/teams-api-overview?view=graph-rest-1.0).

## <a name="next-steps"></a>Nächste Schritte

- Sehen Sie sich [über lernübersichten](http://aka.ms/teamsgraph/v1/video).
- Erfahren Sie, wie Sie [die Microsoft Teams-API verwenden](/graph/api/resources/teams-api-overview?view=graph-rest-1.0).
- Führen Sie einen Drilldown für die Methoden, Eigenschaften und Beziehungen der Ressourcen [team](/graph/api/resources/team?view=graph-rest-1.0), [channel](/graph/api/resources/channel?view=graph-rest-1.0) und [group](/graph/api/resources/group?view=graph-rest-1.0) aus.
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.
- Erfahren Sie mehr über das [Microsoft Teams-Programmiermodell](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/concepts-overview).
- Verwenden Sie die [aufrufen und online-besprechungs-APIs](/graph/api/resources/calls-api-overview?view=graph-rest-beta).
- Ein neuer mit Beispielcode abrufen: [Contoso Airlines](https://github.com/microsoftgraph/contoso-airlines-teams-sample), [C#-Mini-Beispiele](https://github.com/microsoftgraph/csharp-teams-sample-graph)
