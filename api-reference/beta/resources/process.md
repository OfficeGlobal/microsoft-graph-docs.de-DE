---
title: Prozess Ressourcentyp
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: 2e60c9e008ccfddaa0bcc3e78c27cc17c65a3844
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061376"
---
# <a name="process-resource-type"></a><span data-ttu-id="adca7-104">Prozess Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="adca7-104">process resource type</span></span>

 > <span data-ttu-id="adca7-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="adca7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="adca7-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="adca7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="adca7-107">Statusinformationen über den Prozess im Zusammenhang mit der Benachrichtigung enthält.</span><span class="sxs-lookup"><span data-stu-id="adca7-107">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="adca7-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="adca7-108">Properties</span></span>

| <span data-ttu-id="adca7-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="adca7-109">Property</span></span>   | <span data-ttu-id="adca7-110">Typ</span><span class="sxs-lookup"><span data-stu-id="adca7-110">Type</span></span>|<span data-ttu-id="adca7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="adca7-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adca7-112">accountName</span><span class="sxs-lookup"><span data-stu-id="adca7-112">accountName</span></span>|<span data-ttu-id="adca7-113">String</span><span class="sxs-lookup"><span data-stu-id="adca7-113">String</span></span>|<span data-ttu-id="adca7-114">Benutzerkonto für Beispiel, Kontoname, SID und So weiter Bezeichner (Konto Benutzerkontext, unter dem Prozess steht).</span><span class="sxs-lookup"><span data-stu-id="adca7-114">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="adca7-115">commandLine</span><span class="sxs-lookup"><span data-stu-id="adca7-115">commandLine</span></span>|<span data-ttu-id="adca7-116">String</span><span class="sxs-lookup"><span data-stu-id="adca7-116">String</span></span>|<span data-ttu-id="adca7-117">Vollständiger Prozess Aufruf Commandline einschließlich aller Parameter.</span><span class="sxs-lookup"><span data-stu-id="adca7-117">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="adca7-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="adca7-118">createdDateTime</span></span>|<span data-ttu-id="adca7-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adca7-119">DateTimeOffset</span></span>|<span data-ttu-id="adca7-120">Zeitpunkt, an dem der Prozess gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="adca7-120">Time at which the process was started.</span></span> <span data-ttu-id="adca7-121">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="adca7-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="adca7-122">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="adca7-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="adca7-123">fileHash</span><span class="sxs-lookup"><span data-stu-id="adca7-123">fileHash</span></span>|[<span data-ttu-id="adca7-124">fileHash</span><span class="sxs-lookup"><span data-stu-id="adca7-124">fileHash</span></span>](filehash.md)|<span data-ttu-id="adca7-125">Komplexer Typ mit Dateihashes (cryptographic und der Speicherort).</span><span class="sxs-lookup"><span data-stu-id="adca7-125">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="adca7-126">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="adca7-126">integrityLevel</span></span>|<span data-ttu-id="adca7-127">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="adca7-127">processIntegrityLevel</span></span>|<span data-ttu-id="adca7-128">Die Integritätsebene des Prozesses.</span><span class="sxs-lookup"><span data-stu-id="adca7-128">The integrity level of the process.</span></span> <span data-ttu-id="adca7-129">Mögliche Werte sind: `unknown`, `untrusted`, `low`, `medium`, `high` und `system`.</span><span class="sxs-lookup"><span data-stu-id="adca7-129">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="adca7-130">isElevated</span><span class="sxs-lookup"><span data-stu-id="adca7-130">isElevated</span></span>|<span data-ttu-id="adca7-131">Boolesch</span><span class="sxs-lookup"><span data-stu-id="adca7-131">Boolean</span></span>|<span data-ttu-id="adca7-132">True, wenn der Prozess erweitert wird.</span><span class="sxs-lookup"><span data-stu-id="adca7-132">True if the process is elevated.</span></span>|
|<span data-ttu-id="adca7-133">name</span><span class="sxs-lookup"><span data-stu-id="adca7-133">name</span></span>|<span data-ttu-id="adca7-134">String</span><span class="sxs-lookup"><span data-stu-id="adca7-134">String</span></span>|<span data-ttu-id="adca7-135">Der Name der Bilddatei des Prozesses.</span><span class="sxs-lookup"><span data-stu-id="adca7-135">The name of the process' Image file.</span></span>|
|<span data-ttu-id="adca7-136">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="adca7-136">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="adca7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adca7-137">DateTimeOffset</span></span>|<span data-ttu-id="adca7-138">DateTime, an dem der übergeordnete Prozess gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="adca7-138">DateTime at which the parent process was started.</span></span> <span data-ttu-id="adca7-139">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="adca7-139">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="adca7-140">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="adca7-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="adca7-141">Diese Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="adca7-141">parentProcessId</span></span>|<span data-ttu-id="adca7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="adca7-142">Int32</span></span>|<span data-ttu-id="adca7-143">Die Prozess-ID (PID) des übergeordneten Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="adca7-143">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="adca7-144">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="adca7-144">parentProcessName</span></span>|<span data-ttu-id="adca7-145">String</span><span class="sxs-lookup"><span data-stu-id="adca7-145">String</span></span>|<span data-ttu-id="adca7-146">Der Name der Bilddatei des übergeordneten Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="adca7-146">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="adca7-147">Pfad</span><span class="sxs-lookup"><span data-stu-id="adca7-147">path</span></span>|<span data-ttu-id="adca7-148">String</span><span class="sxs-lookup"><span data-stu-id="adca7-148">String</span></span>|<span data-ttu-id="adca7-149">Vollständiger Pfad, einschließlich Dateiname.</span><span class="sxs-lookup"><span data-stu-id="adca7-149">Full path, including filename.</span></span>|
|<span data-ttu-id="adca7-150">processId</span><span class="sxs-lookup"><span data-stu-id="adca7-150">processId</span></span>|<span data-ttu-id="adca7-151">Int32</span><span class="sxs-lookup"><span data-stu-id="adca7-151">Int32</span></span>|<span data-ttu-id="adca7-152">Die Prozess-ID (PID) des Prozesses.</span><span class="sxs-lookup"><span data-stu-id="adca7-152">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="adca7-153">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="adca7-153">JSON representation</span></span>

<span data-ttu-id="adca7-154">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="adca7-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.process"
}-->

```json
{
  "accountName": "String",
  "commandLine": "String",
  "createdDateTime": "String (timestamp)",
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
  "isElevated": true,
  "name": "String",
  "parentProcessCreatedDateTime": "String (timestamp)",
  "parentProcessId": 1024,
  "parentProcessName": "String",
  "path": "String",
  "processId": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->