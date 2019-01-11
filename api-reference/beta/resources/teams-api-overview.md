---
title: Verwenden der Microsoft Graph-API zum Arbeiten mit Microsoft Teams
description: Microsoft-Teams, ist ein Chat-basierten Arbeitsbereich in Office 365, das integrierte Zugriff auf Team-spezifischen Kalender, Dateien, OneNote-Notizen, Planner Pläne und bietet.
localization_priority: Priority
ms.openlocfilehash: 1e46bb3c31b30ec8ef776c4377bd391355abd50d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868677"
---
# <a name="use-the-microsoft-graph-api-to-work-with-microsoft-teams"></a>Verwenden der Microsoft Graph-API zum Arbeiten mit Microsoft Teams

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Microsoft-Teams, ist ein Chat-basierten Arbeitsbereich in Office 365, das integrierte Zugriff auf Team-spezifischen Kalender, Dateien, OneNote-Notizen, Planner Pläne und bietet.

## <a name="key-resources-in-microsoft-teams"></a>Wichtige Ressourcen im Microsoft-Teams

| Ressource | Methoden |
|:---------------|:--------|
|[Team](../resources/team.md)| [Ihren Teams bei der Liste](../api/user-list-joinedteams.md), [teams, die Liste alle](/graph/teams-list-all-teams), [Erstellen](../api/team-put-teams.md), [Lesen](../api/team-get.md), [Aktualisieren](../api/team-update.md), [Löschen](/graph/api/group-delete?view=graph-rest-1.0), [Wenn Sie den Klon](../api/team-clone.md), [Archiv](../api/team-archive.md), [entpackt](../api/team-unarchive.md) |
|[group](../resources/group.md)| [Mitglied hinzufügen](../api/group-post-members.md), [Entfernen von Mitgliedern](../api/group-delete-members.md), [Besitzer hinzufügen](../api/group-post-owners.md), [Entfernen Besitzer](../api/group-delete-owners.md), [Dateien abrufen](drive.md), [Notizbuch erhalten möchten](/graph/api/resources/notebook?view=graph-rest-1.0), [Pläne erhalten möchten](plannergroup.md), [Kalender erhalten möchten](event.md) |
|[DDE-Kanal](../resources/channel.md)|[Liste](../api/channel-list.md), [Erstellen](../api/channel-post.md), [Lesen](../api/channel-get.md), [Aktualisieren](../api/channel-patch.md), [Löschen](../api/channel-delete.md)|
|[teamsTab](../resources/teamstab.md) |[Liste](../api/teamstab-list.md), [Erstellen](../api/teamstab-add.md), [Lesen](../api/teamstab-get.md), [Aktualisieren](../api/teamstab-update.md), [Löschen](../api/teamstab-delete.md) |
|[teamsApp](../resources/teamsapp.md)|[Liste](../api/teamsapp-list.md), [Veröffentlichen](../api/teamsapp-publish.md), [Aktualisieren](../api/teamsapp-update.md), [Entfernen](../api/teamsapp-delete.md)|
|[teamsAppInstallation](../resources/teamsappinstallation.md)| [Liste](../api/teamsappinstallation-list.md), [Installieren](../api/teamsappinstallation-add.md), [Aktualisieren](../api/teamsappinstallation-delete.md), [Entfernen](../api/teamsappinstallation-delete.md) |
| (Vorschau) [ChatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) und [chatThread](/graph/api/resources/chatthread?view=graph-rest-beta) | [Liste](/graph/api/channel-list-messages?view=graph-rest-beta), [Erstellen](/graph/api/channel-post-chatthreads?view=graph-rest-beta), [Lesen](/graph/api/channel-get-message?view=graph-rest-beta) |
| (Vorschau) [rufen Sie](/graph/api/resources/call?view=graph-rest-beta) | [annehmen](/graph/api/call-answer?view=graph-rest-beta), [Ablehnen](/graph/api/call-reject?view=graph-rest-beta), [Umleiten](/graph/api/call-redirect?view=graph-rest-beta), [stumm schalten](/graph/api/call-mute?view=graph-rest-beta), [stummschaltung aufheben](/graph/api/call-unmute?view=graph-rest-beta), [Metadaten zu aktualisieren](/graph/api/call-updatemetadata?view=graph-rest-beta), [Ändern Bildschirmfreigabe Rolle](/graph/api/call-changescreensharingrole?view=graph-rest-beta), [Liste Teilnehmer](/graph/api/call-list-participants?view=graph-rest-beta), [Einladen von Teilnehmern](/graph/api/participant-invite?view=graph-rest-beta), [Stummschalten aller Teilnehmer](/graph/api/participant-muteall?view=graph-rest-beta) |

## <a name="teams-and-groups"></a>Teams und Gruppen

Microsoft-Teams, wird in Microsoft Graph wird durch ein [Group](../resources/group.md) -Ressource dargestellt. Microsoft-Teams und Office 365 Gruppen behandelt die verschiedenen Anforderungen der für die Gruppenzusammenarbeit. Fast alle Gruppen basierende Funktionen gelten für Microsoft-Teams und Office 365-Gruppen, wie für einen Gruppenkalender, Dateien, Notizen, Foto, Pläne, und so weiter. Der Hauptunterschied zwischen einem [Team](team.md) und einer Office 365-Gruppe ist die Kommunikation zwischen Mitgliedern. Teammitglieder kommunizieren per persistent Chat im Zusammenhang mit einem bestimmten Team. Office 365 Gruppenmitglieder kommunizieren, indem Sie Gruppe Unterhaltungen, die e-Mail-Unterhaltungen sind, die im Kontext einer Gruppe in Outlook auftreten.

Jede Gruppe, die ein Team hat hat eine **ResourceProvisioningOptions** -Eigenschaft, "Team" enthält. 

>**Hinweis:** Die **Group.resourceProvisioningOptions** -Eigenschaft kann geändert werden.
Hinzufügen oder Entfernen von "Team" aus der Auflistung nicht; Andernfalls erhalten Sie falsche Ergebnisse, wenn Sie alle Teams anbieten.

Im folgenden sind die Unterschiede zwischen Teams und Gruppen auf der Ebene der API:

- Beständiger Chat ist nur für Microsoft-Teams, verfügbar. Dieses Feature wird durch die Ressourcen [DDE-Kanal](../resources/channel.md), [ChatThread](../resources/chatthread.md)und [ChatMessage](../resources/chatmessage.md) hierarchisch dargestellt.
- Gruppendiskussionen stehen nur für Office 365-Gruppen. Dieses Feature wird durch die [Unterhaltung](../resources/conversation.md), [ConversationThread](../resources/conversationthread.md)und [Buchen von](../resources/post.md) Ressourcen hierarchisch dargestellt. 
- Die [Liste verknüpft Teams](../api/user-list-joinedteams.md) -Methode gilt nur für Microsoft-Teams.
- [Anrufe und onlinebesprechung APIs](./calls-api-overview.md) gelten nur für Microsoft-Teams.
- Siehe auch die [bekannte Probleme](/graph/known-issues) für diese APIs.

>**Hinweis:** Bei Verwendung von Gruppen API nicht in einer eigenständigen-app, sondern in einer [Microsoft-Teams, app](https://docs.microsoft.com/en-us/microsoftteams/platform/#apps-in-microsoft-teams) - Beispiel im Rahmen einer Registerkarte oder die Ausführung in Microsoft-Teams, Bot - befolgen Sie die Anweisungen im Artikel [Verwenden von Microsoft Graph in Ihren Microsoft-Teams, Seiten](https://docs.microsoft.com/en-us/microsoftteams/platform/resources/microsoft-graph).

## <a name="membership-changes-in-microsoft-teams"></a>Mitgliedschaftsänderungen in Microsoft-Teams

Um ein Team Mitgliedern und Besitzern hinzuzufügen, ändern Sie die Mitgliedschaft der [Gruppe](../resources/group.md) mit der gleichen ID.

| Anwendungsfall      | Aktion      | URL |
| ------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Mitglied hinzufügen](../api/group-post-members.md)    | POST      | /Groups/ {Id} /members/$ ref  |
| [Mitglied entfernen](../api/group-delete-members.md)   | DELETE    | /Groups/ {Id} /members/ {Benutzer-ID} / $ref |
| [Add owner](../api/group-post-owners.md)     | POST       | /Groups/ {Id} /owners/$ ref |
| [Besitzer entfernen](../api/group-delete-owners.md) | DELETE    | /Groups/ {Id} /owners/ {Benutzer-ID} / $ref |
| [Update-team](../api/team-update.md)  | PATCH     | /Teams/ {Id} |

Es wird empfohlen, wenn Sie einen Besitzer hinzufügen, auch diesen Benutzer als Mitglied hinzuzufügen. Wenn ein Team einen Besitzer, der kein Mitglied ist umfasst, möglicherweise Änderungen des websitebesitzes und der Mitgliedschaft nicht sofort in Microsoft-Teams angezeigt wird. Darüber hinaus wird verschiedene apps und APIs, die unterschiedlich behandelt. Microsoft-Teams, beispielsweise zeigt Teams an, dass der Benutzer ein Element oder Besitzer, ist die Microsoft-Teams PowerShell-Cmdlets und/me/JoinedTeams API Teams nur angezeigt wird, den, denen der Benutzer Mitglied ist. Um Verwechslungen zu vermeiden, fügen Sie alle Besitzer sowie der Liste Elemente hinzu. 

Bekanntes Problem: Wenn löschen /groups/ {Id} / Besitzer aufgerufen wird, der Benutzer auch aus der /groups/ {Id} entfernt / Mitgliederliste. Zum Umgehen dieses Problems wird empfohlen, entfernen Sie den Benutzer aus der Besitzer und Mitglieder, und klicken Sie dann warten Sie 10 Sekunden und dann wieder an Mitglieder hinzufügen.

Beim Hinzufügen und Entfernen von Mitgliedern und Besitzern, setzen Sie keiner geschweifte Klammern {}, um die-ID.

| Speed | Syntax | 
| ------ | ----- |
| Schnell | https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/members/48d31887-5fad-4d73-a9f5-3c356e68a038/$ref | 
| Langsam | https://graph.microsoft.com/beta/groups/{02bd9fd6-8f93-4758-87c3-1fb73740a315}/members/{48d31887-5fad-4d73-a9f5-3c356e68a038}/$ref | 

Auf ähnliche Weise, wenn die `userId` in die URL oder Nutzlast ausgedrückt als UPN statt als GUID, die Leistung langsamer sein.

| Speed | Syntax | 
| ------ | ----- |
| Schnell | 48d31887-5fad-4d73-a9f5-3c356e68a038 | 
| Langsam | John@example.com | 

Wenn Sie der Pfad langsamere ausgeführt wird, wenn ein Teammitglied aktuelle oder Besitzer auf der Microsoft-Teams Anwendung/Website angemeldet ist, wird die Änderung innerhalb einer Stunde übernommen.
Wenn keine dieser Benutzer auf die Microsoft-Teams Anwendung/Website angemeldet sind, wird die Änderung nicht übernommen werden, bis eine Stunde nach einer von ihnen anmeldet.

## <a name="see-also"></a>Siehe auch

[Übersicht über Microsoft Teams-APIs](/graph/teams-concept-overview)
