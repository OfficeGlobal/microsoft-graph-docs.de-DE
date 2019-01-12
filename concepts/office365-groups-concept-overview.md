---
title: Überblick über Office 365-Gruppen in Microsoft Graph
description: 'Office 365-Gruppen stellen den grundlegenden Mitgliedschaftsdienst für Benutzer bereit, um Unterhaltungen, Dateien, Notizen, Kalender, Pläne und viele andere Ressourcen freizugeben. '
author: dkershaw10
localization_priority: Priority
ms.prod: reports
ms.openlocfilehash: 3706c7373a80992cec1f920dbfdf5e8829829d10
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932709"
---
# <a name="overview-of-office-365-groups-in-microsoft-graph"></a>Überblick über Office 365-Gruppen in Microsoft Graph

Office 365-Gruppen stellen den grundlegenden Mitgliedschaftsdienst für Benutzer bereit, um Unterhaltungen, Dateien, Notizen, Kalender, Pläne und viele andere Ressourcen freizugeben. 

## <a name="why-integrate-with-office-365-groups"></a>Gründe für die Integration in Office 365-Gruppen   

Gruppen bilden die Grundlage, die eine Zusammenarbeit von Benutzern und Integration über Dienste hinweg ermöglicht, um vielfältige Szenarien bei der Aufgabenplanung, der Teamarbeit, der Bildung usw. zu unterstützen. Wenn Sie eine Integration in Office 365-Gruppen durchführen, kann Ihre Anwendung Millionen von Benutzer bei ihrem Übergang von verschiedenen Oberflächen in der Office 365-Suite und darüber hinaus unterstützen.  
 
### <a name="create-groups-to-facilitate-teamwork-across-services"></a>Erstellen von Gruppen zur Erleichterung der Teamarbeit über Dienste hinweg 
 
Sie können die Microsoft Graph-API verwenden, um Gruppen über den Lebenszyklus der Zusammenarbeit zu erstellen, zu verwalten oder zu löschen. So können Sie beispielsweise folgende Aktionen ausführen:  
 
- Verwenden Sie die API [Gruppe erstellen](/graph/api/group-post-groups?view=graph-rest-1.0), um eine neue Gruppe bereitzustellen. Die Gruppe wird dann in einem Bereich von Anwendungen, z. B. Outlook, SharePoint, Microsoft Teams, Planner und sogar Microsoft Stream, verfügbar gemacht. Microsoft Graph führt eine Synchronisierung über diese verbundenen Dienste hinweg durch, um allen Gruppenmitgliedern nahtlos Zugriff zu ermöglichen.  
 
    **Jede Office 365-Gruppe wird in einen Standardsatz von Office 365-Diensten integriert**

    ![Diagramm, in dem die Office 365-Gruppenintegration mit Dateien, Notizen, Aufgaben, Websites, Unterhaltungen und Kalender gezeigt wird.](images/office365-groups-concept-overview-related-services-infographic.png)  

- Geben Sie Mitgliedern die Möglichkeit anzuzeigen, dass sich eine Gruppe in ihren [Favoriten](/graph/api/group-addfavorite?view=graph-rest-1.0) befindet, oder [entfernen Sie sie ggf. aus ihren Favoriten](/graph/api/group-removefavorite?view=graph-rest-1.0). 
- Von Ihrer benutzerdefinierten Anwendung aus können Sie Gruppenunterhaltungen [erstellen](/graph/api/group-post-conversations?view=graph-rest-1.0), [abrufen](/graph/api/group-get-conversation?view=graph-rest-1.0) oder [löschen](/graph/api/group-delete-conversation?view=graph-rest-1.0). 
- Planen Sie Kalender[ereignisse](/graph/api/resources/event?view=graph-rest-1.0) im Gruppenkalender. 
- Rufen Sie Informationen zu der [SharePoint-Website](/graph/api/resources/site?view=graph-rest-1.0) ab, mit einer Gruppe zugewiesen ist, z B. die [Listen](/graph/api/list-list?view=graph-rest-1.0) oder [Unterwebsites](/graph/api/site-list-subsites?view=graph-rest-1.0) der Dokumentbibliothek. 
- [Erstellen Sie einen Plan](/graph/api/planner-post-buckets?view=graph-rest-1.0) in Planner, der im Besitz einer Gruppe ist. Der Plan bietet eine visuelle Möglichkeit zur Aufzeichnung der Teamarbeit, indem Sie [Aufgaben erstellen](/graph/api/planner-post-tasks?view=graph-rest-1.0) können, die [über Buckets hinweg organisiert](/graph/api/planner-post-buckets?view=graph-rest-1.0) werden können.  
- Greifen Sie auf das [OneNote](/graph/api/resources/onenote?view=graph-rest-1.0)-Notizbuch zu, das einer Gruppe zugewiesen ist, das zum Sammeln von Besprechungsnotizen und Organisationsideen verwendet werden kann. 
  
    **Office 365-Gruppen und Unterhaltungen in Outlook im Web**

    ![Screenshot von Outlook im Web mit aufgelisteten Gruppen im Ordner „Gruppen“](images/office365-groups-concept-overview-groups-in-outlook.png) 

- [Aktivieren einer Gruppe für Microsoft Teams](/graph/api/team-put-teams?view=graph-rest-beta) (Vorschau), damit Mitglieder an einem beständigen Chat teilnehmen können.  
- [Gruppen löschen](/graph/api/group-delete?view=graph-rest-1.0). Wenn eine Gruppe gelöscht wird, werden alle zugehörigen Inhalte ebenfalls gelöscht, wodurch verwaiste Websites, Unterhaltungen oder Pläne verhindert werden. 
 
### <a name="manage-group-membership-seamlessly"></a>Nahtloses Verwalten der Gruppenmitgliedschaft 
 
Office 365-Gruppen sind Auflistungen von Benutzern, die den Zugriff auf Ressourcen in Microsoft-Diensten oder in Ihrer App gemeinsam nutzen. Da die Gruppenmitgliedschaft zentral verwaltet wird, wirken sich Änderungen an der Mitgliedschaft auf alle Dienste aus, die mit der Gruppe verknüpft sind. Mit Microsoft Graph können Sie die folgenden Aufgaben für die Gruppenmitgliedschaftsaufgaben ausführen:
 
- [Hinzufügen](/graph/api/group-post-members?view=graph-rest-1.0) und [Entfernen](/graph/api/group-delete-members?view=graph-rest-1.0) von Mitgliedern aus einer vorhandenen Gruppe. 
- Abrufen einer [Liste von Besitzern](/graph/api/group-list-owners?view=graph-rest-1.0) oder einer [Liste von Mitgliedern](/graph/api/group-list-members?view=graph-rest-1.0) für eine Gruppe. Auf diese Weise kann kommuniziert werden, wer Zugriff auf Gruppeninhalte hat oder wer vielleicht administrative Aufgaben ausführen muss, z. B. Verlängern der Gruppe oder Genehmigen einer Beitrittsanfrage. 
- Festlegen von Gruppen als **Öffentlich**, wobei Gruppeninhalte für alle in der gleichen Organisation sichtbar sind, oder auf **Privat**, sodass Gruppeninhalte nur für Mitglieder sichtbar sind, über den Vorgang [Gruppe aktualisieren](/graph/api/group-update?view=graph-rest-1.0). 
- [Entfernen von Besitzern](/graph/api/group-delete-owners?view=graph-rest-1.0), die nicht mehr an den Besitzeraufgaben für eine bestimmte Gruppe aus der Liste von Gruppenbesitzern teilnehmen. 
 
### <a name="establish-and-maintain-group-policy-settings"></a>Einrichten und Verwalten von Gruppenrichtlinieneinstellungen 
 
Wenn die Anzahl von Gruppen, die in einer Organisation erstellt werden, wächst, unterstützt Microsoft Graph die Möglichkeit, die Nutzung und den Lebenszyklus der Gruppe zu steuern. Sie können über alle Gruppen innerhalb einer Organisation hinweg Gruppenrichtlinien erzwingen. Sie können die Microsoft Graph-API für Folgendes verwenden:

- Konfigurieren einer breiten Palette von [Gruppenrichtlinieneinstellungen](/graph/api/resources/groupsetting?view=graph-rest-1.0), mit denen Verhaltensweisen definiert werden, z. B. das automatische Löschen von Gruppen, sofern diese nicht von einem Besitzer verlängert werden, oder das Erzwingen von Benennungsrichtlinien für Office 365-Gruppen. 
- [Verlängern](/graph/api/group-renew?view=graph-rest-1.0) von Gruppen, die bald ablaufen, sodass Teammitglieder die Zusammenarbeit fortsetzen und weiterhin auf Inhalte zugreifen können. Wenn die Gruppe nicht gemäß der geltenden Ablaufrichtlinie verlängert wird, wird die Gruppe automatisch gelöscht. 
- Gelöschte Gruppen [wiederherstellen](/graph/api/directory-deleteditems-restore?view=graph-rest-1.0).

## <a name="api-reference"></a>API-Referenz
Suchen Sie die API-Referenz für diesen Dienst?

- [Gruppen-API in Microsoft Graph v1.0](/graph/api/resources/groups-overview?view=graph-rest-1.0)
- [Gruppen-API in Microsoft Graph, Betaversion](/graph/api/resources/groups-overview?view=graph-rest-beta)


## <a name="next-steps"></a>Nächste Schritte

- Testen Sie ein paar Beispiel-API-Anforderungen im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer). 
- Erfahren Sie mehr über die [Verwendung der Gruppen-API](/graph/api/resources/groups-overview?view=graph-rest-1.0) in Microsoft Graph.
