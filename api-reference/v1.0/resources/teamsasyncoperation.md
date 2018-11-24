# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="931b7-101">Ressourcentyp teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="931b7-101">teamsAsyncOperation resource type</span></span>



<span data-ttu-id="931b7-102">Ein Microsoft-Teams, asynchroner Vorgang ist ein Vorgang, der die Lebensdauer der einzelnen API-Anforderung transcends.</span><span class="sxs-lookup"><span data-stu-id="931b7-102">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="931b7-103">Diese Vorgänge sind langer oder zu teuer, in dem Zeitrahmen ihrer ursprünglichen Anforderung abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="931b7-103">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="931b7-104">Wenn ein asynchroner Vorgang gestartet wird, gibt die Methode eine 202 akzeptierte Antwortcode zurück.</span><span class="sxs-lookup"><span data-stu-id="931b7-104">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="931b7-105">Die Antwort enthält außerdem einen Location-Header, der den Speicherort der die TeamsAsyncOperation enthält.</span><span class="sxs-lookup"><span data-stu-id="931b7-105">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="931b7-106">Überprüfen Sie regelmäßig den Status des Vorgangs, indem er eine GET-Anforderung an diesen Speicherort; Warten Sie > 30 Sekunden zwischen überprüft.</span><span class="sxs-lookup"><span data-stu-id="931b7-106">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="931b7-107">Wenn die Anforderung erfolgreich abgeschlossen wird, der Status wird werden "succeeded" und der TargetResourceLocation verweist auf die erstellte/geänderte Ressource.</span><span class="sxs-lookup"><span data-stu-id="931b7-107">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="931b7-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="931b7-108">Properties</span></span>

| <span data-ttu-id="931b7-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="931b7-109">Property</span></span> | <span data-ttu-id="931b7-110">Typ</span><span class="sxs-lookup"><span data-stu-id="931b7-110">Type</span></span>   | <span data-ttu-id="931b7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="931b7-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="931b7-112">id</span><span class="sxs-lookup"><span data-stu-id="931b7-112">id</span></span>|<span data-ttu-id="931b7-113">string</span><span class="sxs-lookup"><span data-stu-id="931b7-113">string</span></span> |<span data-ttu-id="931b7-114">Eindeutige Vorgangs-Id.</span><span class="sxs-lookup"><span data-stu-id="931b7-114">Unique operation id.</span></span>|
|<span data-ttu-id="931b7-115">Vorgangstyp</span><span class="sxs-lookup"><span data-stu-id="931b7-115">operationType</span></span>|[<span data-ttu-id="931b7-116">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="931b7-116">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="931b7-117">Gibt an, welche Art von Vorgang beschrieben wird.</span><span class="sxs-lookup"><span data-stu-id="931b7-117">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="931b7-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="931b7-118">createdDateTime</span></span>|<span data-ttu-id="931b7-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="931b7-119">DateTimeOffset</span></span> |<span data-ttu-id="931b7-120">Die Uhrzeit der Erstellung des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="931b7-120">Time when the operation was created.</span></span>|
|<span data-ttu-id="931b7-121">status</span><span class="sxs-lookup"><span data-stu-id="931b7-121">status</span></span>|[<span data-ttu-id="931b7-122">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="931b7-122">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="931b7-123">Ausführungsstatus.</span><span class="sxs-lookup"><span data-stu-id="931b7-123">Operation status.</span></span>|
|<span data-ttu-id="931b7-124">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="931b7-124">lastActionDateTime</span></span>|<span data-ttu-id="931b7-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="931b7-125">DateTimeOffset</span></span> |<span data-ttu-id="931b7-126">Zeitpunkt, wann die asynchrone Operation zuletzt aktualisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="931b7-126">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="931b7-127">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="931b7-127">attemptsCount</span></span>|<span data-ttu-id="931b7-128">Int32</span><span class="sxs-lookup"><span data-stu-id="931b7-128">Int32</span></span>|<span data-ttu-id="931b7-129">Anzahl der Häufigkeit, mit die der Vorgang versucht wurde, vor der erfolgreichen oder fehlgeschlagenen markiert werden.</span><span class="sxs-lookup"><span data-stu-id="931b7-129">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="931b7-130">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="931b7-130">targetResourceId</span></span>|<span data-ttu-id="931b7-131">GUID</span><span class="sxs-lookup"><span data-stu-id="931b7-131">guid</span></span> |<span data-ttu-id="931b7-132">Die ID des Objekts, das erstellt oder aufgrund dieses asynchronen Vorgangs, in der Regel ein [Team](../resources/team.md)geändert hat.</span><span class="sxs-lookup"><span data-stu-id="931b7-132">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="931b7-133">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="931b7-133">targetResourceLocation</span></span>|<span data-ttu-id="931b7-134">string</span><span class="sxs-lookup"><span data-stu-id="931b7-134">string</span></span>|<span data-ttu-id="931b7-135">Die Position des Objekts, das erstellt oder aufgrund dieses asynchronen Vorgangs geändert hat.</span><span class="sxs-lookup"><span data-stu-id="931b7-135">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="931b7-136">Diese URL sollte als ein nicht transparenter Wert behandelt und nicht in ihre Pfadkomponenten analysiert werden.</span><span class="sxs-lookup"><span data-stu-id="931b7-136">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="931b7-137">error</span><span class="sxs-lookup"><span data-stu-id="931b7-137">error</span></span>|[<span data-ttu-id="931b7-138">operationError</span><span class="sxs-lookup"><span data-stu-id="931b7-138">operationError</span></span>](operationerror.md)|<span data-ttu-id="931b7-139">Alle Fehler, die bewirkt, dass die asynchrone Operation ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="931b7-139">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="931b7-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="931b7-140">JSON representation</span></span>

<span data-ttu-id="931b7-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="931b7-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsasyncoperation"
}-->

```json
{
    "id": "string",
    "operationType": "archiveTeam",
    "createdDateTime": "2018-01-01T00:00:00.0000000Z",
    "status": "succeeded",
    "lastActionDateTime": "2018-01-01T00:00:00.0000000Z",
    "attemptsCount": 1,
    "targetResourceId": "fa4aa5a2-a75b-4769-86f4-9e2742a18fda",
    "targetResourceLocation": "/groups('fa4aa5a2-a75b-4769-86f4-9e2742a18fda')/team",
    "error": null
}
```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
