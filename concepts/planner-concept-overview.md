# <a name="planner-tasks-and-plans-api-overview"></a>Übersicht über Planner-Aufgaben und Pläne-API
Planner bietet Teams eine einfache und visuelle Möglichkeit, ihre Arbeit zu organisieren. Kunden können mit Planner Pläne erstellen, Aufgaben organisieren und zuweisen, Informationen zum Fortschritt teilen und Inhalte gemeinsam bearbeiten.  Planner bietet mehrere interaktive Oberfläche, darunter ein Task Board, eine Diagrammseite und eine Zeitplanansicht sowie Integrationen in Office 365.

**Task Board in Office 365 Planner**

![Screenshot eines Task Boards in Office 365 Planner](images/plannerboard.png "Bild des Planner-Boards")


## <a name="why-integrate-with-planner-tasks"></a>Vorteile der Integration mit Planner-Aufgaben
Planner bietet Funktionen zum Nachverfolgen von Aufgaben für die Zusammenarbeit in Office 365. Wenn Ihre Szenarien das Nachverfolgen von Aufgaben und Organisieren der Arbeit für ein Team oder eine Gruppe von Endbenutzern erfordert, ist Planner die richtige Wahl für Sie. Die Planner-Integration kann Sie dabei unterstützen, die Millionen von Benutzern zu erreichen, die in Office 365 zusammenarbeiten. 

### <a name="organize-your-teams-work"></a>Organisieren der Arbeit Ihres Teams
Planner bietet einen gemeinsamen Ort, an dem Sie ein Team zusammenstellen, [Aufgaben erstellen](../api-reference/v1.0/api/planner_post_tasks.md) und diese Aufgaben anderen im Team zuweisen können. Mit Planner weiß jeder immer, wer gerade was erledigt und ob die Aufgaben im Zeitplan liegen. Sie können Aufgaben mit zusätzlichen Informationen wie Fälligkeitsdaten, Fortschritt und Beschreibungen aktualisieren und die Aufgaben dann weiter mit anpassbaren Buckets und Kategoriebezeichnungen organisieren.   

### <a name="collaborate-across-office-365"></a>Zusammenarbeit in Office 365
Planner kann in die Oberfläche für die Zusammenarbeit in Office 365 integriert werden. Zusätzlich zu den Web- und Mobilgeräte-Clients von Planner können Benutzer Pläne und Aufgaben von Planner in SharePoint und Microsoft Teams anzeigen und aktualisieren.  

Der Microsoft Graph- und Office 365-Gruppendienst ergänzt Planner ebenfalls. Dateien, die Sie hochladen und an Planner-Aufgaben anfügen, werden in SharePoint gespeichert. Planner-Kommentare basieren auf Outlook-Gruppenunterhaltungen.

<!-- Add image
Note: Put an image here showing the relationship between Planner and other things
-->

### <a name="automate-the-creation-of-plans-and-tasks"></a>Automatisieren der Erstellung von Plänen und Aufgaben
Verwenden Sie sich wiederholende Prozesse oder Projekttypen? Mit der Planner-API können Sie das Erstellen eines Plans und eine Liste der Aufgaben automatisieren.  
 
## <a name="top-planner-api-tasks"></a>Wichtigste Aufgaben der Planner-API

|Vorgang|URL|
|:--------|:--|
|Anzeigen aller [Pläne](../api-reference/beta/resources/plannerplan.md) einer Gruppe|GET [https://graph.microsoft.com/v1.0/groups/{id}/planner/plans](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|Anzeigen aller [Aufgaben](../api-reference/beta/resources/plannertask.md) in einem Plan|GET [https://graph.microsoft.com/v1.0/planner/plans/{id}/tasks](https://developer.microsoft.com/en-us/graph/graph-explorer?request=planner/plans/{id}/tasks&version=v1.0)|
|Anzeigen aller [eigenen Aufgaben](../api-reference/beta/api/planneruser_list_tasks.md), die mir in Plänen zugewiesen sind|GET [https://graph.microsoft.com/v1.0/me/planner/tasks/](https://developer.microsoft.com/en-us/graph/graph-explorer?request=me/planner/tasks/&version=v1.0)|
|[Erstellen einer neuen Aufgabe](../api-reference/v1.0/api/planner_post_tasks.md)|POST [https://graph.microsoft.com/v1.0/planner/tasks](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|[Aktualisieren einer Aufgabe](../api-reference/v1.0/api/plannertask_update.md)|PATCH [https://graph.microsoft.com/v1.0/planner/tasks/{task-id}](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|
|[Löschen einer Aufgabe](../api-reference/v1.0/api/plannertask_delete.md)|DELETE [https://graph.microsoft.com/v1.0/planner/tasks/{id}](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups/{id}/planner/plans&version=v1.0)|


## <a name="next-steps"></a>Nächste Schritte

- [Verwenden der Planner-API](../api-reference/v1.0/resources/planner_overview.md)
- [Arbeiten mit Plänen](../api-reference/v1.0/resources/planner_overview.md#plans)
- [Arbeiten mit Aufgaben](../api-reference/v1.0/resources/planner_overview.md#tasks)
