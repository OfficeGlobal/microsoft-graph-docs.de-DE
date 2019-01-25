---
title: Ressourcentyp synchronizationStatus
description: Stellt den aktuellen Status der SynchronizationJob.
localization_priority: Normal
ms.openlocfilehash: 404fe4f7f58b8189b3059c212aa1ce858350bb01
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523764"
---
# <a name="synchronizationstatus-resource-type"></a><span data-ttu-id="95341-103">Ressourcentyp synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="95341-103">synchronizationStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95341-104">Stellt den aktuellen Status der [SynchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="95341-104">Represents the current status of the [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="95341-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="95341-105">Properties</span></span>

| <span data-ttu-id="95341-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="95341-106">Property</span></span>                              | <span data-ttu-id="95341-107">Typ</span><span class="sxs-lookup"><span data-stu-id="95341-107">Type</span></span>      | <span data-ttu-id="95341-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="95341-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="95341-109">code</span><span class="sxs-lookup"><span data-stu-id="95341-109">code</span></span>|<span data-ttu-id="95341-110">String</span><span class="sxs-lookup"><span data-stu-id="95341-110">String</span></span>|<span data-ttu-id="95341-111">Allgemeine Statuscode des Synchronisierungsauftrags.</span><span class="sxs-lookup"><span data-stu-id="95341-111">High-level status code of the synchronization job.</span></span> <span data-ttu-id="95341-112">Mögliche Werte sind: `NotConfigured`, `NotRun`, `Active`, `Paused` und `Quarantine`.</span><span class="sxs-lookup"><span data-stu-id="95341-112">Possible values are: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.</span></span>|
|<span data-ttu-id="95341-113">countSuccessiveCompleteFailures</span><span class="sxs-lookup"><span data-stu-id="95341-113">countSuccessiveCompleteFailures</span></span>|<span data-ttu-id="95341-114">Int64</span><span class="sxs-lookup"><span data-stu-id="95341-114">Int64</span></span>|<span data-ttu-id="95341-115">Häufigkeit der aufeinander folgenden diesen Auftrag ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="95341-115">Number of consecutive times this job failed.</span></span>|
|<span data-ttu-id="95341-116">escrowsPruned</span><span class="sxs-lookup"><span data-stu-id="95341-116">escrowsPruned</span></span>|<span data-ttu-id="95341-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="95341-117">Boolean</span></span>|<span data-ttu-id="95341-118">`true`Wenn der Auftrag Artikel mit Treuhandservice (Fehler auf Objektebene) während der ersten Synchronisierung gelöscht wurden.</span><span class="sxs-lookup"><span data-stu-id="95341-118">`true` if the job's escrows (object-level errors) were pruned during initial synchronization.</span></span> <span data-ttu-id="95341-119">Artikel mit Treuhandservice können gelöscht werden, wenn während der ersten Synchronisierung des Schwellenwerts für Fehler erreichen, die normalerweise den Auftrag in Quarantäne eingetragen wird.</span><span class="sxs-lookup"><span data-stu-id="95341-119">Escrows can be pruned if during the initial synchronization, you reach the threshold of errors that would normally put the job in quarantine.</span></span> <span data-ttu-id="95341-120">Statt in Quarantäne Synchronisierungsvorgangs löscht den Auftrag Fehler und wird fortgesetzt, bis die anfängliche Synchronisierung abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="95341-120">Instead of going into quarantine, the synchronization process clears the job's errors and continues until the initial synchronization is completed.</span></span> <span data-ttu-id="95341-121">Wenn die anfängliche Synchronisierung abgeschlossen ist, wird der Auftrag anhalten und warten, bis der Kunde, um den Fehler zu bereinigen.</span><span class="sxs-lookup"><span data-stu-id="95341-121">When the initial synchronization is completed, the job will pause and wait for the customer to clean up the errors.</span></span>|
|<span data-ttu-id="95341-122">lastExecution</span><span class="sxs-lookup"><span data-stu-id="95341-122">lastExecution</span></span>|[<span data-ttu-id="95341-123">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="95341-123">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="95341-124">Details der letzten Ausführung des Auftrags.</span><span class="sxs-lookup"><span data-stu-id="95341-124">Details of the last execution of the job.</span></span>|
|<span data-ttu-id="95341-125">lastSuccessfulExecution</span><span class="sxs-lookup"><span data-stu-id="95341-125">lastSuccessfulExecution</span></span>|[<span data-ttu-id="95341-126">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="95341-126">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="95341-127">Details der letzten Ausführung dieser Auftrag, die Fehler aufweisen, nicht.</span><span class="sxs-lookup"><span data-stu-id="95341-127">Details of the last execution of this job, which didn't have any errors.</span></span>|
|<span data-ttu-id="95341-128">lastSuccessfulExecutionWithExports</span><span class="sxs-lookup"><span data-stu-id="95341-128">lastSuccessfulExecutionWithExports</span></span>|[<span data-ttu-id="95341-129">synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="95341-129">synchronizationTaskExecution</span></span>](synchronization-synchronizationtaskexecution.md)|<span data-ttu-id="95341-130">Details der letzten Ausführung des Auftrags, der exportierte Objekte in das Zielverzeichnis.</span><span class="sxs-lookup"><span data-stu-id="95341-130">Details of the last execution of the job, which exported objects into the target directory.</span></span>|
|<span data-ttu-id="95341-131">progress</span><span class="sxs-lookup"><span data-stu-id="95341-131">progress</span></span>|<span data-ttu-id="95341-132">[SynchronizationProgress](synchronization-synchronizationprogress.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="95341-132">[synchronizationProgress](synchronization-synchronizationprogress.md) collection</span></span>|<span data-ttu-id="95341-133">Details zu den Fortschritt eines Auftrags an.</span><span class="sxs-lookup"><span data-stu-id="95341-133">Details of the progress of a job toward completion.</span></span>|
|<span data-ttu-id="95341-134">Quarantäne</span><span class="sxs-lookup"><span data-stu-id="95341-134">quarantine</span></span>|[<span data-ttu-id="95341-135">synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="95341-135">synchronizationQuarantine</span></span>](synchronization-quarantine.md)|<span data-ttu-id="95341-136">Wenn der Auftrag in Quarantäne ist, Quarantänedetails.</span><span class="sxs-lookup"><span data-stu-id="95341-136">If job is in quarantine, quarantine details.</span></span>|
|<span data-ttu-id="95341-137">steadyStateFirstAchievedTime</span><span class="sxs-lookup"><span data-stu-id="95341-137">steadyStateFirstAchievedTime</span></span>|<span data-ttu-id="95341-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95341-138">DateTimeOffset</span></span>|<span data-ttu-id="95341-139">Der Zeitpunkt, wann stabilen Zustand (keine weitere Änderungen an den Prozess) zuerst erreicht wurde.</span><span class="sxs-lookup"><span data-stu-id="95341-139">The time when steady state (no more changes to the process) was first achieved.</span></span> <span data-ttu-id="95341-140">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="95341-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="95341-141">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="95341-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="95341-142">steadyStateLastAchievedTime</span><span class="sxs-lookup"><span data-stu-id="95341-142">steadyStateLastAchievedTime</span></span>|<span data-ttu-id="95341-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95341-143">DateTimeOffset</span></span>|<span data-ttu-id="95341-144">Die Uhrzeit, wann zuletzt stabilen Zustand (keine weitere Änderungen an den Prozess) erreicht wurde.</span><span class="sxs-lookup"><span data-stu-id="95341-144">The time when steady state (no more changes to the process) was last achieved.</span></span> <span data-ttu-id="95341-145">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="95341-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="95341-146">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="95341-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="95341-147">synchronizedEntryCountByType</span><span class="sxs-lookup"><span data-stu-id="95341-147">synchronizedEntryCountByType</span></span>|<span data-ttu-id="95341-148">[StringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="95341-148">[stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md) collection</span></span>|<span data-ttu-id="95341-149">Anzahl der synchronisierten Objekte nach Objekttyp aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="95341-149">Count of synchronized objects, listed by object type.</span></span>|
|<span data-ttu-id="95341-150">troubleshootingUrl</span><span class="sxs-lookup"><span data-stu-id="95341-150">troubleshootingUrl</span></span>|<span data-ttu-id="95341-151">String</span><span class="sxs-lookup"><span data-stu-id="95341-151">String</span></span>|<span data-ttu-id="95341-152">Im Fall eines Fehlers, die URL durch die Schritte zur Problembehandlung für das Problem.</span><span class="sxs-lookup"><span data-stu-id="95341-152">In the event of an error, the URL with the troubleshooting steps for the issue.</span></span>|

### <a name="synchronization-status-code-details"></a><span data-ttu-id="95341-153">Synchronisierung Status Code details</span><span class="sxs-lookup"><span data-stu-id="95341-153">Synchronization status code details</span></span>

| <span data-ttu-id="95341-154">Wert</span><span class="sxs-lookup"><span data-stu-id="95341-154">Value</span></span>                              | <span data-ttu-id="95341-155">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="95341-155">Description</span></span>    |
|:-----------------------------------|:---------------|
|<span data-ttu-id="95341-156">Nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="95341-156">NotConfigured</span></span>                       |<span data-ttu-id="95341-157">Auftrag wurde nicht konfiguriert und nie ausführen.</span><span class="sxs-lookup"><span data-stu-id="95341-157">Job was not configured and never run.</span></span> <span data-ttu-id="95341-158">Es wurde keine Autorisierung bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="95341-158">No authorization was provided.</span></span> |
|<span data-ttu-id="95341-159">NotRun</span><span class="sxs-lookup"><span data-stu-id="95341-159">NotRun</span></span>                              |<span data-ttu-id="95341-160">Auftrag konfiguriert wurde, und möglicherweise gestartet, aber der ersten Ausführung noch nicht abgeschlossen wurde.</span><span class="sxs-lookup"><span data-stu-id="95341-160">Job was configured, and possibly started, but hasn't completed its first run.</span></span>|
|<span data-ttu-id="95341-161">Aktiv</span><span class="sxs-lookup"><span data-stu-id="95341-161">Active</span></span>                              |<span data-ttu-id="95341-162">Auftrag wird in regelmäßigen Abständen ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="95341-162">Job is running periodically.</span></span>|
|<span data-ttu-id="95341-163">Angehalten</span><span class="sxs-lookup"><span data-stu-id="95341-163">Paused</span></span>                              |<span data-ttu-id="95341-164">Auftrag (normalerweise von einem Administrator) angehalten wurde und wird derzeit nicht ausgeführt, aber der Status des Auftrags wird beibehalten.</span><span class="sxs-lookup"><span data-stu-id="95341-164">Job was paused (usually by an administrator) and currently is not running, but the state of the job is preserved.</span></span>|
|<span data-ttu-id="95341-165">Quarantäne</span><span class="sxs-lookup"><span data-stu-id="95341-165">Quarantine</span></span>                          |<span data-ttu-id="95341-166">Auftrag ist in Quarantäne.</span><span class="sxs-lookup"><span data-stu-id="95341-166">Job is in quarantine.</span></span> <span data-ttu-id="95341-167">Dies kann vorkommen, wenn eine große Menge von Fehlern oder kritische Fehler wie widerrufen/Abgelaufene Anmeldeinformationen vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="95341-167">This might happen when there is a high volume of errors, or critical errors such as revoked/expired credentials.</span></span> <span data-ttu-id="95341-168">In Quarantäne, versucht Synchronisierungsvorgangs mit Geringere Häufigkeit den Auftrag ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="95341-168">While in quarantine, the synchronization process will attempt to run the job with reduced frequency.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95341-169">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="95341-169">JSON representation</span></span>

<span data-ttu-id="95341-170">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="95341-170">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
}-->

```json
{
  "code": "String",
  "countSuccessiveCompleteFailures": 1024,
  "escrowsPruned": true,
  "lastExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecutionWithExports": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "progress": [{"@odata.type": "microsoft.graph.synchronizationProgress"}],
  "quarantine": {"@odata.type": "microsoft.graph.synchronizationQuarantine"},
  "steadyStateFirstAchievedTime": "String (timestamp)",
  "steadyStateLastAchievedTime": "String (timestamp)",
  "synchronizedEntryCountByType": [{"@odata.type": "microsoft.graph.stringKeyLongValuePair"}],
  "troubleshootingUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
