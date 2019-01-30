# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="d4936-101">Ressourcentyp dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="d4936-101">dataPolicyOperation resource type</span></span>

<span data-ttu-id="d4936-102">Stellt einen gesendete Daten Richtlinie Vorgang dar.</span><span class="sxs-lookup"><span data-stu-id="d4936-102">Represents a submitted data policy operation.</span></span> <span data-ttu-id="d4936-103">Sie enthält die erforderlichen Informationen für das Nachverfolgen des Status eines Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="d4936-103">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="d4936-104">Beispielsweise kann ein Unternehmensadministrator anfordern, Daten Richtlinie Vorgang zum Exportieren eines Mitarbeiters Unternehmensdaten verwendet, und klicken Sie dann die Anforderung später verfolgen.</span><span class="sxs-lookup"><span data-stu-id="d4936-104">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="d4936-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="d4936-105">Methods</span></span>

| <span data-ttu-id="d4936-106">Methode</span><span class="sxs-lookup"><span data-stu-id="d4936-106">Method</span></span>           | <span data-ttu-id="d4936-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d4936-107">Return Type</span></span>    |<span data-ttu-id="d4936-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4936-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d4936-109">Abrufen von dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="d4936-109">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="d4936-110">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="d4936-110">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="d4936-111">Rufen Sie die Eigenschaften des **DataPolicyOperation** -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="d4936-111">Retrieve properties of the **dataPolicyOperation** object.</span></span>|
|[<span data-ttu-id="d4936-112">Exportieren von persönlichen Daten</span><span class="sxs-lookup"><span data-stu-id="d4936-112">Export personal data</span></span>](../api/user-exportpersonaldata.md) | <span data-ttu-id="d4936-113">Keine</span><span class="sxs-lookup"><span data-stu-id="d4936-113">None</span></span> |<span data-ttu-id="d4936-114">Fordern Sie Daten Richtlinie Vorgang zur Organisationseinheit Benutzerdaten exportieren, die später mithilfe [DataPolicyOperation](../api/datapolicyoperation-get.md) wiedergegeben werden können</span><span class="sxs-lookup"><span data-stu-id="d4936-114">Submit a data policy operation request to export organizational user's data which can later be read using [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span></span>|

## <a name="properties"></a><span data-ttu-id="d4936-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d4936-115">Properties</span></span>

> <span data-ttu-id="d4936-116">**Hinweis:** Alle Eigenschaften dieser Ressource sind schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d4936-116">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="d4936-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4936-117">Property</span></span>     | <span data-ttu-id="d4936-118">Typ</span><span class="sxs-lookup"><span data-stu-id="d4936-118">Type</span></span>   |<span data-ttu-id="d4936-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4936-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4936-120">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4936-120">completedDateTime</span></span>|<span data-ttu-id="d4936-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4936-121">DateTimeOffset</span></span>|<span data-ttu-id="d4936-122">Stellt die bei die Anforderung für diese Richtlinie Datenvorgangs, in UTC-Zeit mit abgeschlossen wurde im ISO 8601-Format.</span><span class="sxs-lookup"><span data-stu-id="d4936-122">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="d4936-123">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d4936-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d4936-124">"NULL", bis der Vorgang abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="d4936-124">Null until the operation completes.</span></span>|
|<span data-ttu-id="d4936-125">id</span><span class="sxs-lookup"><span data-stu-id="d4936-125">id</span></span>|<span data-ttu-id="d4936-126">String</span><span class="sxs-lookup"><span data-stu-id="d4936-126">String</span></span>| <span data-ttu-id="d4936-127">Eindeutiger Schlüssel für diesen Vorgang.</span><span class="sxs-lookup"><span data-stu-id="d4936-127">Unique key for this operation.</span></span> |
|<span data-ttu-id="d4936-128">status</span><span class="sxs-lookup"><span data-stu-id="d4936-128">status</span></span>|<span data-ttu-id="d4936-129">string</span><span class="sxs-lookup"><span data-stu-id="d4936-129">string</span></span>| <span data-ttu-id="d4936-130">Mögliche Werte: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d4936-130">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d4936-131">storageLocation</span><span class="sxs-lookup"><span data-stu-id="d4936-131">storageLocation</span></span>|<span data-ttu-id="d4936-132">String</span><span class="sxs-lookup"><span data-stu-id="d4936-132">String</span></span>|<span data-ttu-id="d4936-133">Der URL-Adresse an, in dem Daten für exportanforderungen exportiert werden.</span><span class="sxs-lookup"><span data-stu-id="d4936-133">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="d4936-134">userId</span><span class="sxs-lookup"><span data-stu-id="d4936-134">userId</span></span>|<span data-ttu-id="d4936-135">String</span><span class="sxs-lookup"><span data-stu-id="d4936-135">String</span></span>|<span data-ttu-id="d4936-136">Die Id für den Benutzer, auf dem die Operation ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="d4936-136">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="d4936-137">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4936-137">submittedDateTime</span></span>|<span data-ttu-id="d4936-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4936-138">DateTimeOffset</span></span>|<span data-ttu-id="d4936-139">Stellt die bei die Anforderung für diesen Datenvorgang im ISO 8601-Format verwenden übermittelt wurde, im UTC-Zeit.</span><span class="sxs-lookup"><span data-stu-id="d4936-139">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="d4936-140">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d4936-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d4936-141">progress</span><span class="sxs-lookup"><span data-stu-id="d4936-141">progress</span></span>|<span data-ttu-id="d4936-142">String</span><span class="sxs-lookup"><span data-stu-id="d4936-142">String</span></span>|<span data-ttu-id="d4936-143">Gibt den Fortschritt eines Vorgangs an.</span><span class="sxs-lookup"><span data-stu-id="d4936-143">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4936-144">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d4936-144">Relationships</span></span>
<span data-ttu-id="d4936-145">Keine.</span><span class="sxs-lookup"><span data-stu-id="d4936-145">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d4936-146">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d4936-146">JSON representation</span></span>

<span data-ttu-id="d4936-147">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d4936-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}-->

```json
{
  "completedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "status": "string",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)", 
  "progress": "String (double)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dataPolicyOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
