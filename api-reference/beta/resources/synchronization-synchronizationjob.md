---
title: Ressourcentyp synchronizationJob
description: Führt eine Synchronisierung von in regelmäßigen Abständen im Hintergrund ausgeführt, abrufen, damit die Änderungen in ein Verzeichnis und pushen von in ein anderes Verzeichnis. Der Synchronisierungsauftrag ist immer spezifisch für eine bestimmte Instanz einer Anwendung in Ihrem Mandanten. Im Rahmen der Synchronisierung Einrichtung müssen Sie die Autorisierung zum Lesen und Schreiben von Objekten in Ihrem Zielverzeichnis übergeben, und passen den Auftrag Synchronisierungsschema.
localization_priority: Normal
ms.openlocfilehash: 57515857ac6561e73ef0f67f91bdead98abfb937
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510568"
---
# <a name="synchronizationjob-resource-type"></a><span data-ttu-id="11e56-105">Ressourcentyp synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="11e56-105">synchronizationJob resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11e56-106">Führt eine Synchronisierung von in regelmäßigen Abständen im Hintergrund ausgeführt, abrufen, damit die Änderungen in ein Verzeichnis und pushen von in ein anderes Verzeichnis.</span><span class="sxs-lookup"><span data-stu-id="11e56-106">Performs synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="11e56-107">Der Synchronisierungsauftrag ist immer spezifisch für eine bestimmte Instanz einer Anwendung in Ihrem Mandanten.</span><span class="sxs-lookup"><span data-stu-id="11e56-107">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="11e56-108">Im Rahmen der Synchronisierung Einrichtung müssen Sie die Autorisierung zum Lesen und Schreiben von Objekten in Ihrem Zielverzeichnis übergeben, und passen den Auftrag Synchronisierungsschema.</span><span class="sxs-lookup"><span data-stu-id="11e56-108">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

## <a name="methods"></a><span data-ttu-id="11e56-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="11e56-109">Methods</span></span>

| <span data-ttu-id="11e56-110">Methode</span><span class="sxs-lookup"><span data-stu-id="11e56-110">Method</span></span>        | <span data-ttu-id="11e56-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="11e56-111">Return Type</span></span>               | <span data-ttu-id="11e56-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11e56-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="11e56-113">List</span><span class="sxs-lookup"><span data-stu-id="11e56-113">List</span></span>](../api/synchronization-synchronizationjob-list.md)             |<span data-ttu-id="11e56-114">[SynchronizationJob](synchronization-synchronizationjob.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="11e56-114">[synchronizationJob](synchronization-synchronizationjob.md) collection</span></span>  |<span data-ttu-id="11e56-115">Vorhandene Aufträge für eine Instanz einer Anwendung (Service Principal) auflisten.</span><span class="sxs-lookup"><span data-stu-id="11e56-115">List existing jobs for a given application instance (service principal).</span></span>|
|[<span data-ttu-id="11e56-116">Abrufen von synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="11e56-116">Get synchronizationJob</span></span>](../api/synchronization-synchronizationjob-get.md) | [<span data-ttu-id="11e56-117">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="11e56-117">synchronizationJob</span></span>](synchronization-synchronizationjob.md) |<span data-ttu-id="11e56-118">Lesen Sie Eigenschaften und die Beziehungen eines SynchronizationJob-Objekts.</span><span class="sxs-lookup"><span data-stu-id="11e56-118">Read properties and relationships of a synchronizationJob object.</span></span>|
|[<span data-ttu-id="11e56-119">Create</span><span class="sxs-lookup"><span data-stu-id="11e56-119">Create</span></span>](../api/synchronization-synchronizationjob-post.md)         |[<span data-ttu-id="11e56-120">synchronizationJob</span><span class="sxs-lookup"><span data-stu-id="11e56-120">synchronizationJob</span></span>](synchronization-synchronizationjob.md)   |<span data-ttu-id="11e56-121">Erstellen Sie neuen Auftrag für eine bestimmte Anwendung.</span><span class="sxs-lookup"><span data-stu-id="11e56-121">Create new job for a given application.</span></span>|
|[<span data-ttu-id="11e56-122">Start</span><span class="sxs-lookup"><span data-stu-id="11e56-122">Start</span></span>](../api/synchronization-synchronizationjob-start.md)          |<span data-ttu-id="11e56-123">Keine</span><span class="sxs-lookup"><span data-stu-id="11e56-123">None</span></span>   |<span data-ttu-id="11e56-124">Starten Sie die Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="11e56-124">Start synchronization.</span></span> <span data-ttu-id="11e56-125">Wenn der Auftrag angehalten ist, der weiterhin an der Stelle, an dem der Auftrag angehalten wurde.</span><span class="sxs-lookup"><span data-stu-id="11e56-125">If the job is in a paused state, it continues from the point where the job was paused.</span></span> <span data-ttu-id="11e56-126">Wenn der Auftrag in Quarantäne befindet, wird der Quarantänestatus gelöscht.</span><span class="sxs-lookup"><span data-stu-id="11e56-126">If the job is in quarantine, the quarantine status is cleared.</span></span>|
|[<span data-ttu-id="11e56-127">Restart</span><span class="sxs-lookup"><span data-stu-id="11e56-127">Restart</span></span>](../api/synchronization-synchronizationjob-restart.md)      |<span data-ttu-id="11e56-128">Keine</span><span class="sxs-lookup"><span data-stu-id="11e56-128">None</span></span>   |<span data-ttu-id="11e56-129">Erzwingen, dass des Auftrags beginnen soll, und alle Objekte im Verzeichnis erneut verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="11e56-129">Force the job to start over and re-process all the objects in the directory.</span></span>|
|[<span data-ttu-id="11e56-130">Pause</span><span class="sxs-lookup"><span data-stu-id="11e56-130">Pause</span></span>](../api/synchronization-synchronizationjob-pause.md)          |<span data-ttu-id="11e56-131">Keine</span><span class="sxs-lookup"><span data-stu-id="11e56-131">None</span></span>   |<span data-ttu-id="11e56-132">Synchronisierung vorübergehend anhalten.</span><span class="sxs-lookup"><span data-stu-id="11e56-132">Temporarily stop synchronization.</span></span> <span data-ttu-id="11e56-133">Der Fortschritt Auftragsstatus, einschließlich wird beibehalten, und der Auftrag wird weiterhin aus, wo es beim [Starten](../api/synchronization-synchronizationjob-start.md) aufgerufen wird unterbrochen.</span><span class="sxs-lookup"><span data-stu-id="11e56-133">All the progress, including job state, is persisted, and the job will continue from where it left off when a [Start](../api/synchronization-synchronizationjob-start.md) call is made.</span></span>|
|[<span data-ttu-id="11e56-134">Delete</span><span class="sxs-lookup"><span data-stu-id="11e56-134">Delete</span></span>](../api/synchronization-synchronizationjob-delete.md)        |<span data-ttu-id="11e56-135">Keine</span><span class="sxs-lookup"><span data-stu-id="11e56-135">None</span></span>   |<span data-ttu-id="11e56-136">Anhalten Sie Synchronisierung, und löschen Sie alle den Status des Auftrags zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="11e56-136">Stop synchronization, and permanently delete all the state associated with the job.</span></span>|
|[<span data-ttu-id="11e56-137">Abrufen von synchrnoizationSchema</span><span class="sxs-lookup"><span data-stu-id="11e56-137">Get synchrnoizationSchema</span></span>](../api/synchronization-synchronizationschema-get.md)    |[<span data-ttu-id="11e56-138">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="11e56-138">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)   |<span data-ttu-id="11e56-139">Rufen Sie den Auftrag effektive Synchronisierungsschema ab.</span><span class="sxs-lookup"><span data-stu-id="11e56-139">Retrieve the job's effective synchronization schema.</span></span>|
|[<span data-ttu-id="11e56-140">SynchroizationSchema aktualisieren</span><span class="sxs-lookup"><span data-stu-id="11e56-140">Update synchroizationSchema</span></span>](../api/synchronization-synchronizationschema-update.md)    |<span data-ttu-id="11e56-141">Keine</span><span class="sxs-lookup"><span data-stu-id="11e56-141">None</span></span>   |<span data-ttu-id="11e56-142">Aktualisieren des Schemas für den Auftrag-Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="11e56-142">Update the job's synchronization schema.</span></span> |
|[<span data-ttu-id="11e56-143">Überprüfen von Anmeldeinformationen</span><span class="sxs-lookup"><span data-stu-id="11e56-143">Validate credentials</span></span>](../api/synchronization-synchronizationjob-validatecredentials.md)|<span data-ttu-id="11e56-144">Keine</span><span class="sxs-lookup"><span data-stu-id="11e56-144">None</span></span>|<span data-ttu-id="11e56-145">Testen Sie die angegebene Anmeldeinformationen gegen Zielverzeichnis.</span><span class="sxs-lookup"><span data-stu-id="11e56-145">Test provided credentials against target directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="11e56-146">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="11e56-146">Properties</span></span>

| <span data-ttu-id="11e56-147">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="11e56-147">Property</span></span>      | <span data-ttu-id="11e56-148">Typ</span><span class="sxs-lookup"><span data-stu-id="11e56-148">Type</span></span>      | <span data-ttu-id="11e56-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11e56-149">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="11e56-150">id</span><span class="sxs-lookup"><span data-stu-id="11e56-150">id</span></span>             |<span data-ttu-id="11e56-151">String</span><span class="sxs-lookup"><span data-stu-id="11e56-151">String</span></span>                     |<span data-ttu-id="11e56-152">Auftrags-ID eindeutig Synchronisierung.</span><span class="sxs-lookup"><span data-stu-id="11e56-152">Unique synchronization job identifier.</span></span> <span data-ttu-id="11e56-153">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="11e56-153">Read-only.</span></span>|
|<span data-ttu-id="11e56-154">Zeitplan</span><span class="sxs-lookup"><span data-stu-id="11e56-154">schedule</span></span>       |[<span data-ttu-id="11e56-155">synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="11e56-155">synchronizationSchedule</span></span>](synchronization-synchronizationschedule.md)|<span data-ttu-id="11e56-156">Zeitplan zum Ausführen des Auftrags verwendet.</span><span class="sxs-lookup"><span data-stu-id="11e56-156">Schedule used to run the job.</span></span> <span data-ttu-id="11e56-157">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="11e56-157">Read-only.</span></span>|
|<span data-ttu-id="11e56-158">status</span><span class="sxs-lookup"><span data-stu-id="11e56-158">status</span></span>         |[<span data-ttu-id="11e56-159">synchronizationStatus</span><span class="sxs-lookup"><span data-stu-id="11e56-159">synchronizationStatus</span></span>](synchronization-synchronizationstatus.md)     |<span data-ttu-id="11e56-160">Status des Auftrags, die bei der letzten des Auftrags Ausführung enthält, aktuellen Auftragsstatus und Fehler.</span><span class="sxs-lookup"><span data-stu-id="11e56-160">Status of the job, which includes when the job was last run, current job state, and errors.</span></span>|
|<span data-ttu-id="11e56-161">templateId</span><span class="sxs-lookup"><span data-stu-id="11e56-161">templateId</span></span>     |<span data-ttu-id="11e56-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="11e56-162">String</span></span>    |<span data-ttu-id="11e56-163">Bezeichner der [Synchronisierung Vorlage](synchronization-synchronizationtemplate.md) basiert auf diesen Auftrag.</span><span class="sxs-lookup"><span data-stu-id="11e56-163">Identifier of the [synchronization template](synchronization-synchronizationtemplate.md) this job is based on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11e56-164">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="11e56-164">Relationships</span></span>
| <span data-ttu-id="11e56-165">Beziehung</span><span class="sxs-lookup"><span data-stu-id="11e56-165">Relationship</span></span> | <span data-ttu-id="11e56-166">Typ</span><span class="sxs-lookup"><span data-stu-id="11e56-166">Type</span></span>   |<span data-ttu-id="11e56-167">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11e56-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11e56-168">Schema</span><span class="sxs-lookup"><span data-stu-id="11e56-168">schema</span></span>|[<span data-ttu-id="11e56-169">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="11e56-169">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)| <span data-ttu-id="11e56-170">Die Synchronisierungsschema-für den Auftrag konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="11e56-170">The synchronization schema configured for the job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11e56-171">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="11e56-171">JSON representation</span></span>

<span data-ttu-id="11e56-172">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="11e56-172">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJob"
}-->

```json
{
  "id": "String (identifier)",
  "schedule": {"@odata.type": "microsoft.graph.synchronizationSchedule"},
  "status": {"@odata.type": "microsoft.graph.synchronizationStatus"},
  "templateId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationjob.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
