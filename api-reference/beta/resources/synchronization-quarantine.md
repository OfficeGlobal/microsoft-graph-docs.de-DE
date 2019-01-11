---
title: Ressourcentyp synchronizationQuarantine
description: Enthält Informationen zu den Quarantäne Status einer SynchronizationJob.
localization_priority: Normal
ms.openlocfilehash: fba0077d48e69ed4c2c190d0b50a6fcfc1749626
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849728"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="8313b-103">Ressourcentyp synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="8313b-103">synchronizationQuarantine resource type</span></span>

> <span data-ttu-id="8313b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8313b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8313b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8313b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8313b-106">Enthält Informationen zu den Quarantäne Status einer [SynchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="8313b-106">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8313b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8313b-107">Properties</span></span>
| <span data-ttu-id="8313b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8313b-108">Property</span></span>     | <span data-ttu-id="8313b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="8313b-109">Type</span></span>   |<span data-ttu-id="8313b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8313b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8313b-111">currentBegan</span><span class="sxs-lookup"><span data-stu-id="8313b-111">currentBegan</span></span>|<span data-ttu-id="8313b-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8313b-112">DateTimeOffset</span></span>|<span data-ttu-id="8313b-113">Datum und Uhrzeit, wann die Quarantäne letzten, ausgewertet und eingeführt.</span><span class="sxs-lookup"><span data-stu-id="8313b-113">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="8313b-114">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="8313b-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8313b-115">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8313b-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8313b-116">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="8313b-116">nextAttempt</span></span>|<span data-ttu-id="8313b-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8313b-117">DateTimeOffset</span></span>|<span data-ttu-id="8313b-118">Datum und Uhrzeit beim nächste Versuch die Quarantäne für die Überprüfung erfolgt.</span><span class="sxs-lookup"><span data-stu-id="8313b-118">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="8313b-119">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="8313b-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8313b-120">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8313b-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8313b-121">Grund</span><span class="sxs-lookup"><span data-stu-id="8313b-121">reason</span></span>|<span data-ttu-id="8313b-122">String</span><span class="sxs-lookup"><span data-stu-id="8313b-122">String</span></span>|<span data-ttu-id="8313b-123">Ein Code, der angibt, warum die Quarantäne eingeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="8313b-123">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="8313b-124">Mögliche Werte sind: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException` und `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="8313b-124">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span></span>|
|<span data-ttu-id="8313b-125">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="8313b-125">seriesBegan</span></span>|<span data-ttu-id="8313b-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8313b-126">DateTimeOffset</span></span>|<span data-ttu-id="8313b-127">Datum und Uhrzeit, als die Quarantäne zunächst, in dieser Reihe (eine Datenreihe beginnt eingeführt wurde, wenn eine Quarantäne wird zuerst eingeführt und wird zurückgesetzt, sobald die Quarantäne transformiert ist).</span><span class="sxs-lookup"><span data-stu-id="8313b-127">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="8313b-128">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="8313b-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8313b-129">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="8313b-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8313b-130">seriesCount</span><span class="sxs-lookup"><span data-stu-id="8313b-130">seriesCount</span></span>|<span data-ttu-id="8313b-131">Int64</span><span class="sxs-lookup"><span data-stu-id="8313b-131">Int64</span></span>|<span data-ttu-id="8313b-132">Wie oft dieser Serie aus der Quarantäne wurde erneut ausgewertet und Links in Kraft (eine Datenreihe beginnt, wenn Quarantäne wird zuerst eingeführt und wird als Quarantäne transformiert wird zurückgesetzt).</span><span class="sxs-lookup"><span data-stu-id="8313b-132">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8313b-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8313b-133">JSON representation</span></span>

<span data-ttu-id="8313b-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8313b-134">The following is a JSON representation of the resource.</span></span>

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
