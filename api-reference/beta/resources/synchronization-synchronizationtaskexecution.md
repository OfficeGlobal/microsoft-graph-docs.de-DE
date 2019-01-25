---
title: Ressourcentyp synchronizationTaskExecution
description: Enthält eine Zusammenfassung der Ergebnisse der Synchronisierungsauftrag ausführen.
localization_priority: Normal
ms.openlocfilehash: 37a0fd57269cef6d3cb03c5cc5c38d3024fe198d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510554"
---
# <a name="synchronizationtaskexecution-resource-type"></a><span data-ttu-id="f932e-103">Ressourcentyp synchronizationTaskExecution</span><span class="sxs-lookup"><span data-stu-id="f932e-103">synchronizationTaskExecution resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f932e-104">Enthält eine Zusammenfassung der Ergebnisse der Synchronisierungsauftrag ausführen.</span><span class="sxs-lookup"><span data-stu-id="f932e-104">Summarizes the results of the synchronization job run.</span></span>

## <a name="properties"></a><span data-ttu-id="f932e-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f932e-105">Properties</span></span>
| <span data-ttu-id="f932e-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f932e-106">Property</span></span>     | <span data-ttu-id="f932e-107">Typ</span><span class="sxs-lookup"><span data-stu-id="f932e-107">Type</span></span>   |<span data-ttu-id="f932e-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f932e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f932e-109">activityIdentifier</span><span class="sxs-lookup"><span data-stu-id="f932e-109">activityIdentifier</span></span>           |<span data-ttu-id="f932e-110">String</span><span class="sxs-lookup"><span data-stu-id="f932e-110">String</span></span> |<span data-ttu-id="f932e-111">Bezeichner des Auftrags ausgeführt.</span><span class="sxs-lookup"><span data-stu-id="f932e-111">Identifier of the job run.</span></span>|
|<span data-ttu-id="f932e-112">countEntitled</span><span class="sxs-lookup"><span data-stu-id="f932e-112">countEntitled</span></span>                |<span data-ttu-id="f932e-113">Int64</span><span class="sxs-lookup"><span data-stu-id="f932e-113">Int64</span></span>  |<span data-ttu-id="f932e-114">Anzahl der verarbeiteten Einträge, die für diese Anwendung zugewiesen wurden.</span><span class="sxs-lookup"><span data-stu-id="f932e-114">Count of processed entries that were assigned for this application.</span></span>|
|<span data-ttu-id="f932e-115">countEntitledForProvisioning</span><span class="sxs-lookup"><span data-stu-id="f932e-115">countEntitledForProvisioning</span></span> |<span data-ttu-id="f932e-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f932e-116">Int64</span></span>  |<span data-ttu-id="f932e-117">Anzahl der verarbeiteten Einträge, die für die Bereitstellung zugewiesen wurden.</span><span class="sxs-lookup"><span data-stu-id="f932e-117">Count of processed entries that were assigned for provisioning.</span></span>|
|<span data-ttu-id="f932e-118">countEscrowed</span><span class="sxs-lookup"><span data-stu-id="f932e-118">countEscrowed</span></span>                |<span data-ttu-id="f932e-119">Int64</span><span class="sxs-lookup"><span data-stu-id="f932e-119">Int64</span></span>  |<span data-ttu-id="f932e-120">Anzahl der Einträge, die escrowed (Fehler) waren.</span><span class="sxs-lookup"><span data-stu-id="f932e-120">Count of entries that were escrowed (errors).</span></span>|
|<span data-ttu-id="f932e-121">countEscrowedRaw</span><span class="sxs-lookup"><span data-stu-id="f932e-121">countEscrowedRaw</span></span>             |<span data-ttu-id="f932e-122">Int64</span><span class="sxs-lookup"><span data-stu-id="f932e-122">Int64</span></span>  |<span data-ttu-id="f932e-123">Anzahl der Einträge, die vom System generierte Artikel mit Treuhandservice einschließlich escrowed wurden.</span><span class="sxs-lookup"><span data-stu-id="f932e-123">Count of entries that were escrowed, including system-generated escrows.</span></span>|
|<span data-ttu-id="f932e-124">countExported</span><span class="sxs-lookup"><span data-stu-id="f932e-124">countExported</span></span>                |<span data-ttu-id="f932e-125">Int64</span><span class="sxs-lookup"><span data-stu-id="f932e-125">Int64</span></span>  |<span data-ttu-id="f932e-126">Anzahl der exportierten Posten.</span><span class="sxs-lookup"><span data-stu-id="f932e-126">Count of exported entries.</span></span>|
|<span data-ttu-id="f932e-127">countExports</span><span class="sxs-lookup"><span data-stu-id="f932e-127">countExports</span></span>                 |<span data-ttu-id="f932e-128">Int64</span><span class="sxs-lookup"><span data-stu-id="f932e-128">Int64</span></span>  |<span data-ttu-id="f932e-129">Anzahl der Einträge, die erwartet wurden, exportiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="f932e-129">Count of entries that were expected to be exported.</span></span>|
|<span data-ttu-id="f932e-130">countImported</span><span class="sxs-lookup"><span data-stu-id="f932e-130">countImported</span></span>                |<span data-ttu-id="f932e-131">Int64</span><span class="sxs-lookup"><span data-stu-id="f932e-131">Int64</span></span>  |<span data-ttu-id="f932e-132">Anzahl der importierten Einträge.</span><span class="sxs-lookup"><span data-stu-id="f932e-132">Count of imported entries.</span></span>|
|<span data-ttu-id="f932e-133">countImportedDeltas</span><span class="sxs-lookup"><span data-stu-id="f932e-133">countImportedDeltas</span></span>          |<span data-ttu-id="f932e-134">Int64</span><span class="sxs-lookup"><span data-stu-id="f932e-134">Int64</span></span>  |<span data-ttu-id="f932e-135">Anzahl der importierten Delta-Änderungen.</span><span class="sxs-lookup"><span data-stu-id="f932e-135">Count of imported delta-changes.</span></span>|
|<span data-ttu-id="f932e-136">countImportedReferenceDeltas</span><span class="sxs-lookup"><span data-stu-id="f932e-136">countImportedReferenceDeltas</span></span> |<span data-ttu-id="f932e-137">Int64</span><span class="sxs-lookup"><span data-stu-id="f932e-137">Int64</span></span>  |<span data-ttu-id="f932e-138">Anzahl der importierten Delta-Änderungen, die Verweis ändert betreffen.</span><span class="sxs-lookup"><span data-stu-id="f932e-138">Count of imported delta-changes pertaining to reference changes.</span></span>|
|<span data-ttu-id="f932e-139">error</span><span class="sxs-lookup"><span data-stu-id="f932e-139">error</span></span>                        |[<span data-ttu-id="f932e-140">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="f932e-140">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="f932e-141">Wenn ein Fehler aufgetreten ist, enthält ein **SynchronizationError** -Objekt mit Details.</span><span class="sxs-lookup"><span data-stu-id="f932e-141">If an error was encountered, contains a **synchronizationError** object with details.</span></span>|
|<span data-ttu-id="f932e-142">state</span><span class="sxs-lookup"><span data-stu-id="f932e-142">state</span></span>                        |<span data-ttu-id="f932e-143">String</span><span class="sxs-lookup"><span data-stu-id="f932e-143">String</span></span> |<span data-ttu-id="f932e-144">Zusammenfassen das Ergebnis dieser Ausführung von Code.</span><span class="sxs-lookup"><span data-stu-id="f932e-144">Code summarizing the result of this run.</span></span> <span data-ttu-id="f932e-145">Mögliche Werte sind: `Succeeded`, `Failed` und `EntryLevelErrors`.</span><span class="sxs-lookup"><span data-stu-id="f932e-145">Possible values are: `Succeeded`, `Failed`, `EntryLevelErrors`.</span></span>|
|<span data-ttu-id="f932e-146">timeBegan</span><span class="sxs-lookup"><span data-stu-id="f932e-146">timeBegan</span></span>                    |<span data-ttu-id="f932e-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f932e-147">DateTimeOffset</span></span>|<span data-ttu-id="f932e-148">Uhrzeit diesen Auftrag Ausführung begonnen hat.</span><span class="sxs-lookup"><span data-stu-id="f932e-148">Time when this job run began.</span></span> <span data-ttu-id="f932e-149">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="f932e-149">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f932e-150">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f932e-150">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f932e-151">timeEnded</span><span class="sxs-lookup"><span data-stu-id="f932e-151">timeEnded</span></span>                    |<span data-ttu-id="f932e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f932e-152">DateTimeOffset</span></span>|<span data-ttu-id="f932e-153">Zeitpunkt der Ausführung dieser Auftrag beendet wurde.</span><span class="sxs-lookup"><span data-stu-id="f932e-153">Time when this job run ended.</span></span> <span data-ttu-id="f932e-154">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="f932e-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f932e-155">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f932e-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f932e-156">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f932e-156">JSON representation</span></span>

<span data-ttu-id="f932e-157">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f932e-157">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationtaskexecution.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
