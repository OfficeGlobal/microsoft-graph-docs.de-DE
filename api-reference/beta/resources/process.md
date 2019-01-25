---
title: Prozess Ressourcentyp
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
ms.openlocfilehash: 13de9a2485aeeaa06fdad3c7cce3eb1f81374193
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521208"
---
# <a name="process-resource-type"></a><span data-ttu-id="8f27d-104">Prozess Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8f27d-104">process resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f27d-105">Statusinformationen über den Prozess im Zusammenhang mit der Benachrichtigung enthält.</span><span class="sxs-lookup"><span data-stu-id="8f27d-105">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="8f27d-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8f27d-106">Properties</span></span>

| <span data-ttu-id="8f27d-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8f27d-107">Property</span></span>   | <span data-ttu-id="8f27d-108">Typ</span><span class="sxs-lookup"><span data-stu-id="8f27d-108">Type</span></span>|<span data-ttu-id="8f27d-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8f27d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f27d-110">accountName</span><span class="sxs-lookup"><span data-stu-id="8f27d-110">accountName</span></span>|<span data-ttu-id="8f27d-111">String</span><span class="sxs-lookup"><span data-stu-id="8f27d-111">String</span></span>|<span data-ttu-id="8f27d-112">Benutzerkonto für Beispiel, Kontoname, SID und So weiter Bezeichner (Konto Benutzerkontext, unter dem Prozess steht).</span><span class="sxs-lookup"><span data-stu-id="8f27d-112">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="8f27d-113">commandLine</span><span class="sxs-lookup"><span data-stu-id="8f27d-113">commandLine</span></span>|<span data-ttu-id="8f27d-114">String</span><span class="sxs-lookup"><span data-stu-id="8f27d-114">String</span></span>|<span data-ttu-id="8f27d-115">Vollständiger Prozess Aufruf Commandline einschließlich aller Parameter.</span><span class="sxs-lookup"><span data-stu-id="8f27d-115">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="8f27d-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f27d-116">createdDateTime</span></span>|<span data-ttu-id="8f27d-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f27d-117">DateTimeOffset</span></span>|<span data-ttu-id="8f27d-118">Zeitpunkt, an dem der Prozess gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="8f27d-118">Time at which the process was started.</span></span> <span data-ttu-id="8f27d-119">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="8f27d-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8f27d-120">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8f27d-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8f27d-121">fileHash</span><span class="sxs-lookup"><span data-stu-id="8f27d-121">fileHash</span></span>|[<span data-ttu-id="8f27d-122">fileHash</span><span class="sxs-lookup"><span data-stu-id="8f27d-122">fileHash</span></span>](filehash.md)|<span data-ttu-id="8f27d-123">Komplexer Typ mit Dateihashes (cryptographic und der Speicherort).</span><span class="sxs-lookup"><span data-stu-id="8f27d-123">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="8f27d-124">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="8f27d-124">integrityLevel</span></span>|<span data-ttu-id="8f27d-125">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="8f27d-125">processIntegrityLevel</span></span>|<span data-ttu-id="8f27d-126">Die Integritätsebene des Prozesses.</span><span class="sxs-lookup"><span data-stu-id="8f27d-126">The integrity level of the process.</span></span> <span data-ttu-id="8f27d-127">Mögliche Werte sind: `unknown`, `untrusted`, `low`, `medium`, `high` und `system`.</span><span class="sxs-lookup"><span data-stu-id="8f27d-127">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="8f27d-128">isElevated</span><span class="sxs-lookup"><span data-stu-id="8f27d-128">isElevated</span></span>|<span data-ttu-id="8f27d-129">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8f27d-129">Boolean</span></span>|<span data-ttu-id="8f27d-130">True, wenn der Prozess erweitert wird.</span><span class="sxs-lookup"><span data-stu-id="8f27d-130">True if the process is elevated.</span></span>|
|<span data-ttu-id="8f27d-131">name</span><span class="sxs-lookup"><span data-stu-id="8f27d-131">name</span></span>|<span data-ttu-id="8f27d-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8f27d-132">String</span></span>|<span data-ttu-id="8f27d-133">Der Name der Bilddatei des Prozesses.</span><span class="sxs-lookup"><span data-stu-id="8f27d-133">The name of the process' Image file.</span></span>|
|<span data-ttu-id="8f27d-134">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f27d-134">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="8f27d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f27d-135">DateTimeOffset</span></span>|<span data-ttu-id="8f27d-136">DateTime, an dem der übergeordnete Prozess gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="8f27d-136">DateTime at which the parent process was started.</span></span> <span data-ttu-id="8f27d-137">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="8f27d-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8f27d-138">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8f27d-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8f27d-139">Diese Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8f27d-139">parentProcessId</span></span>|<span data-ttu-id="8f27d-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8f27d-140">Int32</span></span>|<span data-ttu-id="8f27d-141">Die Prozess-ID (PID) des übergeordneten Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="8f27d-141">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="8f27d-142">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="8f27d-142">parentProcessName</span></span>|<span data-ttu-id="8f27d-143">String</span><span class="sxs-lookup"><span data-stu-id="8f27d-143">String</span></span>|<span data-ttu-id="8f27d-144">Der Name der Bilddatei des übergeordneten Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="8f27d-144">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="8f27d-145">Pfad</span><span class="sxs-lookup"><span data-stu-id="8f27d-145">path</span></span>|<span data-ttu-id="8f27d-146">String</span><span class="sxs-lookup"><span data-stu-id="8f27d-146">String</span></span>|<span data-ttu-id="8f27d-147">Vollständiger Pfad, einschließlich Dateiname.</span><span class="sxs-lookup"><span data-stu-id="8f27d-147">Full path, including filename.</span></span>|
|<span data-ttu-id="8f27d-148">processId</span><span class="sxs-lookup"><span data-stu-id="8f27d-148">processId</span></span>|<span data-ttu-id="8f27d-149">Int32</span><span class="sxs-lookup"><span data-stu-id="8f27d-149">Int32</span></span>|<span data-ttu-id="8f27d-150">Die Prozess-ID (PID) des Prozesses.</span><span class="sxs-lookup"><span data-stu-id="8f27d-150">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f27d-151">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8f27d-151">JSON representation</span></span>

<span data-ttu-id="8f27d-152">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8f27d-152">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/process.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
