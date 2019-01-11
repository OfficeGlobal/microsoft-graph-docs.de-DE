---
title: Verwenden der Planner-REST-API
description: Sie können die Planner-API in Microsoft Graph zum Erstellen von Aufgaben, und weisen Sie diese Benutzer in einer Gruppe im Office 365.
author: TarkanSevilmis
localization_priority: Priority
ms.openlocfilehash: 8a7df9b28efedd128e533eda88d09583ebf12dbc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858023"
---
# <a name="use-the-planner-rest-api"></a>Verwenden der Planner-REST-API

Sie können die Planner-API in Microsoft Graph zum Erstellen von Aufgaben, und weisen Sie diese Benutzer in einer Gruppe im Office 365.

Bevor Sie mit der Planner-API beginnen, sollten Sie verstehen, wie die Hauptobjekte aufeinander sowie über Office 365 Gruppen beziehen.

## <a name="office-365-groups"></a>Office 365-Gruppen

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

Neben dem Aufgaben- und Plan Daten außerdem die Planner-API Ressourcen für eine gemeinsame Visualisierung von Daten über Clients erstellt. Verschiedene Typen von Visualisierungsdaten stehen für Aufgaben vorgestellt, wie in der folgenden Tabelle aufgeführt.

| Aufgaben werden angezeigt als                                                                        | Aufgaben werden sortiert mit Informationen aus                                         |
| :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| Flache Liste (Aufgaben in einem Plan)                                                               | `orderHint`-Eigenschaft für Aufgaben                                                   |
| Flache Liste (einem Benutzer zugewiesene Aufgaben)                                                      | `assigneePriority`-Eigenschaft für Aufgaben                                            |
| Boardansicht mit Spalten für Beauftragte (zugewiesen zum Task Board)                            | [assignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)-Objekt |
| Boardansicht mit Spalten für den Fortschritt der Aufgabe auf dem Weg zur Fertigstellung (Fortschritts-Task Board) | [progressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)-Objekt     |
| Boardansicht mit benutzerdefinierten Spalten von Aufgaben (Bucket-Task Board):                              | [bucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)-Objekt         |

Die benutzerdefinierten Spalten im Bucket-Task Board werden durch [bucket](plannerbucket.md)-Objekte dargestellt und ihre Reihenfolge durch die `orderHint`-Eigenschaft des Objekts.

Gesamten Sortierung wird durch in [Planner Reihenfolge Hinweise](planner-order-hint-format.md)beschriebenen Grundsätze gesteuert.

## <a name="planner-resource-versioning"></a>Versionsverwaltung für Planner-Ressourcen

Planner Versionen alle **Etags**mit Ressourcen. Diese **Etags** mit zurückgegeben werden `@odata.etag` -Eigenschaft in jeder Ressource. `PATCH`und `DELETE` Anfragen erfordern das letzte **Etag** bekanntermaßen vom Client angegeben werden, mit einem `If-Match` Kopfzeile.
Planner ermöglicht Änderungen an ältere Versionen von Ressourcen, wenn die vorgesehene Änderung mit neuere Änderungen, die von den Planner-Dienst auf dieselbe Ressource akzeptiert keine entstehen. Die Clients können identifiziert, welche **Etag** für dieselbe Ressource ist neuer Berechnung, welche **Etag** -Wert in einem Zeichenfolgenvergleich Vergleich größer ist. Jede Ressource verfügt über eine eindeutige **Etag**. ETag-Werte für verschiedene Ressourcen, einschließlich derjenigen Kapselung Beziehungen, können nicht verglichen werden.
Erwartet die Client-apps Versioning behandeln [Fehlercodes](/graph/errors) **409** und **412** durch die neueste Version des Elements zu lesen und Beheben von miteinander in Konflikt stehende Änderungen verknüpft sind.

## <a name="common-planner-error-conditions"></a>Häufige Planner-Fehlerbedingungen

Neben [allgemeinen Fehlern](/graph/errors), die für Microsoft Graph gelten, sind einige Fehlerbedingungen für die Planner-API spezifisch.

### <a name="400-bad-request"></a>400 Ungültige Anforderung

In einigen häufigen Szenarien `POST` und `PATCH` Anfragen 400 Statuscode zurückgeben können. Es folgen einige häufige Ursachen:

* Eigenschaften mit offenem Typ weisen nicht den richtigen Typ auf, der Typ ist nicht angegeben oder sie enthalten keine Eigenschaften. Beispielsweise müssen [plannerAssignments](plannerassignments.md)-Eigenschaften mit komplexen Werten die `@odata.type`-Eigenschaft mit dem Wert `microsoft.graph.plannerAssignment` deklarieren.
* Werte von Anordnungshinweisen weisen nicht das [richtige Format](planner-order-hint-format.md) auf. Beispiel: Ein Anordnungshinweiswert ist direkt auf den vom Client zurückgegebenen Wert festgelegt.
* Die Daten sind logisch inkonsistent. Beispiel: Das Startdatum einer Aufgabe liegt nach dem Fälligkeitsdatum der Aufgabe.

### <a name="403-forbidden"></a>403 Verboten

Zusätzlich zu den allgemeinen Fehlern gibt die Planner-API auch den Statuscode 403 zurück, wenn ein Dienst definiert Grenzwert überschritten wurde. Wenn dies der Fall ist die `code` -Eigenschaft in den Fehlertyp Ressource wird angeben des Typs des der durch die Anforderung wurde überschritten.
Im folgenden werden die möglichen Werte für die Typen der Grenzwert.

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
| MaximumPlannerPlans       | Die Gruppe enthält bereits einen Plan. Gruppen können derzeit nur einen Plan enthalten. **Hinweis:** Einige Microsoft-apps können diesen Grenzwert überschreiten. In der Zukunft werden wir diese Funktion für alle apps erweitern.                                                                                                      |

### <a name="412-precondition-failed"></a>412 Fehler bei Vorbedingung 

Alle Planer API `POST`, `PATCH`, und `DELETE` Anfragen erfordern die `If-Match` Kopfzeile mit dem letzten bekannten Etag-Wert der Ressource angegeben werden, das die Anforderung fällt.
Der 412 Statuscode kann auch zurückgegeben werden, wenn in der Anforderung angegebene Etag-Wert nicht mehr eine Version der Ressource in den Dienst entspricht. In diesem Fall sollte die Clients die Ressource erneut lesen und erhalten eine neue Etag.

