---
title: Verwenden der Microsoft Graph-API zum Arbeiten mit Microsoft Teams
description: Microsoft Teams ist ein Chat-basierter Arbeitsbereich in Office 365, der integrierten Zugriff auf Team-spezifische Kalender, Dateien, OneNote-Notizen, Planner-Pläne und vieles mehr bietet.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 2f101560bf716fcb3455346f7d6a3e01912e5451
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523176"
---
# <a name="use-the-microsoft-graph-api-to-work-with-microsoft-teams"></a>Verwenden der Microsoft Graph-API zum Arbeiten mit Microsoft Teams

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Teams ist ein Chat-basierter Arbeitsbereich in Office 365, der integrierten Zugriff auf Team-spezifische Kalender, Dateien, OneNote-Notizen, Planner-Pläne und vieles mehr bietet.

## <a name="key-resources-in-microsoft-teams"></a>Wichtige Ressourcen in Microsoft Teams

| Ressource | Methoden |
|:---------------|:--------|
|[team](../resources/team.md)| [list your teams](../api/user-list-joinedteams.md), [list all teams](/graph/teams-list-all-teams), [create](../api/team-put-teams.md), [read](../api/team-get.md), [update](../api/team-update.md), [delete](/graph/api/group-delete?view=graph-rest-1.0), [clone](../api/team-clone.md), [archive](../api/team-archive.md), [unarchive](../api/team-unarchive.md) |
|[group](../resources/group.md)| [add member](../api/group-post-members.md), [remove member](../api/group-delete-members.md), [add owner](../api/group-post-owners.md), [remove owner](../api/group-delete-owners.md), [get files](drive.md), [get notebook](/graph/api/resources/notebook?view=graph-rest-1.0), [get plans](plannergroup.md), [get calendar](event.md) |
|[channel](../resources/channel.md)|[list](../api/channel-list.md), [create](../api/channel-post.md), [read](../api/channel-get.md), [update](../api/channel-patch.md), [delete](../api/channel-delete.md)|
|[teamsTab](../resources/teamstab.md) |[list](../api/teamstab-list.md), [create](../api/teamstab-add.md), [read](../api/teamstab-get.md), [update](../api/teamstab-update.md), [delete](../api/teamstab-delete.md) |
|[teamsApp](../resources/teamsapp.md)|[list](../api/teamsapp-list.md), [publish](../api/teamsapp-publish.md), [update](../api/teamsapp-update.md), [remove](../api/teamsapp-delete.md)|
|[teamsAppInstallation](../resources/teamsappinstallation.md)| [list](../api/teamsappinstallation-list.md), [install](../api/teamsappinstallation-add.md), [upgrade](../api/teamsappinstallation-delete.md), [remove](../api/teamsappinstallation-delete.md) |
| (Vorschau) [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) und [chatThread](/graph/api/resources/chatthread?view=graph-rest-beta) | [list](/graph/api/channel-list-messages?view=graph-rest-beta), [create](/graph/api/channel-post-chatthreads?view=graph-rest-beta), [read](/graph/api/channel-get-message?view=graph-rest-beta) |
| (Vorschau) [call](/graph/api/resources/call?view=graph-rest-beta) | [answer](/graph/api/call-answer?view=graph-rest-beta), [reject](/graph/api/call-reject?view=graph-rest-beta), [redirect](/graph/api/call-redirect?view=graph-rest-beta), [mute](/graph/api/call-mute?view=graph-rest-beta), [unmute](/graph/api/call-unmute?view=graph-rest-beta), [update metadata](/graph/api/call-updatemetadata?view=graph-rest-beta), [change screen sharing role](/graph/api/call-changescreensharingrole?view=graph-rest-beta), [list participants](/graph/api/call-list-participants?view=graph-rest-beta), [invite participants](/graph/api/participant-invite?view=graph-rest-beta), [mute all participants](/graph/api/participant-muteall?view=graph-rest-beta) |

## <a name="teams-and-groups"></a>Teams und Gruppen

In Microsoft Graph wird Microsoft Teams durch eine [group](../resources/group.md)-Ressource dargestellt. Sowohl Microsoft Teams- als auch Office 365-Gruppen erfüllen die unterschiedlichen Anforderungen der Zusammenarbeit in Gruppen. Fast alle gruppenbasierten Funktionen gelten sowohl für Microsoft Teams- als auch für Office 365-Gruppen, wie z. B. Gruppenkalender, Dateien, Notizen, Fotos, Pläne usw. Der Hauptunterschied zwischen einer [Team](team.md)- und Office 365-Gruppe ist der Kommunikationsmodus zwischen den Mitgliedern. Team-Mitglieder kommunizieren innerhalb eines beständigen Chats im Kontext eines bestimmten Teams. Office 365-Gruppenmitglieder kommunizieren in Gruppenunterhaltungen, wobei es sich um E-Mail-Kommunikationen handelt, die im Kontext einer Gruppe in Outlook ausgeführt werden.

Jede Gruppe, die über ein Team verfügt, besitzt die **ResourceProvisioningOptions**-Eigenschaft, die "Team" enthält. 

>**Hinweis:** Die **Group.resourceProvisioningOptions**-Eigenschaft kann geändert werden.
"Team" sollte nicht zu dieser Sammlung hinzugefügt oder aus ihr entfernt werden; andernfalls erhalten Sie bei der Auflistung aller Teams falsche Ergebnisse.

Im folgenden werden die Unterschiede zwischen Teams und Gruppen auf der API-Ebene aufgelistet:

- Beständiger Chat steht nur für Microsoft Teams zur Verfügung. Dieses Feature wird von den Ressourcen [channel](../resources/channel.md), [chatThread](../resources/chatthread.md) und [chatMessage](../resources/chatmessage.md) hierarchisch dargestellt.
- Gruppenunterhaltungen sind nur für Office 365-Gruppen verfügbar. Dieses Feature wird von den Ressourcen [conversation](../resources/conversation.md), [conversationThread](../resources/conversationthread.md) und [post](../resources/post.md) hierarchisch dargestellt. 
- Die [Liste joined teams](../api/user-list-joinedteams.md)-Methode gilt nur für Microsoft Teams.
- [Anruf- und Onlinebesprechungs-APIs](./calls-api-overview.md) gelten nur für Microsoft Teams.
- Weitere Informationen finden Sie im Abschnitt [Bekannte Probleme](/graph/known-issues) für diese APIs.

>Hinweis: Wenn Sie die Gruppen-APIs in einer Microsoft Teams-App und nicht in einer eigenständigen App verwenden, z. B. als Teil einer Registerkarte oder eines Bots, der in Microsoft Teams ausgeführt wird, folgen Sie den Anweisungen im Artikel Verwenden von Microsoft Graph in Ihren Microsoft Teams-Seiten.

## <a name="membership-changes-in-microsoft-teams"></a>Ändern der Mitgliedschaft in Microsoft Teams

Wenn Sie Mitglieder und Besitzer zu einem Team hinzufügen möchten, ändern Sie die Mitgliedschaft der [Gruppe](../resources/group.md) mit der gleichen ID.

| Anwendungsfall      | Verb      | URL |
| ------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Mitglied hinzufügen](../api/group-post-members.md)    | POST      | /groups/{id}/members/$ref  |
| [Mitglied entfernen](../api/group-delete-members.md)   | LÖSCHEN    | /groups/{id}/members/{userId}/$ref |
| [Besitzer hinzufügen](../api/group-post-owners.md)     | POST       | /groups/{id}/owners/$ref |
| [Besitzer entfernen](../api/group-delete-owners.md) | LÖSCHEN    | /groups/{id}/owners/{userId}/$ref |
| [Team aktualisieren](../api/team-update.md)  | PATCH     | /teams/{id} |

Wenn Sie einen Besitzer hinzufügen, sollten Sie diesen auch als Mitglied hinzufügen. Wenn ein Team über einen Besitzer verfügt, der kein Mitglied ist, werden Besitzer- und Mitgliedschaftsänderungen möglicherweise nicht sofort in Microsoft Teams angezeigt. Darüber hinaus wird dies je nach App oder API unterschiedlich behandelt. In Microsoft Teams werden z. B. Teams, in denen der Benutzer entweder Mitglied oder Besitzer ist, angezeigt, während die Microsoft Teams PowerShell-Cmdlets und die me/joinedTeams-API nur Teams anzeigt, in denen der Benutzer Mitglied ist. Um Verwirrung zu vermeiden, fügen Sie alle Besitzer auch zur Mitgliederliste hinzu. 

Bekanntes Problem: Wenn /groups/{Id}/owners LÖSCHEN aufgerufen wird, wird der Besitzer auch von der /groups/{Id}/members-Liste entfernt. Um dieses Problem zu umgehen, sollten Sie den Benutzer sowohl aus der Besitzer- als auch aus der Mitgliederliste entfernen, 10 Sekunden warten, und ihn dann wieder zur Liste der Mitglieder hinzufügen.

Fassen Sie die ID beim Hinzufügen und Entfernen von Mitgliedern und Besitzern nicht in geschweifte Klammern {} ein.

| Geschwindigkeit | Syntax | 
| ------ | ----- |
| Schnell | https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/members/48d31887-5fad-4d73-a9f5-3c356e68a038/$ref | 
| Langsam | https://graph.microsoft.com/beta/groups/{02bd9fd6-8f93-4758-87c3-1fb73740a315}/members/{48d31887-5fad-4d73-a9f5-3c356e68a038}/$ref | 

Wenn `userId` in der URL oder Nutzlast als UPN und nicht als GUID ausgedrückt wird, ist die Leistung geringer.

| Geschwindigkeit | Syntax | 
| ------ | ----- |
| Schnell | 48d31887-5fad-4d73-a9f5-3c356e68a038 | 
| Langsam | john@example.com | 

Wenn der langsamere Pfad ausgewählt wird und ein aktuelles Teammitglied oder ein Besitzer bei der Microsoft Teams-Anwendung/Website angemeldet ist, wird die Änderung innerhalb einer Stunde angezeigt.
Wenn keiner dieser Benutzer bei der Microsoft Teams- Anwendung/Website angemeldet ist, wird die Änderung erst eine Stunde nachdem sich einer dieser Benutzer angemeldet hat sichtbar.

## <a name="see-also"></a>Siehe auch

[Übersicht über Microsoft Teams-APIs](/graph/teams-concept-overview)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teams-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
