---
title: Verwenden der Planner-REST-API
description: Mit der Planner-API in Microsoft Graph können Sie Aufgaben erstellen und diese Benutzern in einer Office 365-Gruppe zuweisen.
author: TarkanSevilmis
localization_priority: Priority
ms.prod: planner
ms.openlocfilehash: 327701fde2679ab4c90061cf2ed98c4967a5cf58
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509868"
---
# <a name="use-the-planner-rest-api"></a>Verwenden der Planner-REST-API

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Mit der Planner-API in Microsoft Graph können Sie Aufgaben erstellen und diese Benutzern in einer Office 365-Gruppe zuweisen.

Bevor Sie mit der Arbeit in der Planner-API beginnen, sollten Sie wissen, wie die wichtigsten Objekte in der Planner-API zueinander und zu Office 365-Gruppen in Beziehung stehen.

## <a name="office-365-groups"></a>Office 365-Gruppen

Office 365-Gruppen sind die Besitzer der Pläne in der Planner-API.
Um [die im Besitz einer Gruppe befindlichen Pläne abzurufen](../api/plannergroup-list-plans.md), stellen Sie die folgende HTTP-Anforderung.

``` http
GET /groups/{id}/planner/plans
```

Wenn Sie [einen neuen Plan erstellen](../api/planner-post-plans.md), definieren Sie eine Gruppe als dessen Besitzer, indem Sie einfach die `owner`-Eigenschaft für ein Planobjekt festlegen. Pläne müssen im Besitz von Gruppen sein.

>**Hinweis:** Der Benutzer, der den Plan erstellt, muss ein Mitglied der Gruppe sein, die den Plan besitzt. Wenn Sie eine neue Gruppe über [Gruppe erstellen](../api/group-post-groups.md) erstellen, werden Sie nicht automatisch als Mitglied zur Gruppe hinzugefügt. Nachdem die Gruppe erstellt wurde, fügen Sie sich selbst mithilfe der Option zum [Veröffentlichen der Gruppenmitglieder](../api/group-post-members.md) als Mitglied hinzu.

## <a name="plans"></a>Pläne

[Pläne](plannerplan.md) sind die Container von [Aufgaben](plannertask.md). Um [eine Aufgabe in einem Plan zu erstellen](../api/planner-post-tasks.md), legen Sie die `planId`-Eigenschaft des Aufgabenobjekts beim Erstellen der Aufgabe auf die ID des Plans fest.
Aufgaben können derzeit nicht ohne Pläne erstellt werden.
Um [die Aufgaben in einem Plan abzurufen](../api/plannerplan-list-tasks.md), stellen Sie die folgende HTTP-Anforderung.

``` http
GET /planner/plans/{id}/tasks
```

## <a name="tasks"></a>Aufgaben

Jede Aufgabe kann einem Benutzer zugewiesen werden, indem eine [Zuweisung](plannerassignment.md) in der [assignments](plannerassignments.md)-Eigenschaft des Aufgabenobjekts hinzugefügt wird. Die ID des Benutzers, dem die Aufgabe zugewiesen werden soll, ist der Name der offenen Eigenschaft von `assignments`, und die `orderHint`-Eigenschaft der Zuweisung muss angegeben werden.

## <a name="task-and-plan-details"></a>Aufgaben- und Plandetails 

Planner-Ressourcen sind in einfache Objekte und Detailobjekte unterteilt. Einfache Objekte bieten Zugriff auf allgemeine Eigenschaften der Ressourcen, geeignet für Listenansichten, während die Detailobjekte Zugriff auf umfassende Eigenschaften der Ressourcen bieten, die für Drilldownansichten geeignet sind.

## <a name="visualization"></a>Visualisierung

Neben Aufgaben- und Plandaten stellt die Planner-API auch Ressourcen zum Erstellen einer allgemeinen Visualisierung von Daten für alle Clients bereit. Für Aufgaben stehen mehrere Arten von Visualisierungsdaten zur Verfügung, wie in der folgenden Tabelle aufgeführt.

| Aufgaben werden angezeigt als                                                                        | Aufgaben werden sortiert mit Informationen aus                                         |
| :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| Flache Liste (Aufgaben in einem Plan)                                                               | `orderHint`-Eigenschaft für Aufgaben                                                   |
| Flache Liste (einem Benutzer zugewiesene Aufgaben)                                                      | `assigneePriority`-Eigenschaft für Aufgaben                                            |
| Boardansicht mit Spalten für Beauftragte (zugewiesen zum Task Board)                            | [assignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)-Objekt |
| Boardansicht mit Spalten für den Fortschritt der Aufgabe auf dem Weg zur Fertigstellung (Fortschritts-Task Board) | [progressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)-Objekt     |
| Boardansicht mit benutzerdefinierten Spalten von Aufgaben (Bucket-Task Board):                              | [bucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)-Objekt         |

Die benutzerdefinierten Spalten im Bucket-Task Board werden durch [bucket](plannerbucket.md)-Objekte dargestellt und ihre Reihenfolge durch die `orderHint`-Eigenschaft des Objekts.

Die gesamte Sortierung wird durch die unter [ORDER-Hinweise in Planner ](planner-order-hint-format.md) genannten Grundsätze gesteuert.

## <a name="delta">Nachverfolgen von Änderungen mithilfe einer Delta-Abfrage</a>

Die Delta-Abfrage von Planner unterstützt das Abfragen von Objekten, die der Benutzer abonniert hat.

Benutzer haben die folgenden Objekte abonniert.

| Planner-Ressourcentyp | Abonnierte Instanzen                                                                                                                                                                                    |
| :-------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Aufgaben                 | <ul><li>Vom Benutzer erstellt</li><li>Dem Benutzer zugewiesen</li><li>Gehören zu einem Plan, den der Benutzer besitzt</li><li>In einem Plan enthalten, der für den Benutzer über die **SharedWith**-Sammlung des Plans freigegeben wird.</li> |
| Pläne                 | <ul><li>Für den Benutzer über die **SharedWith**-Sammlung des Plans freigegeben.</li></ul>                                                                                                                     |
| Buckets               | <ul><li>In einem Plan enthalten, der für den Benutzer über die **SharedWith**-Sammlung des Plans freigegeben wird.</li></ul>                                                                                                 |  |

### <a name="objectcache">Auffüllen des Objektcaches für Delta-Abfragen</a>

Wenn Sie die Delta-Abfrage-API von Planner verwenden möchten, verwalten Sie einen lokalen Cache von Objekten, die der Benutzer beobachten möchte, um die Änderungen aus dem Delta-Antwortfeed anzuwenden.

Die Delta-Nutzlastobjekte, die die Planner-Delta-Abfrage derzeit zurückgeben kann, weisen einen der folgenden Typen auf:

* [plannerTask](plannertask.md)
* [plannerTaskDetails](plannertaskdetails.md)
* [plannerPlan](plannerplan.md)
* [plannerPlanDetails](plannerplandetails.md)
* [plannerBucket](plannerbucket.md)
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)
* [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)

Verwenden Sie die entsprechenden `GET`-Methoden in der Ressource, um den ursprünglichen Status von Objekten abzurufen, die im lokalen Cache aufgefüllt werden sollen.

### <a name="differentiating-between-object-creation-and-object-modification"></a>Unterscheidung zwischen Objekterstellung und Objektänderung

In bestimmten Szenarien möchte der Aufrufer innerhalb des Delta-Abfragefeeds von Planner vielleicht zwischen Objekterstellung und Objektänderung unterscheiden.

Die folgenden Richtlinien können für das Ableiten der Objekterstellung verwendet werden:

* Die `createdBy`-Eigenschaft wird nur für neu erstellte Objekte angezeigt.
* Auf ein neu erstelltes `plannerTask`-Objekt folgen entsprechende `plannerTaskDetails`-Objekte.
* Auf ein neu erstelltes `plannerPlan`-Objekt folgen entsprechende `plannerPlanDetails`-Objekte.

### <a name="usage"></a>Verwendung

Vom Aufrufer wird erwartet, dass er einen Cache aufweist, der abonnierte Objekte enthält. Weitere Informationen zum Füllen des lokalen Caches abonnierter Objekte finden Sie unter [Auffüllen des Objektcaches für Delta-Abfragen](#populate-the-object-cache-for-delta-queries).

Der Aufruffluss von Delta-Abfragen in Planner ist wie folgt:

1. Der Aufrufer initiiert eine Delta-Synchronisierungsabfrage, wodurch ein `nextLink`-Element und eine leere Auflistung von Änderungen abgerufen wird.
2. Der Aufrufer muss [den Objektcache für Delta-Abfragen](#populate-the-object-cache-for-delta-queries) mit Objekten auffüllen, die der Benutzer abonniert hat, wodurch der Cache aktualisiert wird.
3. Der Aufrufer folgt dem in der ursprünglichen Delta-Synchronisierungsabfrage bereitgestellten `nextLink`, um einen neuen `deltaLink` für alle Änderungen seit dem vorherigen Schritt abzurufen.
4. Der Aufrufer wendet die Änderungen in der zurückgegebenen Delta-Antwort auf die Objekte im Cache an.
5. Der Aufrufer folgt dem neuen deltaLink, um den nächsten deltaLink und Änderungen abzurufen, seit das aktuelle `deltaLink`-Element generiert wurde.
6. Der Aufrufer wendet die Änderungen (sofern vorhanden) an und wartet einen Moment, bevor der vorherige Schritt und dieser Schritt erneut ausgeführt werden.

## <a name="planner-resource-versioning"></a>Versionsverwaltung für Planner-Ressourcen

Planner verwendet für alle Ressourcen **ETags** zur Versionsverwaltung. Diese **ETags** werden mit der `@odata.etag`-Eigenschaft in jeder Ressource zurückgegeben. `PATCH`- und `DELETE`-Anfragen erfordern, dass das letzte **ETag**, das dem Client bekannt ist, mit einer `If-Match`-Kopfzeile angegeben wird.
Planner erlaubt Änderungen an älteren Versionen von Ressourcen, sofern die beabsichtigte Änderung nicht in Konflikt mit neueren Änderungen steht, die vom Planner-Dienst für dieselbe Ressource akzeptiert wurden. Die Clients können ermitteln, welches **ETag** für eine bestimmte Ressource neuer ist, indem sie berechnen, welcher **Etag**-Wert in einem Vergleich von Ordnungszeichenfolgen größer ist. Jede Ressource verfügt über ein eigenes **ETag**. ETag-Werte für verschiedene Ressourcen, einschließlich solcher mit Einschlussbeziehungen, können nicht verglichen werden.
Die Client-Apps müssen die [Fehlercodes](/graph/errors) **409** und **412** im Zusammenhang mit der Versionsverwaltung verarbeiten können, indem sie die aktuelle Version des Elements lesen und in Konflikt stehende Änderungen beheben.

## <a name="common-planner-error-conditions"></a>Häufige Planner-Fehlerbedingungen

Neben [allgemeinen Fehlern](/graph/errors), die für Microsoft Graph gelten, sind einige Fehlerbedingungen für die Planner-API spezifisch.

### <a name="400-bad-request"></a>400 Ungültige Anforderung

In einigen häufigen Szenarios können `POST`- und `PATCH`-Anforderungen auch den Fehlerstatuscode 400 zurückgeben. Nachfolgend sehen Sie die häufigsten Ursachen:

* Eigenschaften mit offenem Typ weisen nicht den richtigen Typ auf, der Typ ist nicht angegeben oder sie enthalten keine Eigenschaften. Beispielsweise müssen plannerAssignments-Eigenschaften mit komplexen Werten die -Eigenschaft mit dem Wert  deklarieren.
* Werte von Anordnungshinweisen weisen nicht das richtige Format auf. Beispiel: Ein Anordnungshinweiswert ist direkt auf den vom Client zurückgegebenen Wert festgelegt.
* Die Daten sind logisch inkonsistent. Das Startdatum einer Aufgabe liegt z. B. nach dem Fälligkeitsdatum der Aufgabe.

### <a name="403-forbidden"></a>403 Verboten

Zusätzlich zu den allgemeinen Fehlern gibt die Planner-API auch den Statuscode 403 zurück, wenn ein von einem Dienst definierter Grenzwert überschritten wurde. In diesem Fall gibt die `code`-Eigenschaft des error-Ressourcentyps den Typ des Grenzwerts an, der von der Anforderung überschritten wurde.
Nachfolgend finden Sie die möglichen Werte für die Grenzwerttypen.

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
| MaximumFavoritePlansForUser   | Die `favoritePlanReferences`-Eigenschaft der [plannerUser](planneruser.md)-Ressource enthält zu viele Werte.                                                                                            |
| MaximumRecentPlansForUser     | Die `recentPlanReferences`-Eigenschaft der [plannerUser](planneruser.md)-Ressource enthält zu viele Werte.                                                                                              |
| MaximumContextsOnPlan         | Die `contexts`-Eigenschaft der [plannerPlan](plannerplan.md)-Ressource enthält zu viele Werte.                                                                                                          |
| MaximumPlannerPlans       | Die Gruppe enthält bereits einen Plan. Gruppen können derzeit nur einen Plan enthalten. **Hinweis:** Einige Microsoft-Apps können diesen Grenzwert überschreiten. Diese Funktion wird in Zukunft auf alle Apps erweitert.                                                                                                      |

### <a name="412-precondition-failed"></a>412 Fehler bei Vorbedingung 

Alle `POST`-, `PATCH`- und `DELETE` Anforderungen in der Planner-API erfordern, dass im `If-Match`-Header der letzte bekannte Etag-Wert der Ressource angegeben wird, für die die Anforderung gilt.
Der Statuscode 412 kann auch zurückgegeben werden, wenn der in der Anforderung angegeben Etag-Wert nicht mehr einer Version der Ressource im Dienst entspricht. In diesem Fall sollten die Clients die Ressource erneut lesen und ein neues Etag abrufen.

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/planner-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
