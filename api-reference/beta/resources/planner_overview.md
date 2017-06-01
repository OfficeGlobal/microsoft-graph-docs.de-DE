# <a name="planner"></a>Planner
Mit der Planner-API von Office 365 können Sie Aufgaben erstellen und Benutzern in einer Office 365-Gruppe zuweisen.

Bevor Sie mit der Arbeit in der Planner-API beginnen, sollten Sie wissen, wie die wichtigsten Objekte in der Planner-API zueinander und zu Office 365-Gruppen in Beziehung stehen.

## <a name="groups"></a>Gruppen
Office 365-Gruppen sind die Besitzer der Pläne in der Planner-API. Um [die im Besitz einer Gruppe befindlichen Pläne abzurufen](../api/plannergroup_list_plans.md), stellen Sie die folgende HTTP-Anforderung.

```http
GET /groups/{id}/planner/plans
```

Wenn Sie [einen neuen Plan erstellen](../api/planner_post_plans.md), definieren Sie eine Gruppe als dessen Besitzer, indem einfach die `owner`-Eigenschaft für ein Planobjekt festlegen. Pläne müssen im Besitz von Gruppen sein.

>**Hinweis:** Der Benutzer, der den Plan erstellt, muss ein Mitglied der Gruppe sein. Wenn Sie eine neue Gruppe mit der API erstellen, werden Sie nicht automatisch als Mitglied zur Gruppe hinzugefügt. Dieser Schritt muss mit einem separaten API-Aufruf ausgeführt werden.

## <a name="plans"></a>Pläne
[Pläne](plannerplan.md) sind die Container von [Aufgaben](plannertask.md). Um [eine Aufgabe in einem Plan zu erstellen](../api/planner_post_tasks.md), legen Sie die `planId`-Eigenschaft des Aufgabenobjekts beim Erstellen der Aufgabe auf die ID des Plans fest. Aufgaben können derzeit nicht ohne Pläne erstellt werden. Um [die Aufgaben in einem Plan abzurufen](../api/plannerplan_list_tasks.md), stellen Sie die folgende HTTP-Anforderung.

```http
GET /planner/plans/{id}/tasks
```

## <a name="tasks"></a>Aufgaben
Jede Aufgabe kann einem Benutzer zugewiesen werden, indem eine [Zuweisung](plannerassignment.md) in der [assignments](plannerassignments.md)-Eigenschaft des Aufgabenobjekts hinzugefügt wird. Die ID des Benutzers, dem die Aufgabe zugewiesen werden soll, ist der Name der offenen Eigenschaft von `assignments`, und die `orderHint`-Eigenschaft der Zuweisung muss angegeben werden.

## <a name="task-and-plan-details"></a>Aufgaben- und Plandetails 
Planner-Ressourcen sind in einfache Objekte und Detailobjekte unterteilt. Einfache Objekte bieten Zugriff auf allgemeine Eigenschaften der Ressourcen, geeignet für Listenansichten, während die Detailobjekte Zugriff auf umfassende Eigenschaften der Ressourcen bieten, die für Drilldownansichten geeignet sind.

## <a name="visualization"></a>Visualisierung
Neben Aufgaben- und Plandaten stellt die Planner-API auch Ressourcen für die allgemeine Visualisierung von Daten für alle Clients bereit. Für Aufgaben stehen mehrere Arten von Visualisierungsdaten zur Verfügung:

| Aufgaben werden angezeigt als      | Aufgaben werden sortiert mit Informationen aus|
|:------------------|:----------|
|Flache Liste (Aufgaben in einem Plan)| `orderHint`-Eigenschaft für Aufgaben|
|Flache Liste (einem Benutzer zugewiesene Aufgaben)| `assigneePriority`-Eigenschaft für Aufgaben|
|Boardansicht mit Spalten für Beauftragte (zugewiesen zum Task Board)| [assignedToTaskBoardTaskFormat](plannerassignedToTaskBoardTaskFormat.md)-Objekt|
|Boardansicht mit Spalten für den Fortschritt der Aufgabe auf dem Weg zur Fertigstellung (Fortschritts-Task Board)| [progressTaskBoardTaskFormat](plannerprogressTaskBoardTaskFormat.md)-Objekt|
|Boardansicht mit benutzerdefinierten Spalten von Aufgaben (Bucket-Task Board):|[bucketTaskBoardTaskFormat](plannerbucketTaskBoardTaskFormat.md)-Objekt|

Die benutzerdefinierten Spalten im Bucket-Task Board werden durch [bucket](plannerbucket.md)-Objekte dargestellt und ihre Reihenfolge durch die `orderHint`-Eigenschaft des Objekts.

Die gesamte Sortierung wird durch die unter [Verwenden von ORDER-Hinweisen in Planner ](planner_order_hint_format.md) genannten Grundsätze gesteuert.

## <a name="planner-resource-versioning"></a>Versionsverwaltung für Planner-Ressourcen

Planner verwendet für alle Ressourcen Etags zur Versionsverwaltung. Diese Etags werden mit der `@odata.etag`-Eigenschaft jeder Ressource zurückgegeben; in `PATCH`- und `DELETE`-Anforderungen muss das letzte dem Client bekannte Etag mit dem `If-Match`-Header angegeben werden. Planner erlaubt Änderungen an älteren Versionen von Ressourcen, sofern die beabsichtigte Änderung nicht in Konflikt mit neueren Änderungen steht, die vom Planner-Dienst für dieselbe Ressource akzeptiert wurden. Die Clients können ermitteln, welches Etag für eine bestimmte Ressource neuer ist, indem sie berechnen, welcher Etag-Wert in einem Vergleich von Ordnungszeichenfolgen größer ist. Jede Ressource verfügt über ein eigenes Etag. Etag-Werte für verschiedene Ressourcen, einschließlich solcher mit Einschlussbeziehungen, können nicht verglichen werden. Die Client-Apps müssen zwei Fehlerstatuscodes im Zusammenhang mit der Versionsverwaltung verarbeiten können (409 und 412), indem sie die aktuelle Version des Elements lesen und in Konflikt stehende Änderungen beheben.

## <a name="common-planner-error-conditions"></a>Häufige Planner-Fehlerbedingungen

Neben [allgemeinen Fehlern](../../../concepts/errors.md), die für Microsoft Graph gelten, sind einige Fehlerbedingungen für die Planner-API spezifisch.

### <a name="400-bad-request"></a>400 Ungültige Anforderung

Es gibt mehrere häufig auftretende Fälle, in denen für die `POST`- und `PATCH`- Anforderungen ein Statuscode 400 zurückgegeben werden kann. Zu den häufigen Problemen gehören:
* Eigenschaften mit offenem Typ weisen nicht den richtigen Typ auf, der Typ ist nicht angegeben oder sie enthalten keine Eigenschaften. Beispielsweise müssen [plannerAssignments](plannerAssignments.md)-Eigenschaften mit komplexen Werten die `@odata.type`-Eigenschaft mit dem Wert `microsoft.graph.plannerAssignment` deklarieren.
* Werte von Anordnungshinweisen weisen nicht das [richtige Format](planner_order_hint_format.md) auf. Beispiel: Ein Anordnungshinweiswert ist direkt auf den vom Client zurückgegebenen Wert festgelegt.
* Die Daten sind logisch inkonsistent. Beispiel: Das Startdatum einer Aufgabe liegt nach dem Fälligkeitsdatum der Aufgabe.

### <a name="403-forbidden"></a>403 Verboten

Zusätzlich zu den allgemeinen Fehlern gibt die Planner-API auch diesen Statuscode zurück, wenn ein von einem Dienst definierter Grenzwert überschritten wurde. In diesem Fall gibt die `code`-Eigenschaft des error-Ressourcentyps den Typ des Grenzwerts an, der von der Anforderung überschritten wurde. Die möglichen Werte für die Grenzwerttypen sind u. a.:

| Wert  | Beschreibung|
|:------------------|:----------|
|MaximumProjectsOwnedByUser|Der Grenzwert für die maximale Anzahl von Plänen, die im Besitz eines Gruppe sein können, wurde überschritten. Dieser Grenzwert basiert auf der `owner`-Eigenschaft der [plannerPlan](plannerPlan.md)-Ressource.|
|MaximumProjectsSharedWithUser|Der Grenzwert für die maximale Anzahl von Plänen, die für einen Benutzer freigegeben werden können, wurde überschritten.  Dieser Grenzwert basiert auf der `sharedWith`-Eigenschaft der [plannerPlanDetails](plannerPlanDetails.md)-Ressource.|
|MaximumTasksCreatedByUser|Der Grenzwert für die maximale Anzahl von Aufgaben, die von einem Benutzer erstellt werden können, wurde überschritten. Dieser Grenzwert basiert auf der `createdBy`-Eigenschaft der [plannerTask](plannerTask.md)-Ressource.|
|MaximumTasksAssignedToUser|Der Grenzwert für die maximale Anzahl von Aufgaben, die einem Benutzer zugewiesen werden können, wurde überschritten. Dieser Grenzwert basiert auf der `assignments`-Eigenschaft der [plannerTask](plannerTask.md)-Ressource.|
|MaximumTasksInProject|Der Grenzwert für die maximale Anzahl von Aufgaben in einem Plan wurde überschritten. Dieser Grenzwert basiert auf der `planId`-Eigenschaft der [plannerTask](plannerTask.md)-Ressource.|
|MaximumActiveTasksInProject|Der Grenzwert für die maximale Anzahl von nicht abgeschlossenen Aufgaben in einem Plan wurde überschritten. Dieser Grenzwert basiert auf den Eigenschaften `planId` und `percentComplete` der [plannerTask](plannerTask.md)-Ressource.|
|MaximumBucketsInProject|Der Grenzwert für die maximale Anzahl von Buckets in einem Plan wurde überschritten. Dieser Grenzwert basiert auf der `planId`-Eigenschaft der [plannerBucket](plannerBucket.md)-Ressource.|
|MaximumUsersSharedWithProject|Die `sharedWith`-Eigenschaft der [plannerPlanDetails](plannerPlanDetails.md)-Ressource enthält zu viele Werte.|
|MaximumReferencesOnTask|Die `references`-Eigenschaft der [plannerTaskDetails](plannerTaskDetails.md)-Ressource enthält zu viele Werte.|
|MaximumChecklistItemsOnTask|Die `checklist`-Eigenschaft der [plannerTaskDetails](plannerTaskDetails.md)-Ressource enthält zu viele Werte.|
|MaximumAssigneesInTasks|Die `assignments`-Eigenschaft der [plannerTask](plannerTask.md)-Ressource enthält zu viele Werte.|

### <a name="412-precondition-failed"></a>412 Fehler bei Vorbedingung 

Alle `POST`-, `PATCH`- und `DELETE` Anforderungen in der Planner-API erfordern, dass im `If-Match`-Header der letzte Etag-Wert der Ressource angegeben wird, für die die Anforderung gilt. Darüber hinaus kann der Statuscode 412 zurückgegeben werden, wenn der in der Anforderung angegeben Etag-Wert nicht mehr einer Version der Ressource im Dienst entspricht. In diesem Fall sollten die Clients die Ressource erneut lesen und ein neues Etag abrufen.

