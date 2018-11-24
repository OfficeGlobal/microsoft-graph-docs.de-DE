# <a name="use-the-microsoft-graph-api-to-work-with-microsoft-teams"></a>Verwenden der Microsoft Graph-API zum Arbeiten mit Microsoft Teams



Microsoft-Teams, ist ein Chat-basierten Arbeitsbereich in Office 365, das integrierte Zugriff auf Team-spezifischen Kalender, Dateien, OneNote-Notizen, Planner Pläne und bietet.

## <a name="key-resources-in-microsoft-teams"></a>Wichtige Ressourcen im Microsoft-Teams

| Ressource | Methoden |
|:---------------|:--------|
|[Team](../resources/team.md)| [Ihren Teams bei der Liste](../api/user_list_joinedteams.md), [teams, die Liste alle](../../../concepts/teams_list_all_teams.md), [Erstellen](../api/team_put_teams.md), [Lesen](../api/team_get.md), [Aktualisieren](../api/team_update.md), [Löschen](../../v1.0/api/group_delete.md), [Wenn Sie den Klon](../api/team_clone.md), [Archiv](../api/team_archive.md), [entpackt](../api/team_unarchive.md) |
|[Gruppe](../resources/group.md)| [Mitglied hinzufügen](../api/group_post_members.md), [Entfernen von Mitgliedern](../api/group_delete_members.md), [Besitzer hinzufügen](../api/group_post_owners.md), [Entfernen Besitzer](../api/group_delete_owners.md), [Dateien abrufen](drive.md), [Notizbuch erhalten möchten](../../v1.0/resources/notebook.md), [Pläne erhalten möchten](plannergroup.md), [Kalender erhalten möchten](event.md) |
|[DDE-Kanal](../resources/channel.md)|[Liste](../api/channel_list.md), [Erstellen](../api/channel_post.md), [Lesen](../api/channel_get.md), [Aktualisieren](../api/channel_patch.md), [Löschen](../api/channel_delete.md)|
|[teamsTab](../resources/teamstab.md) |[Liste](../api/teamstab_list.md), [Erstellen](../api/teamstab_add.md), [Lesen](../api/teamstab_get.md), [Aktualisieren](../api/teamstab_update.md), [Löschen](../api/teamstab_delete.md) |
|[teamsApp](../resources/teamsapp.md)|[Liste](../api/teamsapp_list.md), [Veröffentlichen](../api/teamsapp_publish.md), [Aktualisieren](../api/teamsapp_update.md), [Entfernen](../api/teamsapp_delete.md)|
|[teamsAppInstallation](../resources/teamsappinstallation.md)| [Liste](../api/teamsappinstallation_list.md), [Installieren](../api/teamsappinstallation_add.md), [Aktualisieren](../api/teamsappinstallation_delete.md), [Entfernen](../api/teamsappinstallation_delete.md) |
| (Vorschau) [ChatMessage](../../beta/resources/chatmessage.md) und [chatThread](../../beta/resources/chatthread.md) | [Liste](../../beta/api/channel_list_messages.md), [Erstellen](../../beta/api/channel_post_chatthreads.md), [Lesen](../../beta/api/channel_get_message.md) |
| (Vorschau) [rufen Sie](../../beta/resources/call.md) | [annehmen](../../beta/api/call_answer.md), [Ablehnen](../../beta/api/call_reject.md), [Umleiten](../../beta/api/call_redirect.md), [stumm schalten](../../beta/api/call_mute.md), [stummschaltung aufheben](../../beta/api/call_unmute.md), [Metadaten zu aktualisieren](../../beta/api/call_updatemetadata.md), [Ändern Bildschirmfreigabe Rolle](../../beta/api/call_changescreensharingrole.md), [Liste Teilnehmer](../../beta/api/call_list_participants.md), [Einladen von Teilnehmern](../../beta/api/participant_invite.md), [Stummschalten aller Teilnehmer](../../beta/api/participant_muteall.md) |

## <a name="teams-and-groups"></a>Teams und Gruppen

Microsoft-Teams, wird in Microsoft Graph wird durch ein [Group](../resources/group.md) -Ressource dargestellt. Microsoft-Teams und Office 365 Gruppen behandelt die verschiedenen Anforderungen der für die Gruppenzusammenarbeit. Fast alle Gruppen basierende Funktionen gelten für Microsoft-Teams und Office 365-Gruppen, wie für einen Gruppenkalender, Dateien, Notizen, Foto, Pläne, und so weiter. Der Hauptunterschied zwischen einem [Team](team.md) und einer Office 365-Gruppe ist die Kommunikation zwischen Mitgliedern. Teammitglieder kommunizieren per persistent Chat im Zusammenhang mit einem bestimmten Team. Office 365 Gruppenmitglieder kommunizieren, indem Sie Gruppe Unterhaltungen, die e-Mail-Unterhaltungen sind, die im Kontext einer Gruppe in Outlook auftreten.

Jede Gruppe, die ein Team hat hat eine **ResourceProvisioningOptions** -Eigenschaft, "Team" enthält. 

>**Hinweis:** Die **Group.resourceProvisioningOptions** -Eigenschaft kann geändert werden.
Hinzufügen oder Entfernen von "Team" aus der Auflistung nicht; Andernfalls erhalten Sie falsche Ergebnisse, wenn Sie alle Teams anbieten.

Im folgenden sind die Unterschiede zwischen Teams und Gruppen auf der Ebene der API:

- Die [Liste verknüpft Teams](../api/user_list_joinedteams.md) -Methode gilt nur für Microsoft-Teams.
- Siehe auch die [bekannte Probleme](../../../concepts/known_issues.md) für diese APIs.

>**Hinweis:** Bei Verwendung von Gruppen API nicht in einer eigenständigen-app, sondern in einer [Microsoft-Teams, app](https://docs.microsoft.com/en-us/microsoftteams/platform/#apps-in-microsoft-teams) - Beispiel im Rahmen einer Registerkarte oder die Ausführung in Microsoft-Teams, Bot - befolgen Sie die Anweisungen im Artikel [Verwenden von Microsoft Graph in Ihren Microsoft-Teams, Seiten](https://docs.microsoft.com/en-us/microsoftteams/platform/resources/microsoft-graph).

## <a name="membership-changes-in-microsoft-teams"></a>Mitgliedschaftsänderungen in Microsoft-Teams

Um ein Team Mitgliedern und Besitzern hinzuzufügen, ändern Sie die Mitgliedschaft der [Gruppe](../resources/group.md) mit der gleichen ID.

| Anwendungsfall      | Aktion      | URL |
| ------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Mitglied hinzufügen](../api/group_post_members.md)    | POST      | /Groups/ {Id} /members/$ ref  |
| [Mitglied entfernen](../api/group_delete_members.md)   | DELETE    | /Groups/ {Id} /members/ {Benutzer-ID} / $ref |
| [Add owner](../api/group_post_owners.md)     | POST       | /Groups/ {Id} /owners/$ ref |
| [Besitzer entfernen](../api/group_delete_owners.md) | DELETE    | /Groups/ {Id} /owners/ {Benutzer-ID} / $ref |
| [Update-team](../api/team_update.md)  | PATCH     | /Teams/ {Id} |

Es wird empfohlen, wenn Sie einen Besitzer hinzufügen, auch diesen Benutzer als Mitglied hinzuzufügen. Wenn ein Team einen Besitzer, der kein Mitglied ist umfasst, möglicherweise Änderungen des websitebesitzes und der Mitgliedschaft nicht sofort in Microsoft-Teams angezeigt wird. Darüber hinaus wird verschiedene apps und APIs, die unterschiedlich behandelt. Microsoft-Teams, beispielsweise zeigt Teams an, dass der Benutzer ein Element oder Besitzer, ist die Microsoft-Teams PowerShell-Cmdlets und/me/JoinedTeams API Teams nur angezeigt wird, den, denen der Benutzer Mitglied ist. Um Verwechslungen zu vermeiden, fügen Sie alle Besitzer sowie der Liste Elemente hinzu. 

Bekanntes Problem: Wenn löschen /groups/ {Id} / Besitzer aufgerufen wird, der Benutzer auch aus der /groups/ {Id} entfernt / Mitgliederliste. Zum Umgehen dieses Problems wird empfohlen, entfernen Sie den Benutzer aus der Besitzer und Mitglieder, und klicken Sie dann warten Sie 10 Sekunden und dann wieder an Mitglieder hinzufügen.

Beim Hinzufügen und Entfernen von Mitgliedern und Besitzern, setzen Sie keiner geschweifte Klammern {}, um die-ID.

| Speed | Syntax | 
| ------ | ----- |
| Schnell | https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/members/48d31887-5fad-4d73-a9f5-3c356e68a038/$ref | 
| Langsam | https://graph.microsoft.com/v1.0/groups/{02bd9fd6-8f93-4758-87c3-1fb73740a315}/members/{48d31887-5fad-4d73-a9f5-3c356e68a038}/$ref | 

Auf ähnliche Weise, wenn die `userId` in die URL oder Nutzlast ausgedrückt als UPN statt als GUID, die Leistung langsamer sein.

| Speed | Syntax | 
| ------ | ----- |
| Schnell | 48d31887-5fad-4d73-a9f5-3c356e68a038 | 
| Langsam | John@example.com | 

Wenn Sie der Pfad langsamere ausgeführt wird, wenn ein Teammitglied aktuelle oder Besitzer auf der Microsoft-Teams Anwendung/Website angemeldet ist, wird die Änderung innerhalb einer Stunde übernommen.
Wenn keine dieser Benutzer auf die Microsoft-Teams Anwendung/Website angemeldet sind, wird die Änderung nicht übernommen werden, bis eine Stunde nach einer von ihnen anmeldet.

## <a name="see-also"></a>Siehe auch

- [Microsoft-Teams-API (Übersicht)](../../../concepts/teams-concept-overview.md)
- Beispielcode: [Contoso Airlines](https://github.com/microsoftgraph/contoso-airlines-teams-sample), [C#-Mini-Beispiele](https://github.com/microsoftgraph/csharp-teams-sample-graph)
