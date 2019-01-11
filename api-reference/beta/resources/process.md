---
title: Prozess Ressourcentyp
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 36acd6ed0f6e2cee5095d445de3ba4ff024a024a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869468"
---
# <a name="process-resource-type"></a><span data-ttu-id="08317-104">Prozess Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="08317-104">process resource type</span></span>

 > <span data-ttu-id="08317-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="08317-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08317-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="08317-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08317-107">Statusinformationen über den Prozess im Zusammenhang mit der Benachrichtigung enthält.</span><span class="sxs-lookup"><span data-stu-id="08317-107">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="08317-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="08317-108">Properties</span></span>

| <span data-ttu-id="08317-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08317-109">Property</span></span>   | <span data-ttu-id="08317-110">Typ</span><span class="sxs-lookup"><span data-stu-id="08317-110">Type</span></span>|<span data-ttu-id="08317-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="08317-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08317-112">accountName</span><span class="sxs-lookup"><span data-stu-id="08317-112">accountName</span></span>|<span data-ttu-id="08317-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08317-113">String</span></span>|<span data-ttu-id="08317-114">Benutzerkonto für Beispiel, Kontoname, SID und So weiter Bezeichner (Konto Benutzerkontext, unter dem Prozess steht).</span><span class="sxs-lookup"><span data-stu-id="08317-114">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="08317-115">commandLine</span><span class="sxs-lookup"><span data-stu-id="08317-115">commandLine</span></span>|<span data-ttu-id="08317-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08317-116">String</span></span>|<span data-ttu-id="08317-117">Vollständiger Prozess Aufruf Commandline einschließlich aller Parameter.</span><span class="sxs-lookup"><span data-stu-id="08317-117">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="08317-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08317-118">createdDateTime</span></span>|<span data-ttu-id="08317-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08317-119">DateTimeOffset</span></span>|<span data-ttu-id="08317-120">Zeitpunkt, an dem der Prozess gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="08317-120">Time at which the process was started.</span></span> <span data-ttu-id="08317-121">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="08317-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="08317-122">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="08317-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="08317-123">fileHash</span><span class="sxs-lookup"><span data-stu-id="08317-123">fileHash</span></span>|[<span data-ttu-id="08317-124">fileHash</span><span class="sxs-lookup"><span data-stu-id="08317-124">fileHash</span></span>](filehash.md)|<span data-ttu-id="08317-125">Komplexer Typ mit Dateihashes (cryptographic und der Speicherort).</span><span class="sxs-lookup"><span data-stu-id="08317-125">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="08317-126">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="08317-126">integrityLevel</span></span>|<span data-ttu-id="08317-127">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="08317-127">processIntegrityLevel</span></span>|<span data-ttu-id="08317-128">Die Integritätsebene des Prozesses.</span><span class="sxs-lookup"><span data-stu-id="08317-128">The integrity level of the process.</span></span> <span data-ttu-id="08317-129">Mögliche Werte sind: `unknown`, `untrusted`, `low`, `medium`, `high` und `system`.</span><span class="sxs-lookup"><span data-stu-id="08317-129">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="08317-130">isElevated</span><span class="sxs-lookup"><span data-stu-id="08317-130">isElevated</span></span>|<span data-ttu-id="08317-131">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="08317-131">Boolean</span></span>|<span data-ttu-id="08317-132">True, wenn der Prozess erweitert wird.</span><span class="sxs-lookup"><span data-stu-id="08317-132">True if the process is elevated.</span></span>|
|<span data-ttu-id="08317-133">name</span><span class="sxs-lookup"><span data-stu-id="08317-133">name</span></span>|<span data-ttu-id="08317-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08317-134">String</span></span>|<span data-ttu-id="08317-135">Der Name der Bilddatei des Prozesses.</span><span class="sxs-lookup"><span data-stu-id="08317-135">The name of the process' Image file.</span></span>|
|<span data-ttu-id="08317-136">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="08317-136">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="08317-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08317-137">DateTimeOffset</span></span>|<span data-ttu-id="08317-138">DateTime, an dem der übergeordnete Prozess gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="08317-138">DateTime at which the parent process was started.</span></span> <span data-ttu-id="08317-139">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="08317-139">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="08317-140">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="08317-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="08317-141">Diese Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="08317-141">parentProcessId</span></span>|<span data-ttu-id="08317-142">Int32</span><span class="sxs-lookup"><span data-stu-id="08317-142">Int32</span></span>|<span data-ttu-id="08317-143">Die Prozess-ID (PID) des übergeordneten Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="08317-143">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="08317-144">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="08317-144">parentProcessName</span></span>|<span data-ttu-id="08317-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08317-145">String</span></span>|<span data-ttu-id="08317-146">Der Name der Bilddatei des übergeordneten Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="08317-146">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="08317-147">Pfad</span><span class="sxs-lookup"><span data-stu-id="08317-147">path</span></span>|<span data-ttu-id="08317-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="08317-148">String</span></span>|<span data-ttu-id="08317-149">Vollständiger Pfad, einschließlich Dateiname.</span><span class="sxs-lookup"><span data-stu-id="08317-149">Full path, including filename.</span></span>|
|<span data-ttu-id="08317-150">processId</span><span class="sxs-lookup"><span data-stu-id="08317-150">processId</span></span>|<span data-ttu-id="08317-151">Int32</span><span class="sxs-lookup"><span data-stu-id="08317-151">Int32</span></span>|<span data-ttu-id="08317-152">Die Prozess-ID (PID) des Prozesses.</span><span class="sxs-lookup"><span data-stu-id="08317-152">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08317-153">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="08317-153">JSON representation</span></span>

<span data-ttu-id="08317-154">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="08317-154">The following is a JSON representation of the resource.</span></span>

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
