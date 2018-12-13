---
title: Übersicht über Microsoft Teams-APIs
description: 'Microsoft Teams ist der ultimative Hub für Zusammenarbeit und intelligente Kommunikation. '
ms.openlocfilehash: 1f210bf529769c96f22c2c7180d3736cdc9ed776
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092252"
---
# <a name="microsoft-teams-api-overview"></a>Übersicht über Microsoft Teams-APIs

[Microsoft Teams](https://products.office.com/microsoft-teams) ist der ultimative Hub für Zusammenarbeit und intelligente Kommunikation. Microsoft Teams, das auf den Stärken und der Größe von [Office 365](https://products.office.com/) aufbaut, bietet mit mehr als 120 Millionen von Benutzern chatbasierte Funktionen für Zusammenarbeit, Besprechungen, Anrufe sowie Enterprise-VoIP-Funktionen.

## <a name="why-integrate-with-microsoft-teams"></a>Gründe für die Integration in Microsoft Teams

### <a name="automate-team-lifecycles"></a>Automatisieren von Teamlebenszyklen

Verwenden Sie Microsoft Graph, um [ein neues virtuelles Team zu erstellen](/graph/api/team-put-teams?view=graph-rest-1.0), wenn sich ein neues Unternehmensproblem ergibt, [fügen Sie die entsprechenden Benutzer zum Team hinzu](/graph/api/group-post-members?view=graph-rest-1.0), und konfigurieren Sie das Team mit [Kanälen](/graph/api/channel-post?view=graph-rest-1.0), [Registerkarten](/graph/api/teamstab-add?view=graph-rest-1.0) und [Apps](/graph/api/teamsappinstallation-add?view=graph-rest-1.0).
Wenn Sie das neue Team zusammenbringen möchten, um das Unternehmensproblem zu besprechen, fügen Sie dem Teamkalender [ein neues Ereignis hinzu](/graph/api/group-post-events?view=graph-rest-1.0).

![Automatisieren Sie Teamlebenszyklen, indem Sie ein Team erstellen, Mitglieder und Besitzer hinzufügen, Teameinstellungen konfigurieren, Kanäle hinzufügen, Apps installieren, Registerkarten hinzufügen und das Team zum entsprechenden Zeitpunkt archivieren oder löschen.](images/teams-lifecycle.png)

Wenn das Unternehmensproblem gelöst wurde und Sie das Team nicht mehr benötigen, verwenden Sie die Microsoft Teams-API, um das Team zu [archivieren](/graph/api/team-archive?view=graph-rest-1.0) oder zu [löschen](/graph/api/group-delete?view=graph-rest-1.0). Wenn Sie die maximale Dauer des Teams bei der Erstellung kennen, legen Sie eine [Ablaufrichtlinie für die Office 365-Gruppe](https://support.office.com/en-us/article/office-365-group-expiration-policy-8d253fe5-0e09-4b3c-8b5e-f48def064733?ui=en-US&rs=en-US&ad=US) für das Team fest, durch die das Team gemäß der Richtlinie automatisch entfernt wird.

### <a name="get-work-done-even-when-no-one-is-around"></a>Effizientes Arbeiten, auch wenn niemand zur Stelle ist

Verwenden Sie [Anwendungsberechtigungen](permissions-reference.md) zum Arbeiten mit [Teams](/graph/api/resources/team?view=graph-rest-1.0), [Kanälen](/graph/api/resources/channel?view=graph-rest-1.0) und [Registerkarten](/graph/api/resources/teamstab?view=graph-rest-1.0) ohne menschliches Eingreifen. Erstellen Sie einen neuen Kanal, wenn Ihr Kunde eine Bestellung aufgibt.
Erstellen Sie automatisch Teams für Klassen am Anfang des Schuljahrs, und archivieren Sie sie am Ende.

### <a name="create-teams-linked-to-your-app"></a>Erstellen von Teams, die mit Ihrer App verknüpft sind

Ermöglichen Sie Kunden das Erstellen neuer [Teams](/graph/api/resources/team?view=graph-rest-1.0) und [Kanäle](/graph/api/resources/channel?view=graph-rest-1.0). 
[Installieren Sie ](/graph/api/teamsappinstallation-add?view=graph-rest-1.0) Ihre [Teams-App](https://docs.microsoft.com/de-DE/microsoftteams/platform/#pivot=home&panel=home-all) für neue Teams. 
[Heften Sie Ihre App an eine Registerkarte](/graph/api/teamstab-add?view=graph-rest-1.0) im neuen Kanal an. 
[Senden Sie Nachrichten](/graph/api/channel-post-chatthreads?view=graph-rest-beta) an den Kanal zurück, der mit Ihrer Website verknüpft ist.

### <a name="create-and-manage-multiple-teams-and-channels"></a>Erstellen und Verwalten mehrerer Teams und Kanäle

Mit Microsoft Graph können Sie ganz einfach große Anzahl Teams erstellen und diese mit Benutzern und Kanälen füllen, indem Sie das Erstellen und Verwalten von [Teams](/graph/api/resources/team?view=graph-rest-1.0), [Kanälen](/graph/api/resources/channel?view=graph-rest-1.0), [Registerkarten](/graph/api/resources/teamstab?view=graph-rest-1.0) und [Apps](/graph/api/resources/teamsapp?view=graph-rest-1.0) automatisieren.
Mit Microsoft Graph können Sie nach Teams, die nicht länger verwendet werden, [suchen](teams-list-all-teams.md) und diese [archivieren](/graph/api/team-archive?view=graph-rest-1.0). Dies ist die gleiche API, auf der [Microsoft Teams Admin Center](https://docs.microsoft.com/de-DE/microsoftteams/enable-features-office-365) und [PowerShell-Cmdlets für Teams](https://docs.microsoft.com/de-DE/microsoftteams/teams-powershell-overview) basieren.

### <a name="deploy-apps-to-teams"></a>Bereitstellen von Apps für Teams

[Führen Sie die Teams in Ihrem Mandanten auf](teams-list-all-teams.md), und [installieren Sie Apps](/graph/api/teamsappinstallation-add?view=graph-rest-1.0) für das Team. 
[Erstellen Sie Registerkarten](/graph/api/teamstab-add?view=graph-rest-1.0) in Kanälen, um Benutzern einfachen Zugriff auf Apps zu gewähren.

### <a name="use-microsoft-graph-in-any-kind-of-app"></a>Verwenden von Microsoft Graph in jeder Art von App

Microsoft Teams-Apps geben Arbeitsgruppen ein neues Tool an die Hand, um die Zusammenarbeit produktiver und interessanter zu gestalten. Mit diesen Apps können Arbeitsgruppenbenutzer Ressourcen freigeben, über Chats interagieren und Ereignisse im Teamkalender planen. Diese Apps können auch dabei helfen, das Erstellen von Teams, Kanälen und Unterhaltungen zur Steigerung des Werts von Microsoft Teams zu automatisieren.

Sie können Websites, Dienste und native Plattformanwendungen erstellen, die außerhalb der Benutzeroberfläche von Microsoft Teams ausgeführt werden, und die Teams-API aufrufen, um Teams-Szenarien zu automatisieren.

**Typen von Apps, die für Microsoft Teams aktiviert sind**

![Rufen Sie die Microsoft Teams-API von Registerkarten, Bots, Websites und Diensten auf.](images/teamsappendpoints.png)

Diese Zusammenarbeitstools umfassen Microsoft Graph-fähige Registerkarten oder Bots, die innerhalb von Microsoft Teams-Apps ausgeführt werden. Sie können Microsoft Graph auch außerhalb einer Microsoft Teams-App aufrufen, z. B. von einer Website oder einem Webdienst aus. Wenn Sie Ihre Website bereits für Microsoft Graph aktiviert haben, können Sie diese Arbeit für Microsoft Teams verwenden, indem Sie die [Microsoft Teams-Entwicklerplattform](https://docs.microsoft.com/de-DE/microsoftteams/platform/#pivot=home&panel=home-all) verwenden, um [eine Registerkarte zu erstellen](https://docs.microsoft.com/de-DE/microsoftteams/platform/concepts/tabs/tabs-overview), die den vorhandenen Websitecode verwendet.

Mit Microsoft Teams-APIs können Apps innerhalb und außerhalb von Teams verbessert werden:

|App-Typ|Szenariobeschreibung|
|:-------|:-------------------|
| [Registerkarten](https://docs.microsoft.com/de-DE/microsoftteams/platform/concepts/tabs/tabs-overview) |Gestalten Sie Ihre Inhalte in Microsoft Teams.|
| [Bots](https://docs.microsoft.com/de-DE/microsoftteams/platform/concepts/bots/bots-overview) |Helfen Sie Benutzern, Aufgaben in Unterhaltungen zu erledigen.|
| [Connectors](https://docs.microsoft.com/de-DE/microsoftteams/platform/concepts/connectors/connectors) |Stellen Sie Updates aus externen Diensten in Kanälen bereit.|
| [Aktionen erfordernde Nachrichten](https://docs.microsoft.com/de-DE/microsoftteams/platform/concepts/cards/cards) |Fügen Sie Ihren Connector-Karten verbesserte Interaktion hinzu.|
| [Messaging-Erweiterungen](https://docs.microsoft.com/de-DE/microsoftteams/platform/concepts/messaging-extensions) |Zulassen, dass Benutzer Informationen in Unterhaltungen abfragen und freigeben.|
|Websites| Inhalte mit verbesserter Anzeige in Ihren Webseiten.|
|Dienste|Verbessern Sie Ihre Clientanwendungen mit Microsoft Graph-Daten über Ihren Webdienst.|
| [Aktivitätsfeed](https://docs.microsoft.com/de-DE/microsoftteams/platform/concepts/activity-feed)|Benutzer über Feed-Benachrichtigungen einbeziehen.|
| [Anrufe und Onlinebesprechungen (Vorschau)](/graph/api/resources/calls-api-overview?view=graph-rest-beta) |Erstellen Sie Microsoft Teams-Apps mithilfe von Bots, die Audio-/Videoanrufe initiieren und an diesen teilnehmen, Anrufe basierend auf IVR-Flüssen (Interactive Voice Response) umleiten/weiterleiten und an Onlinebesprechungen teilnehmen können.|

## <a name="api-reference"></a>API-Referenz

Suchen Sie die API-Referenz für diesen Dienst?

Informationen hierzu finden Sie unter [Teams-API in Microsoft Graph](/graph/api/resources/teams-api-overview?view=graph-rest-1.0).

## <a name="next-steps"></a>Nächste Schritte

- Sehen Sie sich das [Übersichtsvideo](http://aka.ms/teamsgraph/v1/video) an.
- Erfahren Sie, wie Sie [die Microsoft Teams-API verwenden](/graph/api/resources/teams-api-overview?view=graph-rest-1.0).
- Führen Sie einen Drilldown für die Methoden, Eigenschaften und Beziehungen der Ressourcen [team](/graph/api/resources/team?view=graph-rest-1.0), [channel](/graph/api/resources/channel?view=graph-rest-1.0) und [group](/graph/api/resources/group?view=graph-rest-1.0) aus.
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.
- Erfahren Sie mehr über das [Microsoft Teams-Programmiermodell](https://docs.microsoft.com/de-DE/microsoftteams/platform/concepts/concepts-overview).
- Informieren Sie sich über die [Anruf- und Onlinebesprechungs-APIs](/graph/api/resources/calls-api-overview?view=graph-rest-beta).
- Schnelleinstieg mit Beispielcode: [Contoso Airlines](https://github.com/microsoftgraph/contoso-airlines-teams-sample), [Minibeispiele in C#](https://github.com/microsoftgraph/csharp-teams-sample-graph)
