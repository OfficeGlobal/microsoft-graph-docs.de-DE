---
title: Ressourcentyp synchronizationQuarantine
description: Enthält Informationen zu den Quarantäne Status einer SynchronizationJob.
ms.openlocfilehash: b29da9644968ffe17abb02010f8aa5c304ca7905
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058940"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="80c78-103">Ressourcentyp synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="80c78-103">synchronizationQuarantine resource type</span></span>

> <span data-ttu-id="80c78-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="80c78-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80c78-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="80c78-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="80c78-106">Enthält Informationen zu den Quarantäne Status einer [SynchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="80c78-106">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="80c78-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="80c78-107">Properties</span></span>
| <span data-ttu-id="80c78-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="80c78-108">Property</span></span>     | <span data-ttu-id="80c78-109">Typ</span><span class="sxs-lookup"><span data-stu-id="80c78-109">Type</span></span>   |<span data-ttu-id="80c78-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80c78-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80c78-111">currentBegan</span><span class="sxs-lookup"><span data-stu-id="80c78-111">currentBegan</span></span>|<span data-ttu-id="80c78-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80c78-112">DateTimeOffset</span></span>|<span data-ttu-id="80c78-113">Datum und Uhrzeit, wann die Quarantäne letzten, ausgewertet und eingeführt.</span><span class="sxs-lookup"><span data-stu-id="80c78-113">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="80c78-114">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="80c78-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="80c78-115">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="80c78-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="80c78-116">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="80c78-116">nextAttempt</span></span>|<span data-ttu-id="80c78-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80c78-117">DateTimeOffset</span></span>|<span data-ttu-id="80c78-118">Datum und Uhrzeit beim nächste Versuch die Quarantäne für die Überprüfung erfolgt.</span><span class="sxs-lookup"><span data-stu-id="80c78-118">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="80c78-119">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="80c78-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="80c78-120">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="80c78-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="80c78-121">Grund</span><span class="sxs-lookup"><span data-stu-id="80c78-121">reason</span></span>|<span data-ttu-id="80c78-122">String</span><span class="sxs-lookup"><span data-stu-id="80c78-122">String</span></span>|<span data-ttu-id="80c78-123">Ein Code, der angibt, warum die Quarantäne eingeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="80c78-123">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="80c78-124">Mögliche Werte sind: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException` und `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="80c78-124">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span></span>|
|<span data-ttu-id="80c78-125">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="80c78-125">seriesBegan</span></span>|<span data-ttu-id="80c78-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80c78-126">DateTimeOffset</span></span>|<span data-ttu-id="80c78-127">Datum und Uhrzeit, als die Quarantäne zunächst, in dieser Reihe (eine Datenreihe beginnt eingeführt wurde, wenn eine Quarantäne wird zuerst eingeführt und wird zurückgesetzt, sobald die Quarantäne transformiert ist).</span><span class="sxs-lookup"><span data-stu-id="80c78-127">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="80c78-128">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="80c78-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="80c78-129">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="80c78-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="80c78-130">seriesCount</span><span class="sxs-lookup"><span data-stu-id="80c78-130">seriesCount</span></span>|<span data-ttu-id="80c78-131">Int64</span><span class="sxs-lookup"><span data-stu-id="80c78-131">Int64</span></span>|<span data-ttu-id="80c78-132">Wie oft dieser Serie aus der Quarantäne wurde erneut ausgewertet und Links in Kraft (eine Datenreihe beginnt, wenn Quarantäne wird zuerst eingeführt und wird als Quarantäne transformiert wird zurückgesetzt).</span><span class="sxs-lookup"><span data-stu-id="80c78-132">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="80c78-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="80c78-133">JSON representation</span></span>

<span data-ttu-id="80c78-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="80c78-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationQuarantine"
}-->

```json
{
  "currentBegan": "String (timestamp)",
  "nextAttempt": "String (timestamp)",
  "reason": "String",
  "seriesBegan": "String (timestamp)",
  "seriesCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationQuarantine resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->