---
title: Verwenden der Planner-REST-API
description: Sie können die Planner-API in Microsoft Graph zum Erstellen von Aufgaben, und weisen Sie diese Benutzer in einer Gruppe im Office 365.
ms.openlocfilehash: 264a196a24dde21b57ff3627c7c39c1951a02ce6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058115"
---
# <a name="use-the-planner-rest-api"></a>Verwenden der Planner-REST-API

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Sie können die Planner-API in Microsoft Graph zum Erstellen von Aufgaben, und weisen Sie diese Benutzer in einer Gruppe im Office 365.

Bevor Sie mit Planner-API beginnen ist es zu verstehen, wie die Hauptobjekte aufeinander sowie über Office 365 Gruppen beziehen.

## <a name="groups"></a>Gruppen

Office 365-Gruppen sind die Besitzer der Pläne in der Planner-API.
Stellen Sie um [den Besitz einer Gruppe Pläne erhalten möchten](../api/plannergroup-list-plans.md)die folgenden HTTP-Anforderung.

``` http
GET /groups/{id}/planner/plans
```

Beim [Erstellen eines neuen Plans](../api/planner-post-plans.md), geben Sie dem Plan einen Gruppenbesitzer durch Festlegen der `owner` -Eigenschaft für ein Objekt Plan. Ein Plan Besitzer muss von einer Gruppe. Eine Gruppe kann mehrere Pläne besitzen.

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

Planner Ressourcen werden in Aufgaben- und Plan Basisobjekte und Detail Aufgaben- und Plan Objekte angeordnet. Basisobjekte bieten Zugriff auf Allgemeine Eigenschaften die Ressourcen, die geeignet für Listenansichten, während die Detailobjekte Zugriff auf große Eigenschaften der Ressourcen für Drilldown Ansichten bereitzustellen.

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

## <a name="delta">Nachverfolgen von Änderungen mithilfe von Delta-Abfrage</a>

Planner Delta Query unterstützt abfragende-Objekten, die der Benutzer abonniert.

Benutzer haben die folgenden Objekte abonniert.

| Ressourcentyp Planner | Abonnierten Instanzen                                                                                                                                                                                    |
| :-------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Aufgaben                 | <ul><li>Vom Benutzer erstellt</li><li>Dem Benutzer zugewiesene</li><li>Gehören Sie zu einem Plan, den der Benutzer besitzt</li><li>In einem Plan gemeinsam mit dem Benutzer über den Plan **SharedWith** -Auflistung enthalten sind</li> |
| Pläne                 | <ul><li>Gemeinsam mit dem Benutzer über den Plan **SharedWith** -Auflistung</li></ul>                                                                                                                     |
| Buckets               | <ul><li>In einem Plan gemeinsam mit dem Benutzer über den Plan **SharedWith** -Auflistung enthalten sind</li></ul>                                                                                                 |  |

### <a name="objectcache">Füllen Sie den Objektcache für Delta-Abfragen</a>

Wenn Sie die Planner Delta-Abfrage-API verwenden möchten, müssen verwalten Sie einen lokalen Cache der Objekte, die der Benutzer verwendet, um die Änderungen aus dem Delta-Antwort-Feed zu übernehmen und möchte.

Die Delta-Nutzlast-Objekte, die die Planner Delta-Abfrage, die derzeit werden kann, die folgenden Typen werden:

* [plannerTask](plannertask.md)
* [plannerTaskDetails](plannertaskdetails.md)
* [plannerPlan](plannerplan.md)
* [plannerPlanDetails](plannerplandetails.md)
* [plannerBucket](plannerbucket.md)
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)
* [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)

Verwenden Sie die entsprechende `GET` Methoden für die Ressource den Anfangszustand der Objekte in den lokalen Cache aufgefüllt werden abgerufen.

### <a name="differentiating-between-object-creation-and-object-modification"></a>Unterscheidung zwischen Erstellung und Änderung Objekt

In bestimmten Szenarien sollten der Aufrufer zur Unterscheidung zwischen Erstellung und Änderung in Planner Delta Abfrage feed Objekt.

Diese Richtlinien können zum Erstellen eines Objekts ableiten verwendet werden:

* Die `createdBy` Eigenschaft wird nur für neu erstellte Objekte angezeigt.
* Ein neu erstelltes `plannerTask` Objekt gefolgt von dem zugehörigen `plannerTaskDetails` Objekt.
* Ein neu erstelltes `plannerPlan` Objekt gefolgt von dem zugehörigen `plannerPlanDetails` Objekt.

### <a name="usage"></a>Verwendung

Der Anrufer wird erwartet, dass einen Cache mit abonnierten Objekten haben. Ausführliche Informationen zum Auffüllen des lokalen Caches der abonnierten Objekte finden Sie unter [Auffüllen des Objektcaches für Delta-Abfragen](#populate-the-object-cache-for-delta-queries).

Planner Delta Abfrage Anruffluss lautet wie folgt:

1. Der Aufrufer initiiert eine Delta Sync-Abfrage, Abrufen von einem `nextLink` und eine leere Auflistung von Änderungen.
2. Der Aufrufer muss [den Objektcache für Delta Abfragen Auffüllen](#populate-the-object-cache-for-delta-queries) mit Objekten, die der Benutzer, abonniert ist Aktualisieren des Caches.
3. Der Aufrufer folgt die `nextLink` bereitgestellt, in der anfänglichen Delta Sync-Abfrage zum Abrufen einer neuen `deltaLink` um Änderungen seit dem vorherigen Schritt.
4. Der Anrufer die Änderungen in der zurückgegebenen Delta-Antwort auf die Objekte im Cache angewendet.
5. Der Aufrufer die neue DeltaLink zum Abrufen der nächsten DeltaLink folgt und geändert, seit die aktuelle `deltaLink` generiert wurde.
6. Der Aufrufer die Änderungen (falls vorhanden) angewendet und wartet, bis ein kurzes Zeitformat an erneutes Ausführen der vorherigen Schritt und diesen Schritt.

## <a name="planner-resource-versioning"></a>Versionsverwaltung für Planner-Ressourcen

Planner Versionen alle **Etags**mit Ressourcen. Diese **Etags** mit zurückgegeben werden `@odata.etag` -Eigenschaft in jeder Ressource. `PATCH`und `DELETE` Anfragen erfordern das letzte **Etag** bekanntermaßen vom Client angegeben werden, mit einem `If-Match` Kopfzeile.
Planner zugelassen, dass Änderungen an ältere Versionen von Ressourcen, sofern die vorgesehene Änderung mit neuere Änderungen, die von den Planner-Dienst auf dieselbe Ressource akzeptiert keine entstehen. Die Clients können identifiziert, welche **Etag** für dieselbe Ressource ist neuer Berechnung, welche **Etag** -Wert in einem Zeichenfolgenvergleich Vergleich größer ist. Jede Ressource verfügt über eine eindeutige **Etag**. ETag-Werte für verschiedene Ressourcen, einschließlich derjenigen Kapselung Beziehungen, können nicht verglichen werden.
Erwartet die Client-apps Versioning behandeln [Fehlercodes](/graph/errors) **409** und **412** durch die neueste Version des Elements zu lesen und Beheben von miteinander in Konflikt stehende Änderungen verknüpft sind.

## <a name="common-planner-error-conditions"></a>Häufige Planner-Fehlerbedingungen

Neben [allgemeinen Fehlern](/graph/errors), die für Microsoft Graph gelten, sind einige Fehlerbedingungen für die Planner-API spezifisch.

### <a name="400-bad-request"></a>400 Ungültige Anforderung

Es gibt mehrere häufig auftretende Fälle, in denen für die `POST`- und `PATCH`- Anforderungen ein Statuscode 400 zurückgegeben werden kann. Zu den häufigen Problemen gehören:

* Open Typeigenschaften sind nicht der richtigen Typen.
* Der Typ ist nicht angegeben.
* Die Anforderung enthält keine Eigenschaften.

#### <a name="example"></a>Beispiel

Eigenschaften mit komplexen Werten [PlannerAssignments](plannerassignments.md) deklarieren müssen `@odata.type` -Eigenschaft mit dem Wert `microsoft.graph.plannerAssignment`.

* Reihenfolge Hint Werte müssen nicht das [richtige Format](planner-order-hint-format.md).

   Beispielsweise wird direkt auf den Wert an den Client zurückgegeben ein Order Hint-Wert festgelegt.

* Die Daten sind logisch inkonsistent.

   Beispielsweise liegt Anfangstermin des Vorgangs fällig nach Datum des Vorgangs.

### <a name="planner-error-status-codes"></a>Planner Status Fehlercodes

Zusätzlich zu den allgemeinen Status Fehlercodes gibt Planner spezielle fehlerbedingungen durch die folgenden Codes zurückgeben.

#### <a name="403-forbidden"></a>403 Verboten

Die Planner-API gibt den Statuscode **403** zurück, wenn ein Dienst definiert Grenzwert überschritten wurde. In diesem Fall die `code` -Eigenschaft in den Fehlertyp Ressource gibt den Typ des der durch die Anforderung wurde überschritten.
Die möglichen Werte für die Arten von Grenzwerten umfassen:

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
| MaximumFavoritePlansForUser   | Die `favoritePlanReferences` -Eigenschaft für die Ressource [PlannerUser](planneruser.md) enthält zu viele Werte.                                                                                            |
| MaximumRecentPlansForUser     | Die `recentPlanReferences` -Eigenschaft für die Ressource [PlannerUser](planneruser.md) enthält zu viele Werte.                                                                                              |
| MaximumContextsOnPlan         | Die `contexts` -Eigenschaft für die Ressource [PlannerPlan](plannerplan.md) enthält zu viele Werte.                                                                                                          |

#### <a name="412-precondition-failed"></a>412 Fehler bei Vorbedingung

Alle `POST`-, `PATCH`- und `DELETE` Anforderungen in der Planner-API erfordern, dass im `If-Match`-Header der letzte Etag-Wert der Ressource angegeben wird, für die die Anforderung gilt. Darüber hinaus kann der Statuscode 412 zurückgegeben werden, wenn der in der Anforderung angegeben Etag-Wert nicht mehr einer Version der Ressource im Dienst entspricht. In diesem Fall sollten die Clients die Ressource erneut lesen und ein neues Etag abrufen.

