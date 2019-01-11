---
title: Prozess Ressourcentyp
description: Statusinformationen über den Prozess im Zusammenhang mit der Benachrichtigung enthält.
localization_priority: Normal
ms.openlocfilehash: 0b4207c1780dfd6327ceb67e837f793341e609ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864421"
---
# <a name="process-resource-type"></a><span data-ttu-id="635cd-103">Prozess Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="635cd-103">process resource type</span></span>

<span data-ttu-id="635cd-104">Statusinformationen über den Prozess im Zusammenhang mit der Benachrichtigung enthält.</span><span class="sxs-lookup"><span data-stu-id="635cd-104">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="635cd-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="635cd-105">Properties</span></span>

| <span data-ttu-id="635cd-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="635cd-106">Property</span></span>   | <span data-ttu-id="635cd-107">Typ</span><span class="sxs-lookup"><span data-stu-id="635cd-107">Type</span></span>|<span data-ttu-id="635cd-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="635cd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="635cd-109">accountName</span><span class="sxs-lookup"><span data-stu-id="635cd-109">accountName</span></span>|<span data-ttu-id="635cd-110">String</span><span class="sxs-lookup"><span data-stu-id="635cd-110">String</span></span>|<span data-ttu-id="635cd-111">Benutzerkonto für Beispiel, Kontoname, SID und So weiter Bezeichner (Konto Benutzerkontext, unter dem Prozess steht).</span><span class="sxs-lookup"><span data-stu-id="635cd-111">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="635cd-112">commandLine</span><span class="sxs-lookup"><span data-stu-id="635cd-112">commandLine</span></span>|<span data-ttu-id="635cd-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="635cd-113">String</span></span>|<span data-ttu-id="635cd-114">Vollständiger Prozess Aufruf Commandline einschließlich aller Parameter.</span><span class="sxs-lookup"><span data-stu-id="635cd-114">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="635cd-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="635cd-115">createdDateTime</span></span>|<span data-ttu-id="635cd-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="635cd-116">DateTimeOffset</span></span>|<span data-ttu-id="635cd-117">Zeitpunkt, an dem der Prozess gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="635cd-117">Time at which the process was started.</span></span> <span data-ttu-id="635cd-118">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="635cd-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="635cd-119">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="635cd-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="635cd-120">fileHash</span><span class="sxs-lookup"><span data-stu-id="635cd-120">fileHash</span></span>|[<span data-ttu-id="635cd-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="635cd-121">fileHash</span></span>](filehash.md)|<span data-ttu-id="635cd-122">Komplexer Typ mit Dateihashes (cryptographic und der Speicherort).</span><span class="sxs-lookup"><span data-stu-id="635cd-122">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="635cd-123">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="635cd-123">integrityLevel</span></span>|<span data-ttu-id="635cd-124">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="635cd-124">processIntegrityLevel</span></span>|<span data-ttu-id="635cd-125">Die Integritätsebene des Prozesses.</span><span class="sxs-lookup"><span data-stu-id="635cd-125">The integrity level of the process.</span></span> <span data-ttu-id="635cd-126">Mögliche Werte sind: `unknown`, `untrusted`, `low`, `medium`, `high` und `system`.</span><span class="sxs-lookup"><span data-stu-id="635cd-126">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="635cd-127">isElevated</span><span class="sxs-lookup"><span data-stu-id="635cd-127">isElevated</span></span>|<span data-ttu-id="635cd-128">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="635cd-128">Boolean</span></span>|<span data-ttu-id="635cd-129">True, wenn der Prozess erweitert wird.</span><span class="sxs-lookup"><span data-stu-id="635cd-129">True if the process is elevated.</span></span>|
|<span data-ttu-id="635cd-130">name</span><span class="sxs-lookup"><span data-stu-id="635cd-130">name</span></span>|<span data-ttu-id="635cd-131">String</span><span class="sxs-lookup"><span data-stu-id="635cd-131">String</span></span>|<span data-ttu-id="635cd-132">Der Name der Bilddatei des Prozesses.</span><span class="sxs-lookup"><span data-stu-id="635cd-132">The name of the process' Image file.</span></span>|
|<span data-ttu-id="635cd-133">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="635cd-133">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="635cd-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="635cd-134">DateTimeOffset</span></span>|<span data-ttu-id="635cd-135">DateTime, an dem der übergeordnete Prozess gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="635cd-135">DateTime at which the parent process was started.</span></span> <span data-ttu-id="635cd-136">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="635cd-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="635cd-137">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="635cd-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="635cd-138">Diese Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="635cd-138">parentProcessId</span></span>|<span data-ttu-id="635cd-139">Int32</span><span class="sxs-lookup"><span data-stu-id="635cd-139">Int32</span></span>|<span data-ttu-id="635cd-140">Die Prozess-ID (PID) des übergeordneten Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="635cd-140">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="635cd-141">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="635cd-141">parentProcessName</span></span>|<span data-ttu-id="635cd-142">String</span><span class="sxs-lookup"><span data-stu-id="635cd-142">String</span></span>|<span data-ttu-id="635cd-143">Der Name der Bilddatei des übergeordneten Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="635cd-143">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="635cd-144">Pfad</span><span class="sxs-lookup"><span data-stu-id="635cd-144">path</span></span>|<span data-ttu-id="635cd-145">String</span><span class="sxs-lookup"><span data-stu-id="635cd-145">String</span></span>|<span data-ttu-id="635cd-146">Vollständiger Pfad, einschließlich Dateiname.</span><span class="sxs-lookup"><span data-stu-id="635cd-146">Full path, including filename.</span></span>|
|<span data-ttu-id="635cd-147">processId</span><span class="sxs-lookup"><span data-stu-id="635cd-147">processId</span></span>|<span data-ttu-id="635cd-148">Int32</span><span class="sxs-lookup"><span data-stu-id="635cd-148">Int32</span></span>|<span data-ttu-id="635cd-149">Die Prozess-ID (PID) des Prozesses.</span><span class="sxs-lookup"><span data-stu-id="635cd-149">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="635cd-150">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="635cd-150">JSON representation</span></span>

<span data-ttu-id="635cd-151">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="635cd-151">The following is a JSON representation of the resource.</span></span>

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
