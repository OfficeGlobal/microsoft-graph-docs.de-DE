---
title: Ressourcentyp teamsAsyncOperation
description: 'Ein Microsoft-Teams, asynchroner Vorgang ist ein Vorgang, der die Lebensdauer der einzelnen API-Anforderung transcends. '
author: nkramer
ms.openlocfilehash: fd64f99c20505a8e670c865faa039e9db3174ed6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320608"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="581c7-103">Ressourcentyp teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="581c7-103">teamsAsyncOperation resource type</span></span>



<span data-ttu-id="581c7-104">Ein Microsoft-Teams, asynchroner Vorgang ist ein Vorgang, der die Lebensdauer der einzelnen API-Anforderung transcends.</span><span class="sxs-lookup"><span data-stu-id="581c7-104">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="581c7-105">Diese Vorgänge sind langer oder zu teuer, in dem Zeitrahmen ihrer ursprünglichen Anforderung abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="581c7-105">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="581c7-106">Wenn ein asynchroner Vorgang gestartet wird, gibt die Methode eine 202 akzeptierte Antwortcode zurück.</span><span class="sxs-lookup"><span data-stu-id="581c7-106">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="581c7-107">Die Antwort enthält außerdem einen Location-Header, der den Speicherort der die TeamsAsyncOperation enthält.</span><span class="sxs-lookup"><span data-stu-id="581c7-107">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="581c7-108">Überprüfen Sie regelmäßig den Status des Vorgangs, indem er eine GET-Anforderung an diesen Speicherort; Warten Sie > 30 Sekunden zwischen überprüft.</span><span class="sxs-lookup"><span data-stu-id="581c7-108">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="581c7-109">Wenn die Anforderung erfolgreich abgeschlossen wird, der Status wird werden "succeeded" und der TargetResourceLocation verweist auf die erstellte/geänderte Ressource.</span><span class="sxs-lookup"><span data-stu-id="581c7-109">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="581c7-110">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="581c7-110">Properties</span></span>

| <span data-ttu-id="581c7-111">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="581c7-111">Property</span></span> | <span data-ttu-id="581c7-112">Typ</span><span class="sxs-lookup"><span data-stu-id="581c7-112">Type</span></span>   | <span data-ttu-id="581c7-113">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="581c7-113">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="581c7-114">id</span><span class="sxs-lookup"><span data-stu-id="581c7-114">id</span></span>|<span data-ttu-id="581c7-115">string</span><span class="sxs-lookup"><span data-stu-id="581c7-115">string</span></span> |<span data-ttu-id="581c7-116">Eindeutige Vorgangs-Id.</span><span class="sxs-lookup"><span data-stu-id="581c7-116">Unique operation id.</span></span>|
|<span data-ttu-id="581c7-117">Vorgangstyp</span><span class="sxs-lookup"><span data-stu-id="581c7-117">operationType</span></span>|[<span data-ttu-id="581c7-118">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="581c7-118">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="581c7-119">Gibt an, welche Art von Vorgang beschrieben wird.</span><span class="sxs-lookup"><span data-stu-id="581c7-119">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="581c7-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="581c7-120">createdDateTime</span></span>|<span data-ttu-id="581c7-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="581c7-121">DateTimeOffset</span></span> |<span data-ttu-id="581c7-122">Die Uhrzeit der Erstellung des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="581c7-122">Time when the operation was created.</span></span>|
|<span data-ttu-id="581c7-123">status</span><span class="sxs-lookup"><span data-stu-id="581c7-123">status</span></span>|[<span data-ttu-id="581c7-124">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="581c7-124">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="581c7-125">Ausführungsstatus.</span><span class="sxs-lookup"><span data-stu-id="581c7-125">Operation status.</span></span>|
|<span data-ttu-id="581c7-126">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="581c7-126">lastActionDateTime</span></span>|<span data-ttu-id="581c7-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="581c7-127">DateTimeOffset</span></span> |<span data-ttu-id="581c7-128">Zeitpunkt, wann die asynchrone Operation zuletzt aktualisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="581c7-128">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="581c7-129">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="581c7-129">attemptsCount</span></span>|<span data-ttu-id="581c7-130">Int32</span><span class="sxs-lookup"><span data-stu-id="581c7-130">Int32</span></span>|<span data-ttu-id="581c7-131">Anzahl der Häufigkeit, mit die der Vorgang versucht wurde, vor der erfolgreichen oder fehlgeschlagenen markiert werden.</span><span class="sxs-lookup"><span data-stu-id="581c7-131">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="581c7-132">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="581c7-132">targetResourceId</span></span>|<span data-ttu-id="581c7-133">GUID</span><span class="sxs-lookup"><span data-stu-id="581c7-133">guid</span></span> |<span data-ttu-id="581c7-134">Die ID des Objekts, das erstellt oder aufgrund dieses asynchronen Vorgangs, in der Regel ein [Team](../resources/team.md)geändert hat.</span><span class="sxs-lookup"><span data-stu-id="581c7-134">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="581c7-135">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="581c7-135">targetResourceLocation</span></span>|<span data-ttu-id="581c7-136">string</span><span class="sxs-lookup"><span data-stu-id="581c7-136">string</span></span>|<span data-ttu-id="581c7-137">Die Position des Objekts, das erstellt oder aufgrund dieses asynchronen Vorgangs geändert hat.</span><span class="sxs-lookup"><span data-stu-id="581c7-137">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="581c7-138">Diese URL sollte als ein nicht transparenter Wert behandelt und nicht in ihre Pfadkomponenten analysiert werden.</span><span class="sxs-lookup"><span data-stu-id="581c7-138">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="581c7-139">error</span><span class="sxs-lookup"><span data-stu-id="581c7-139">error</span></span>|[<span data-ttu-id="581c7-140">operationError</span><span class="sxs-lookup"><span data-stu-id="581c7-140">operationError</span></span>](operationerror.md)|<span data-ttu-id="581c7-141">Alle Fehler, die bewirkt, dass die asynchrone Operation ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="581c7-141">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="581c7-142">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="581c7-142">JSON representation</span></span>

<span data-ttu-id="581c7-143">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="581c7-143">The following is a JSON representation of the resource.</span></span>

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
