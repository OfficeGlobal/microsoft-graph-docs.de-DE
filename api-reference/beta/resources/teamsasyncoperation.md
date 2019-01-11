---
title: Ressourcentyp teamsAsyncOperation
description: 'Ein Microsoft-Teams, asynchroner Vorgang ist ein Vorgang, der die Lebensdauer der einzelnen API-Anforderung transcends. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 20a616d3c09337b96c50cc008e4f56021c61e593
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885575"
---
# <a name="teamsasyncoperation-resource-type"></a><span data-ttu-id="05eb5-103">Ressourcentyp teamsAsyncOperation</span><span class="sxs-lookup"><span data-stu-id="05eb5-103">teamsAsyncOperation resource type</span></span>

> <span data-ttu-id="05eb5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="05eb5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05eb5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="05eb5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="05eb5-106">Ein Microsoft-Teams, asynchroner Vorgang ist ein Vorgang, der die Lebensdauer der einzelnen API-Anforderung transcends.</span><span class="sxs-lookup"><span data-stu-id="05eb5-106">A Microsoft Teams async operation is an operation that transcends the lifetime of a single API request.</span></span> <span data-ttu-id="05eb5-107">Diese Vorgänge sind langer oder zu teuer, in dem Zeitrahmen ihrer ursprünglichen Anforderung abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="05eb5-107">These operations are long-running or too expensive to complete within the timeframe of their originating request.</span></span>

<span data-ttu-id="05eb5-108">Wenn ein asynchroner Vorgang gestartet wird, gibt die Methode eine 202 akzeptierte Antwortcode zurück.</span><span class="sxs-lookup"><span data-stu-id="05eb5-108">When an async operation is initiated, the method returns a 202 Accepted response code.</span></span> <span data-ttu-id="05eb5-109">Die Antwort enthält außerdem einen Location-Header, der den Speicherort der die TeamsAsyncOperation enthält.</span><span class="sxs-lookup"><span data-stu-id="05eb5-109">The response will also contain a Location header, which contains the location of the teamsAsyncOperation.</span></span> <span data-ttu-id="05eb5-110">Überprüfen Sie regelmäßig den Status des Vorgangs, indem er eine GET-Anforderung an diesen Speicherort; Warten Sie > 30 Sekunden zwischen überprüft.</span><span class="sxs-lookup"><span data-stu-id="05eb5-110">Periodically check the status of the operation by making a GET request to this location; wait >30 seconds between checks.</span></span>
<span data-ttu-id="05eb5-111">Wenn die Anforderung erfolgreich abgeschlossen wird, der Status wird werden "succeeded" und der TargetResourceLocation verweist auf die erstellte/geänderte Ressource.</span><span class="sxs-lookup"><span data-stu-id="05eb5-111">When the request completes successfully, the status will be "succeeded" and the targetResourceLocation will point to the created/modified resource.</span></span>

## <a name="properties"></a><span data-ttu-id="05eb5-112">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="05eb5-112">Properties</span></span>

| <span data-ttu-id="05eb5-113">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="05eb5-113">Property</span></span> | <span data-ttu-id="05eb5-114">Typ</span><span class="sxs-lookup"><span data-stu-id="05eb5-114">Type</span></span>   | <span data-ttu-id="05eb5-115">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="05eb5-115">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="05eb5-116">id</span><span class="sxs-lookup"><span data-stu-id="05eb5-116">id</span></span>|<span data-ttu-id="05eb5-117">string</span><span class="sxs-lookup"><span data-stu-id="05eb5-117">string</span></span> |<span data-ttu-id="05eb5-118">Eindeutige Vorgangs-Id.</span><span class="sxs-lookup"><span data-stu-id="05eb5-118">Unique operation id.</span></span>|
|<span data-ttu-id="05eb5-119">Vorgangstyp</span><span class="sxs-lookup"><span data-stu-id="05eb5-119">operationType</span></span>|[<span data-ttu-id="05eb5-120">teamsAsyncOperationType</span><span class="sxs-lookup"><span data-stu-id="05eb5-120">teamsAsyncOperationType</span></span>](teamsasyncoperationtype.md) |<span data-ttu-id="05eb5-121">Gibt an, welche Art von Vorgang beschrieben wird.</span><span class="sxs-lookup"><span data-stu-id="05eb5-121">Denotes which type of operation is being described.</span></span>|
|<span data-ttu-id="05eb5-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="05eb5-122">createdDateTime</span></span>|<span data-ttu-id="05eb5-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05eb5-123">DateTimeOffset</span></span> |<span data-ttu-id="05eb5-124">Die Uhrzeit der Erstellung des Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="05eb5-124">Time when the operation was created.</span></span>|
|<span data-ttu-id="05eb5-125">status</span><span class="sxs-lookup"><span data-stu-id="05eb5-125">status</span></span>|[<span data-ttu-id="05eb5-126">teamsAsyncOperationStatus</span><span class="sxs-lookup"><span data-stu-id="05eb5-126">teamsAsyncOperationStatus</span></span>](teamsasyncoperationstatus.md)| <span data-ttu-id="05eb5-127">Ausführungsstatus.</span><span class="sxs-lookup"><span data-stu-id="05eb5-127">Operation status.</span></span>|
|<span data-ttu-id="05eb5-128">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="05eb5-128">lastActionDateTime</span></span>|<span data-ttu-id="05eb5-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05eb5-129">DateTimeOffset</span></span> |<span data-ttu-id="05eb5-130">Zeitpunkt, wann die asynchrone Operation zuletzt aktualisiert wurde.</span><span class="sxs-lookup"><span data-stu-id="05eb5-130">Time when the async operation was last updated.</span></span>|
|<span data-ttu-id="05eb5-131">attemptsCount</span><span class="sxs-lookup"><span data-stu-id="05eb5-131">attemptsCount</span></span>|<span data-ttu-id="05eb5-132">Int32</span><span class="sxs-lookup"><span data-stu-id="05eb5-132">Int32</span></span>|<span data-ttu-id="05eb5-133">Anzahl der Häufigkeit, mit die der Vorgang versucht wurde, vor der erfolgreichen oder fehlgeschlagenen markiert werden.</span><span class="sxs-lookup"><span data-stu-id="05eb5-133">Number of times the operation was attempted before being marked successful or failed.</span></span>|
|<span data-ttu-id="05eb5-134">targetResourceId</span><span class="sxs-lookup"><span data-stu-id="05eb5-134">targetResourceId</span></span>|<span data-ttu-id="05eb5-135">GUID</span><span class="sxs-lookup"><span data-stu-id="05eb5-135">guid</span></span> |<span data-ttu-id="05eb5-136">Die ID des Objekts, das erstellt oder aufgrund dieses asynchronen Vorgangs, in der Regel ein [Team](../resources/team.md)geändert hat.</span><span class="sxs-lookup"><span data-stu-id="05eb5-136">The ID of the object that's created or modified as result of this async operation, typically a [team](../resources/team.md).</span></span>|
|<span data-ttu-id="05eb5-137">targetResourceLocation</span><span class="sxs-lookup"><span data-stu-id="05eb5-137">targetResourceLocation</span></span>|<span data-ttu-id="05eb5-138">string</span><span class="sxs-lookup"><span data-stu-id="05eb5-138">string</span></span>|<span data-ttu-id="05eb5-139">Die Position des Objekts, das erstellt oder aufgrund dieses asynchronen Vorgangs geändert hat.</span><span class="sxs-lookup"><span data-stu-id="05eb5-139">The location of the object that's created or modified as result of this async operation.</span></span> <span data-ttu-id="05eb5-140">Diese URL sollte als ein nicht transparenter Wert behandelt und nicht in ihre Pfadkomponenten analysiert werden.</span><span class="sxs-lookup"><span data-stu-id="05eb5-140">This URL should be treated as an opaque value and not parsed into its component paths.</span></span>|
|<span data-ttu-id="05eb5-141">error</span><span class="sxs-lookup"><span data-stu-id="05eb5-141">error</span></span>|[<span data-ttu-id="05eb5-142">operationError</span><span class="sxs-lookup"><span data-stu-id="05eb5-142">operationError</span></span>](operationerror.md)|<span data-ttu-id="05eb5-143">Alle Fehler, die bewirkt, dass die asynchrone Operation ein Fehler auftritt.</span><span class="sxs-lookup"><span data-stu-id="05eb5-143">Any error that causes the async operation to fail.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="05eb5-144">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="05eb5-144">JSON representation</span></span>

<span data-ttu-id="05eb5-145">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="05eb5-145">The following is a JSON representation of the resource.</span></span>

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
