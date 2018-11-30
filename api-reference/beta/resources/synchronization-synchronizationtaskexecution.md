---
title: Ressourcentyp synchronizationTaskExecution
description: Enthält eine Zusammenfassung der Ergebnisse der Synchronisierungsauftrag ausführen.
ms.openlocfilehash: 4aefba4bdf9ab850892344e6e34683e81d1a1afa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061911"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="ec60a-103">Ressourcentyp synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="ec60a-103">synchronizationTaskExecution resource type</span></span>

> <span data-ttu-id="ec60a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ec60a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec60a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ec60a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec60a-106">Enthält eine Zusammenfassung der Ergebnisse der Synchronisierungsauftrag ausführen.</span><span class="sxs-lookup"><span data-stu-id="ec60a-106">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="ec60a-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ec60a-107">Properties</span></span>
| <span data-ttu-id="ec60a-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ec60a-108">Property</span></span>     | <span data-ttu-id="ec60a-109">Typ</span><span class="sxs-lookup"><span data-stu-id="ec60a-109">Type</span></span>   |<span data-ttu-id="ec60a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec60a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec60a-111">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="ec60a-111">activityIdentifier</span></span>           |<span data-ttu-id="ec60a-112">String</span><span class="sxs-lookup"><span data-stu-id="ec60a-112">String</span></span> |<span data-ttu-id="ec60a-113">Bezeichner des Auftrags ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="ec60a-113">Identifier of the job run.</span></span>|
|<span data-ttu-id="ec60a-114">countEntitled</span><span class="sxs-lookup"><span data-stu-id="ec60a-114">countEntitled</span></span>                |<span data-ttu-id="ec60a-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ec60a-115">Int64</span></span>  |<span data-ttu-id="ec60a-116">Anzahl der verarbeiteten Einträge, die für diese Anwendung zugewiesen wurden.</span><span class="sxs-lookup"><span data-stu-id="ec60a-116">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="ec60a-117">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="ec60a-117">countEntitledForProvisioning</span></span> |<span data-ttu-id="ec60a-118">Int64</span><span class="sxs-lookup"><span data-stu-id="ec60a-118">Int64</span></span>  |<span data-ttu-id="ec60a-119">Anzahl der verarbeiteten Einträge, die für die Bereitstellung zugewiesen wurden.</span><span class="sxs-lookup"><span data-stu-id="ec60a-119">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="ec60a-120">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="ec60a-120">countEscrowed</span></span>                |<span data-ttu-id="ec60a-121">Int64</span><span class="sxs-lookup"><span data-stu-id="ec60a-121">Int64</span></span>  |<span data-ttu-id="ec60a-122">Anzahl der Einträge, die escrowed (Fehler) waren.</span><span class="sxs-lookup"><span data-stu-id="ec60a-122">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="ec60a-123">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="ec60a-123">countEscrowedRaw</span></span>             |<span data-ttu-id="ec60a-124">Int64</span><span class="sxs-lookup"><span data-stu-id="ec60a-124">Int64</span></span>  |<span data-ttu-id="ec60a-125">Anzahl der Einträge, die vom System generierte Artikel mit Treuhandservice einschließlich escrowed wurden.</span><span class="sxs-lookup"><span data-stu-id="ec60a-125">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="ec60a-126">countExported</span><span class="sxs-lookup"><span data-stu-id="ec60a-126">countExported</span></span>                |<span data-ttu-id="ec60a-127">Int64</span><span class="sxs-lookup"><span data-stu-id="ec60a-127">Int64</span></span>  |<span data-ttu-id="ec60a-128">Anzahl der exportierten Posten.</span><span class="sxs-lookup"><span data-stu-id="ec60a-128">Count of exported entries.</span></span>|
|<span data-ttu-id="ec60a-129">countExports</span><span class="sxs-lookup"><span data-stu-id="ec60a-129">countExports</span></span>                 |<span data-ttu-id="ec60a-130">Int64</span><span class="sxs-lookup"><span data-stu-id="ec60a-130">Int64</span></span>  |<span data-ttu-id="ec60a-131">Anzahl der Einträge, die erwartet wurden, exportiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ec60a-131">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="ec60a-132">countImported</span><span class="sxs-lookup"><span data-stu-id="ec60a-132">countImported</span></span>                |<span data-ttu-id="ec60a-133">Int64</span><span class="sxs-lookup"><span data-stu-id="ec60a-133">Int64</span></span>  |<span data-ttu-id="ec60a-134">Anzahl der importierten Einträge.</span><span class="sxs-lookup"><span data-stu-id="ec60a-134">Count of imported entries.</span></span>|
|<span data-ttu-id="ec60a-135">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="ec60a-135">countImportedDeltas</span></span>          |<span data-ttu-id="ec60a-136">Int64</span><span class="sxs-lookup"><span data-stu-id="ec60a-136">Int64</span></span>  |<span data-ttu-id="ec60a-137">Anzahl der importierten Delta-Änderungen.</span><span class="sxs-lookup"><span data-stu-id="ec60a-137">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="ec60a-138">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="ec60a-138">countImportedReferenceDeltas</span></span> |<span data-ttu-id="ec60a-139">Int64</span><span class="sxs-lookup"><span data-stu-id="ec60a-139">Int64</span></span>  |<span data-ttu-id="ec60a-140">Anzahl der importierten Delta-Änderungen, die Verweis ändert betreffen.</span><span class="sxs-lookup"><span data-stu-id="ec60a-140">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="ec60a-141">error</span><span class="sxs-lookup"><span data-stu-id="ec60a-141">error</span></span>                        |[<span data-ttu-id="ec60a-142">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="ec60a-142">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="ec60a-143">Wenn ein Fehler aufgetreten ist, enthält ein **SynchronizationError** -Objekt mit Details.</span><span class="sxs-lookup"><span data-stu-id="ec60a-143">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="ec60a-144">state</span><span class="sxs-lookup"><span data-stu-id="ec60a-144">state</span></span>                        |<span data-ttu-id="ec60a-145">String</span><span class="sxs-lookup"><span data-stu-id="ec60a-145">String</span></span> |<span data-ttu-id="ec60a-146">Zusammenfassen das Ergebnis dieser Ausführung von Code.</span><span class="sxs-lookup"><span data-stu-id="ec60a-146">Code summarizing the result of this run.</span></span> <span data-ttu-id="ec60a-147">Mögliche Werte sind: `Succeeded`, `Failed` und `EntryLevelErrors`.</span><span class="sxs-lookup"><span data-stu-id="ec60a-147">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="ec60a-148">timeBegan</span><span class="sxs-lookup"><span data-stu-id="ec60a-148">timeBegan</span></span>                    |<span data-ttu-id="ec60a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec60a-149">DateTimeOffset</span></span>|<span data-ttu-id="ec60a-150">Uhrzeit diesen Auftrag Ausführung begonnen hat.</span><span class="sxs-lookup"><span data-stu-id="ec60a-150">Time when this job run began.</span></span> <span data-ttu-id="ec60a-151">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="ec60a-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ec60a-152">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ec60a-152">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="ec60a-153">timeEnded</span><span class="sxs-lookup"><span data-stu-id="ec60a-153">timeEnded</span></span>                    |<span data-ttu-id="ec60a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec60a-154">DateTimeOffset</span></span>|<span data-ttu-id="ec60a-155">Zeitpunkt der Ausführung dieser Auftrag beendet wurde.</span><span class="sxs-lookup"><span data-stu-id="ec60a-155">Time when this job run ended.</span></span> <span data-ttu-id="ec60a-156">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="ec60a-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ec60a-157">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ec60a-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec60a-158">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ec60a-158">JSON representation</span></span>

<span data-ttu-id="ec60a-159">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ec60a-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationTaskExecution"
}-->

```json
{
  "activityIdentifier": "String",
  "countEntitled": 1024,
  "countEntitledForProvisioning": 1024,
  "countEscrowed": 1024,
  "countEscrowedRaw": 1024,
  "countExported": 1024,
  "countExports": 1024,
  "countImported": 1024,
  "countImportedDeltas": 1024,
  "countImportedReferenceDeltas": 1024,
  "error": {"@odata.type": "microsoft.graph.synchronizationError"},
  "state": "String",
  "timeBegan": "String (timestamp)",
  "timeEnded": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->