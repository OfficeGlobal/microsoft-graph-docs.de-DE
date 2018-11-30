---
title: Verwenden der Planner-REST-API
description: Sie können die Planner-API in Microsoft Graph zum Erstellen von Aufgaben, und weisen Sie diese Benutzer in einer Gruppe im Office 365.
ms.openlocfilehash: 1befd7a7e504aa8f568c9b28bc8a08322064bd37
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017955"
---
# <a name="use-the-planner-rest-api"></a>Verwenden der Planner-REST-API

Sie können die Planner-API in Microsoft Graph zum Erstellen von Aufgaben, und weisen Sie diese Benutzer in einer Gruppe im Office 365.

Bevor Sie mit Planner-API beginnen ist es zu verstehen, wie die Hauptobjekte aufeinander sowie über Office 365 Gruppen beziehen.

## <a name="groups"></a>Gruppen

Office 365-Gruppen sind die Besitzer der Pläne in der Planner-API.
Stellen Sie um [den Besitz einer Gruppe Pläne erhalten möchten](../api/plannergroup-list-plans.md)die folgenden HTTP-Anforderung.

``` http
GET /groups/{id}/planner/plans
```

Beim [Erstellen eines neuen Plans](../api/planner-post-plans.md), stellen Sie einer Gruppe Besitzer durch Festlegen der `owner` -Eigenschaft für ein Objekt Plan. Pläne müssen im Besitz von Gruppen.

>**Hinweis:** Der Benutzer, der den Plan erstellen wird, muss ein Mitglied der Gruppe, die Besitzer des Plans. Wenn Sie eine neue Gruppe erstellen, mit der [Gruppe erstellen](../api/group-post-groups.md), werden Sie nicht als Mitglied der Gruppe hinzugefügt. Nach dem Erstellen der Gruppe fügen selbst mithilfe der [Gruppe Mitglieder buchen](../api/group-post-members.md)als Mitglied hinzu.

## <a name="plans"></a>Pläne

[Plant](plannerplan.md) , sind die Container von [Aufgaben](plannertask.md). Legen Sie zum [Erstellen einer Aufgabe in einem Plan](../api/planner-post-tasks.md), der `planId` -Eigenschaft für das Task-Objekt auf die ID des Plans beim Erstellen der Aufgabe.
Aufgaben können derzeit ohne Wählpläne erstellt werden.
Stellen Sie [die Aufgaben in einem Plan abrufen](../api/plannerplan-list-tasks.md)die folgenden HTTP-Anforderung.

``` http
GET /planner/plans/{id}/tasks
```

## <a name="tasks"></a>Aufgaben

Jede Aufgabe kann einem Benutzer zugewiesen werden, indem eine [Zuweisung](plannerassignment.md) in der [assignments](plannerassignments.md)-Eigenschaft des Aufgabenobjekts hinzugefügt wird. Die ID des Benutzers, dem die Aufgabe zugewiesen werden soll, ist der Name der offenen Eigenschaft von `assignments`, und die `orderHint`-Eigenschaft der Zuweisung muss angegeben werden.

## <a name="task-and-plan-details"></a>Aufgaben- und Plandetails 

Planner-Ressourcen sind in einfache Objekte und Detailobjekte unterteilt. Einfache Objekte bieten Zugriff auf allgemeine Eigenschaften der Ressourcen, geeignet für Listenansichten, während die Detailobjekte Zugriff auf umfassende Eigenschaften der Ressourcen bieten, die für Drilldownansichten geeignet sind.

## <a name="visualization"></a>Visualisierung

Neben Aufgaben- und Plandaten stellt die Planner-API auch Ressourcen für die allgemeine Visualisierung von Daten für alle Clients bereit. Für Aufgaben stehen mehrere Arten von Visualisierungsdaten zur Verfügung:

| Aufgaben werden angezeigt als                                                                        | Aufgaben werden sortiert mit Informationen aus                                         |
| :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| Flache Liste (Aufgaben in einem Plan)                                                               | `orderHint`-Eigenschaft für Aufgaben                                                   |
| Flache Liste (einem Benutzer zugewiesene Aufgaben)                                                      | `assigneePriority`-Eigenschaft für Aufgaben                                            |
| Boardansicht mit Spalten für Beauftragte (zugewiesen zum Task Board)                            | [assignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)-Objekt |
| Boardansicht mit Spalten für den Fortschritt der Aufgabe auf dem Weg zur Fertigstellung (Fortschritts-Task Board) | [progressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)-Objekt     |
| Boardansicht mit benutzerdefinierten Spalten von Aufgaben (Bucket-Task Board):                              | [bucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)-Objekt         |

Die benutzerdefinierten Spalten im Bucket-Task Board werden durch [bucket](plannerbucket.md)-Objekte dargestellt und ihre Reihenfolge durch die `orderHint`-Eigenschaft des Objekts.

Die gesamte Sortierung wird durch die unter [Verwenden von ORDER-Hinweisen in Planner ](planner-order-hint-format.md) genannten Grundsätze gesteuert.

## <a name="planner-resource-versioning"></a>Versionsverwaltung für Planner-Ressourcen

Planner verwendet für alle Ressourcen Etags zur Versionsverwaltung. Diese Etags werden mit der `@odata.etag`-Eigenschaft jeder Ressource zurückgegeben; in `PATCH`- und `DELETE`-Anforderungen muss das letzte dem Client bekannte Etag mit dem `If-Match`-Header angegeben werden. Planner erlaubt Änderungen an älteren Versionen von Ressourcen, sofern die beabsichtigte Änderung nicht in Konflikt mit neueren Änderungen steht, die vom Planner-Dienst für dieselbe Ressource akzeptiert wurden. Die Clients können ermitteln, welches Etag für eine bestimmte Ressource neuer ist, indem sie berechnen, welcher Etag-Wert in einem Vergleich von Ordnungszeichenfolgen größer ist. Jede Ressource verfügt über ein eigenes Etag. Etag-Werte für verschiedene Ressourcen, einschließlich solcher mit Einschlussbeziehungen, können nicht verglichen werden. Die Client-Apps müssen zwei Fehlerstatuscodes im Zusammenhang mit der Versionsverwaltung verarbeiten können (409 und 412), indem sie die aktuelle Version des Elements lesen und in Konflikt stehende Änderungen beheben.

## <a name="common-planner-error-conditions"></a>Häufige Planner-Fehlerbedingungen

Neben [allgemeinen Fehlern](/graph/errors), die für Microsoft Graph gelten, sind einige Fehlerbedingungen für die Planner-API spezifisch.

### <a name="400-bad-request"></a>400 Ungültige Anforderung

Es gibt mehrere häufig auftretende Fälle, in denen für die `POST`- und `PATCH`- Anforderungen ein Statuscode 400 zurückgegeben werden kann. Zu den häufigen Problemen gehören:

* Eigenschaften mit offenem Typ weisen nicht den richtigen Typ auf, der Typ ist nicht angegeben oder sie enthalten keine Eigenschaften. Beispielsweise müssen [plannerAssignments](plannerassignments.md)-Eigenschaften mit komplexen Werten die `@odata.type`-Eigenschaft mit dem Wert `microsoft.graph.plannerAssignment` deklarieren.
* Werte von Anordnungshinweisen weisen nicht das [richtige Format](planner-order-hint-format.md) auf. Beispiel: Ein Anordnungshinweiswert ist direkt auf den vom Client zurückgegebenen Wert festgelegt.
* Die Daten sind logisch inkonsistent. Beispiel: Das Startdatum einer Aufgabe liegt nach dem Fälligkeitsdatum der Aufgabe.

### <a name="403-forbidden"></a>403 Verboten

Zusätzlich zu den allgemeinen Fehlern gibt die Planner-API auch diesen Statuscode zurück, wenn ein von einem Dienst definierter Grenzwert überschritten wurde. In diesem Fall gibt die `code`-Eigenschaft des error-Ressourcentyps den Typ des Grenzwerts an, der von der Anforderung überschritten wurde. Die möglichen Werte für die Grenzwerttypen sind u. a.:

| Wert                         | Beschreibung                                                                                                                                                                                              |
| :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| MaximumProjectsOwnedByUser    | Der Grenzwert für die maximale Anzahl von Plänen, die im Besitz eines Gruppe sein können, wurde überschritten. Dieser Grenzwert basiert auf der `owner`-Eigenschaft der [plannerPlan](plannerplan.md)-Ressource.                                         |
| MaximumProjectsSharedWithUser | Der Grenzwert für die maximale Anzahl von Plänen, die für einen Benutzer freigegeben werden können, wurde überschritten.  Dieser Grenzwert basiert auf der `sharedWith`-Eigenschaft der [plannerPlanDetails](plannerplandetails.md)-Ressource.                   |
| MaximumTasksCreatedByUser     | Der Grenzwert für die maximale Anzahl von Aufgaben, die von einem Benutzer erstellt werden können, wurde überschritten. Dieser Grenzwert basiert auf der `createdBy`-Eigenschaft der [plannerTask](plannertask.md)-Ressource.                                    |
| MaximumTasksAssignedToUser    | Der Grenzwert für die maximale Anzahl von Aufgaben, die einem Benutzer zugewiesen werden können, wurde überschritten. Dieser Grenzwert basiert auf der `assignments`-Eigenschaft der [plannerTask](plannertask.md)-Ressource.                                 |
| MaximumTasksInProject         | Der Grenzwert für die maximale Anzahl von Aufgaben in einem Plan wurde überschritten. Dieser Grenzwert basiert auf der `planId`-Eigenschaft der [plannerTask](plannertask.md)-Ressource.                                               |
| MaximumActiveTasksInProject   | Der Grenzwert für die maximale Anzahl von nicht abgeschlossenen Aufgaben in einem Plan wurde überschritten. Dieser Grenzwert basiert auf den Eigenschaften `planId` und `percentComplete` der [plannerTask](plannertask.md)-Ressource. |
| MaximumBucketsInProject       | Der Grenzwert für die maximale Anzahl von Buckets in einem Plan wurde überschritten. Dieser Grenzwert basiert auf der `planId`-Eigenschaft der [plannerBucket](plannerbucket.md)-Ressource.                                         |
| MaximumUsersSharedWithProject | Die `sharedWith`-Eigenschaft der [plannerPlanDetails](plannerplandetails.md)-Ressource enthält zu viele Werte.                                                                                          |
| MaximumReferencesOnTask       | Die `references`-Eigenschaft der [plannerTaskDetails](plannertaskdetails.md)-Ressource enthält zu viele Werte.                                                                                          |
| MaximumChecklistItemsOnTask   | Die `checklist`-Eigenschaft der [plannerTaskDetails](plannertaskdetails.md)-Ressource enthält zu viele Werte.                                                                                           |
| MaximumAssigneesInTasks       | Die `assignments`-Eigenschaft der [plannerTask](plannertask.md)-Ressource enthält zu viele Werte.                                                                                                       |

### <a name="412-precondition-failed"></a>412 Fehler bei Vorbedingung 

Alle `POST`-, `PATCH`- und `DELETE` Anforderungen in der Planner-API erfordern, dass im `If-Match`-Header der letzte Etag-Wert der Ressource angegeben wird, für die die Anforderung gilt. Darüber hinaus kann der Statuscode 412 zurückgegeben werden, wenn der in der Anforderung angegeben Etag-Wert nicht mehr einer Version der Ressource im Dienst entspricht. In diesem Fall sollten die Clients die Ressource erneut lesen und ein neues Etag abrufen.

