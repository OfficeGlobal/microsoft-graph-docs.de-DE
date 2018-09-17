# <a name="process-resource-type"></a><span data-ttu-id="24b2c-101">Ressourcentyp process</span><span class="sxs-lookup"><span data-stu-id="24b2c-101">process resource type</span></span>

<span data-ttu-id="24b2c-102">Enthält Zustandsinformationen über den Vorgang im Zusammenhang mit der Warnung.</span><span class="sxs-lookup"><span data-stu-id="24b2c-102">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="24b2c-103">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="24b2c-103">Properties</span></span>

| <span data-ttu-id="24b2c-104">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="24b2c-104">Property</span></span>   | <span data-ttu-id="24b2c-105">Typ</span><span class="sxs-lookup"><span data-stu-id="24b2c-105">Type</span></span>|<span data-ttu-id="24b2c-106">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24b2c-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24b2c-107">accountName</span><span class="sxs-lookup"><span data-stu-id="24b2c-107">accountName</span></span>|<span data-ttu-id="24b2c-108">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="24b2c-108">String</span></span>|<span data-ttu-id="24b2c-109">Benutzerkontobezeichner (Benutzerkonto-Kontext, unter dem der Prozess gelaufen ist), z.B. AccountName, SID, etc.</span><span class="sxs-lookup"><span data-stu-id="24b2c-109">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="24b2c-110">commandLine</span><span class="sxs-lookup"><span data-stu-id="24b2c-110">commandLine</span></span>|<span data-ttu-id="24b2c-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="24b2c-111">String</span></span>|<span data-ttu-id="24b2c-112">Vollständiger Prozess-Aufruf-Eingabezeile einschließlich aller Parameter.</span><span class="sxs-lookup"><span data-stu-id="24b2c-112">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="24b2c-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24b2c-113">createdDateTime</span></span>|<span data-ttu-id="24b2c-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24b2c-114">DateTimeOffset</span></span>|<span data-ttu-id="24b2c-115">Zeitpunkt, an dem der Prozess gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="24b2c-115">Time at which the process was started.</span></span> <span data-ttu-id="24b2c-116">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="24b2c-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="24b2c-117">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="24b2c-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="24b2c-118">fileHash</span><span class="sxs-lookup"><span data-stu-id="24b2c-118">fileHash</span></span>|[<span data-ttu-id="24b2c-119">fileHash</span><span class="sxs-lookup"><span data-stu-id="24b2c-119">fileHash</span></span>](filehash.md)|<span data-ttu-id="24b2c-120">Komplexer Typ mit Datei-Hashes (kryptographisch und der ortsabhängig).</span><span class="sxs-lookup"><span data-stu-id="24b2c-120">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="24b2c-121">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="24b2c-121">integrityLevel</span></span>|<span data-ttu-id="24b2c-122">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="24b2c-122">processIntegrityLevel</span></span>|<span data-ttu-id="24b2c-123">Die Integritätsebene des Prozesses.</span><span class="sxs-lookup"><span data-stu-id="24b2c-123">The integrity level of the process.</span></span> <span data-ttu-id="24b2c-124">Mögliche Werte sind: `unknown`, `untrusted`, `low`, `medium`, `high` und `system`.</span><span class="sxs-lookup"><span data-stu-id="24b2c-124">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="24b2c-125">isElevated</span><span class="sxs-lookup"><span data-stu-id="24b2c-125">isElevated</span></span>|<span data-ttu-id="24b2c-126">Boolesch</span><span class="sxs-lookup"><span data-stu-id="24b2c-126">Boolean</span></span>|<span data-ttu-id="24b2c-127">True, wenn der Prozess erhöht ist.</span><span class="sxs-lookup"><span data-stu-id="24b2c-127">True if the process is elevated.</span></span>|
|<span data-ttu-id="24b2c-128">Name</span><span class="sxs-lookup"><span data-stu-id="24b2c-128">name</span></span>|<span data-ttu-id="24b2c-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="24b2c-129">String</span></span>|<span data-ttu-id="24b2c-130">Der Name der Bilddatei des Prozesses.</span><span class="sxs-lookup"><span data-stu-id="24b2c-130">The name of the process' Image file.</span></span>|
|<span data-ttu-id="24b2c-131">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="24b2c-131">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="24b2c-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24b2c-132">DateTimeOffset</span></span>|<span data-ttu-id="24b2c-133">DateTime, an dem der übergeordnete Prozess gestartet wurde.</span><span class="sxs-lookup"><span data-stu-id="24b2c-133">DateTime at which the parent process was started.</span></span> <span data-ttu-id="24b2c-134">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="24b2c-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="24b2c-135">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="24b2c-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="24b2c-136">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="24b2c-136">parentProcessId</span></span>|<span data-ttu-id="24b2c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="24b2c-137">Int32</span></span>|<span data-ttu-id="24b2c-138">Die Prozess-ID (PID) des übergeordneten Prozesses.</span><span class="sxs-lookup"><span data-stu-id="24b2c-138">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="24b2c-139">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="24b2c-139">parentProcessName</span></span>|<span data-ttu-id="24b2c-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="24b2c-140">String</span></span>|<span data-ttu-id="24b2c-141">Der Name der Bilddatei des übergeordneten Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="24b2c-141">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="24b2c-142">Pfad</span><span class="sxs-lookup"><span data-stu-id="24b2c-142">path</span></span>|<span data-ttu-id="24b2c-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="24b2c-143">String</span></span>|<span data-ttu-id="24b2c-144">Vollständiger Pfad, einschließlich Dateiname.</span><span class="sxs-lookup"><span data-stu-id="24b2c-144">Full path, including filename.</span></span>|
|<span data-ttu-id="24b2c-145">processId</span><span class="sxs-lookup"><span data-stu-id="24b2c-145">processId</span></span>|<span data-ttu-id="24b2c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="24b2c-146">Int32</span></span>|<span data-ttu-id="24b2c-147">Die Prozess-ID (PID) des übergeordneten Prozesses.</span><span class="sxs-lookup"><span data-stu-id="24b2c-147">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24b2c-148">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="24b2c-148">JSON representation</span></span>

<span data-ttu-id="24b2c-149">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="24b2c-149">The following is a JSON representation of the resource.</span></span>

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