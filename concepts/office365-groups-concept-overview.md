# <a name="overview-of-office-365-groups-in-microsoft-graph"></a>Überblick über Office 365-Gruppen in Microsoft Graph

Office 365-Gruppen stellen den grundlegenden Mitgliedschaftsdienst für Benutzer bereit, um Unterhaltungen, Dateien, Notizen, Kalender, Pläne und viele andere Ressourcen freizugeben. 

## <a name="why-integrate-with-office-365-groups"></a>Gründe für die Integration in Office 365-Gruppen   

Gruppen bilden die Grundlage, die eine Zusammenarbeit von Benutzern und Integration über Dienste hinweg ermöglicht, um vielfältige Szenarien bei der Aufgabenplanung, der Teamarbeit, der Bildung usw. zu unterstützen. Wenn Sie eine Integration in Office 365-Gruppen durchführen, kann Ihre Anwendung Millionen von Benutzer bei ihrem Übergang von verschiedenen Oberflächen in der Office 365-Suite und darüber hinaus unterstützen.  
 
### <a name="create-groups-to-facilitate-teamwork-across-services"></a>Erstellen von Gruppen zur Erleichterung der Teamarbeit über Dienste hinweg 
 
Sie können die Microsoft Graph-API verwenden, um Gruppen über den Lebenszyklus der Zusammenarbeit zu erstellen, zu verwalten oder zu löschen. So können Sie beispielsweise folgende Aktionen ausführen:  
 
- Verwenden Sie die API [Gruppe erstellen](../api-reference/v1.0/api/group_post_groups.md), um eine neue Gruppe bereitzustellen. Die Gruppe wird dann in einem Bereich von Anwendungen, z. B. Outlook, SharePoint, Microsoft Teams, Planner und sogar Microsoft Stream, verfügbar gemacht. Microsoft Graph führt eine Synchronisierung über diese verbundenen Dienste hinweg durch, um allen Gruppenmitgliedern nahtlos Zugriff zu ermöglichen.  
 
    **Jede Office 365-Gruppe wird in einen Standardsatz von Office 365-Diensten integriert**

    ![Diagramm, in dem die Office 365-Gruppenintegration mit Dateien, Notizen, Aufgaben, Websites, Unterhaltungen und Kalender gezeigt wird.](images/office365-groups-concept-overview-related-services-infographic.png)  

- Geben Sie Mitgliedern die Möglichkeit anzuzeigen, dass sich eine Gruppe in ihren [Favoriten](../api-reference/v1.0/api/group_addfavorite.md) befindet, oder [entfernen Sie sie ggf. aus ihren Favoriten](../api-reference/v1.0/api/group_removefavorite.md). 
- Von Ihrer benutzerdefinierten Anwendung aus können Sie Gruppenunterhaltungen [erstellen](../api-reference/v1.0/api/group_post_conversations.md), [abrufen](../api-reference/v1.0/api/group_get_conversation.md) oder [löschen](../api-reference/v1.0/api/group_delete_conversation.md). 
- Planen Sie Kalender[ereignisse](../api-reference/v1.0/resources/event.md) im Gruppenkalender. 
- Rufen Sie Informationen zu der [SharePoint-Website](../api-reference/v1.0/resources/site.md) ab, mit einer Gruppe zugewiesen ist, z B. die [Listen](../api-reference/v1.0/api/list_list.md) oder [Unterwebsites](../api-reference/v1.0/api/site_list_subsites.md) der Dokumentbibliothek. 
- [Erstellen Sie einen Plan](../api-reference/v1.0/api/planner_post_buckets.md) in Planner, der im Besitz einer Gruppe ist. Der Plan bietet eine visuelle Möglichkeit zur Aufzeichnung der Teamarbeit, indem Sie [Aufgaben erstellen](../api-reference/v1.0/api/planner_post_tasks.md) können, die [über Buckets hinweg organisiert](../api-reference/v1.0/api/planner_post_buckets.md) werden können.  
- Greifen Sie auf das [OneNote](../api-reference/v1.0/resources/onenote.md)-Notizbuch zu, das einer Gruppe zugewiesen ist, das zum Sammeln von Besprechungsnotizen und Organisationsideen verwendet werden kann. 
  
    **Office 365-Gruppen und Unterhaltungen in Outlook im Web**

    ![Screenshot von Outlook im Web mit aufgelisteten Gruppen im Ordner „Gruppen“](images/office365-groups-concept-overview-groups-in-outlook.png) 

- [Aktivieren einer Gruppe für Microsoft Teams](../api-reference/beta/api/team_put_teams.md) (Vorschau), damit Mitglieder an einem beständigen Chat teilnehmen können.  
- [Gruppen löschen](../api-reference/v1.0/api/group_delete.md). Wenn eine Gruppe gelöscht wird, werden alle zugehörigen Inhalte ebenfalls gelöscht, wodurch verwaiste Websites, Unterhaltungen oder Pläne verhindert werden. 
 
### <a name="manage-group-membership-seamlessly"></a>Nahtloses Verwalten der Gruppenmitgliedschaft 
 
Office 365-Gruppen sind Auflistungen von Benutzern, die den Zugriff auf Ressourcen in Microsoft-Diensten oder in Ihrer App gemeinsam nutzen. Da die Gruppenmitgliedschaft zentral verwaltet wird, wirken sich Änderungen an der Mitgliedschaft auf alle Dienste aus, die mit der Gruppe verknüpft sind. Mit Microsoft Graph können Sie die folgenden Aufgaben für die Gruppenmitgliedschaftsaufgaben ausführen:
 
- [Hinzufügen](../api-reference/v1.0/api/group_post_members.md) und [Entfernen](../api-reference/v1.0/api/group_delete_members.md) von Mitgliedern aus einer vorhandenen Gruppe. 
- Abrufen einer [Liste von Besitzern](../api-reference/v1.0/api/group_list_owners.md) oder einer [Liste von Mitgliedern](../api-reference/v1.0/api/group_list_members.md) für eine Gruppe. Auf diese Weise kann kommuniziert werden, wer Zugriff auf Gruppeninhalte hat oder wer vielleicht administrative Aufgaben ausführen muss, z. B. Verlängern der Gruppe oder Genehmigen einer Beitrittsanfrage. 
- Festlegen von Gruppen als **Öffentlich**, wobei Gruppeninhalte für alle in der gleichen Organisation sichtbar sind, oder auf **Privat**, sodass Gruppeninhalte nur für Mitglieder sichtbar sind, über den Vorgang [Gruppe aktualisieren](../api-reference/v1.0/api/group_update.md). 
- [Entfernen von Besitzern](../api-reference/v1.0/api/group_delete_owners.md), die nicht mehr an den Besitzeraufgaben für eine bestimmte Gruppe aus der Liste von Gruppenbesitzern teilnehmen. 
 
### <a name="establish-and-maintain-group-policy-settings"></a>Einrichten und Verwalten von Gruppenrichtlinieneinstellungen 
 
Wenn die Anzahl von Gruppen, die in einer Organisation erstellt werden, wächst, unterstützt Microsoft Graph die Möglichkeit, die Nutzung und den Lebenszyklus der Gruppe zu steuern. Sie können über alle Gruppen innerhalb einer Organisation hinweg Gruppenrichtlinien erzwingen. Sie können die Microsoft Graph-API für Folgendes verwenden:

- Konfigurieren einer breiten Palette von [Gruppenrichtlinieneinstellungen](../api-reference/v1.0/resources/groupsetting.md), mit denen Verhaltensweisen definiert werden, z. B. das automatische Löschen von Gruppen, sofern diese nicht von einem Besitzer verlängert werden, oder das Erzwingen von Benennungsrichtlinien für Office 365-Gruppen. 
- [Verlängern](../api-reference/v1.0/api/group_renew.md) von Gruppen, die bald ablaufen, sodass Teammitglieder die Zusammenarbeit fortsetzen und weiterhin auf Inhalte zugreifen können. Wenn die Gruppe nicht gemäß der geltenden Ablaufrichtlinie verlängert wird, wird die Gruppe automatisch gelöscht. 
- Gelöschte Gruppe [wiederherstellen](../api-reference/v1.0/api/directory_deleteditems_restore.md).
 
## <a name="next-steps"></a>Nächste Schritte

- Testen Sie ein paar Beispiel-API-Anforderungen im [Graph-Tester](https://developer.microsoft.com/de-DE/graph/graph-explorer). 
- Erfahren Sie mehr über die [Verwendung der Gruppen-API](../api-reference/v1.0/resources/groups-overview.md) in Microsoft Graph.
