---
title: Prozess Ressourcentyp
description: Statusinformationen über den Prozess im Zusammenhang mit der Benachrichtigung enthält.
ms.openlocfilehash: 67bc65cfa47cda877578d89aa20c4e34b3a0c501
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018942"
---
# <a name="process-resource-type"></a><span data-ttu-id="f87fd-103">Prozess Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f87fd-103">process resource type</span></span>

<span data-ttu-id="f87fd-104">Statusinformationen über den Prozess im Zusammenhang mit der Benachrichtigung enthält.</span><span class="sxs-lookup"><span data-stu-id="f87fd-104">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="f87fd-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f87fd-105">Properties</span></span>

| <span data-ttu-id="f87fd-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f87fd-106">Property</span></span>   | <span data-ttu-id="f87fd-107">Typ</span><span class="sxs-lookup"><span data-stu-id="f87fd-107">Type</span></span>|<span data-ttu-id="f87fd-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f87fd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f87fd-109">accountName</span><span class="sxs-lookup"><span data-stu-id="f87fd-109">accountName</span></span>|<span data-ttu-id="f87fd-110">String</span><span class="sxs-lookup"><span data-stu-id="f87fd-110">String</span></span>|<span data-ttu-id="f87fd-111">Benutzerkonto für Beispiel, Kontoname, SID und So weiter Bezeichner (Konto Benutzerkontext, unter dem Prozess steht).</span><span class="sxs-lookup"><span data-stu-id="f87fd-111">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="f87fd-112">commandLine</span><span class="sxs-lookup"><span data-stu-id="f87fd-112">commandLine</span></span>|<span data-ttu-id="f87fd-113">String</span><span class="sxs-lookup"><span data-stu-id="f87fd-113">String</span></span>|<span data-ttu-id="f87fd-114">Vollständiger Prozess Aufruf Commandline einschließlich aller Parameter.</span><span class="sxs-lookup"><span data-stu-id="f87fd-114">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="f87fd-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f87fd-115">createdDateTime</span></span>|<span data-ttu-id="f87fd-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f87fd-116">DateTimeOffset</span></span>|<span data-ttu-id="f87fd-117">Zeitpunkt, an dem der Prozess gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="f87fd-117">Time at which the process was started.</span></span> <span data-ttu-id="f87fd-118">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="f87fd-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f87fd-119">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f87fd-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f87fd-120">fileHash</span><span class="sxs-lookup"><span data-stu-id="f87fd-120">fileHash</span></span>|[<span data-ttu-id="f87fd-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="f87fd-121">fileHash</span></span>](filehash.md)|<span data-ttu-id="f87fd-122">Komplexer Typ mit Dateihashes (cryptographic und der Speicherort).</span><span class="sxs-lookup"><span data-stu-id="f87fd-122">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="f87fd-123">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="f87fd-123">integrityLevel</span></span>|<span data-ttu-id="f87fd-124">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="f87fd-124">processIntegrityLevel</span></span>|<span data-ttu-id="f87fd-125">Die Integritätsebene des Prozesses.</span><span class="sxs-lookup"><span data-stu-id="f87fd-125">The integrity level of the process.</span></span> <span data-ttu-id="f87fd-126">Mögliche Werte sind: `unknown`, `untrusted`, `low`, `medium`, `high` und `system`.</span><span class="sxs-lookup"><span data-stu-id="f87fd-126">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="f87fd-127">isElevated</span><span class="sxs-lookup"><span data-stu-id="f87fd-127">isElevated</span></span>|<span data-ttu-id="f87fd-128">Boolesch</span><span class="sxs-lookup"><span data-stu-id="f87fd-128">Boolean</span></span>|<span data-ttu-id="f87fd-129">True, wenn der Prozess erweitert wird.</span><span class="sxs-lookup"><span data-stu-id="f87fd-129">True if the process is elevated.</span></span>|
|<span data-ttu-id="f87fd-130">name</span><span class="sxs-lookup"><span data-stu-id="f87fd-130">name</span></span>|<span data-ttu-id="f87fd-131">String</span><span class="sxs-lookup"><span data-stu-id="f87fd-131">String</span></span>|<span data-ttu-id="f87fd-132">Der Name der Bilddatei des Prozesses.</span><span class="sxs-lookup"><span data-stu-id="f87fd-132">The name of the process' Image file.</span></span>|
|<span data-ttu-id="f87fd-133">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f87fd-133">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="f87fd-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f87fd-134">DateTimeOffset</span></span>|<span data-ttu-id="f87fd-135">DateTime, an dem der übergeordnete Prozess gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="f87fd-135">DateTime at which the parent process was started.</span></span> <span data-ttu-id="f87fd-136">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="f87fd-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f87fd-137">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f87fd-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f87fd-138">Diese Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f87fd-138">parentProcessId</span></span>|<span data-ttu-id="f87fd-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f87fd-139">Int32</span></span>|<span data-ttu-id="f87fd-140">Die Prozess-ID (PID) des übergeordneten Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="f87fd-140">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="f87fd-141">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="f87fd-141">parentProcessName</span></span>|<span data-ttu-id="f87fd-142">String</span><span class="sxs-lookup"><span data-stu-id="f87fd-142">String</span></span>|<span data-ttu-id="f87fd-143">Der Name der Bilddatei des übergeordneten Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="f87fd-143">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="f87fd-144">Pfad</span><span class="sxs-lookup"><span data-stu-id="f87fd-144">path</span></span>|<span data-ttu-id="f87fd-145">String</span><span class="sxs-lookup"><span data-stu-id="f87fd-145">String</span></span>|<span data-ttu-id="f87fd-146">Vollständiger Pfad, einschließlich Dateiname.</span><span class="sxs-lookup"><span data-stu-id="f87fd-146">Full path, including filename.</span></span>|
|<span data-ttu-id="f87fd-147">processId</span><span class="sxs-lookup"><span data-stu-id="f87fd-147">processId</span></span>|<span data-ttu-id="f87fd-148">Int32</span><span class="sxs-lookup"><span data-stu-id="f87fd-148">Int32</span></span>|<span data-ttu-id="f87fd-149">Die Prozess-ID (PID) des Prozesses.</span><span class="sxs-lookup"><span data-stu-id="f87fd-149">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f87fd-150">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f87fd-150">JSON representation</span></span>

<span data-ttu-id="f87fd-151">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f87fd-151">The following is a JSON representation of the resource.</span></span>

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