---
title: Ressourcentyp synchronizationQuarantine
description: Enthält Informationen zu den Quarantäne Status einer SynchronizationJob.
localization_priority: Normal
ms.openlocfilehash: 6d5d5c3cbe96eda6b39833287e8efb6e0771b19a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518814"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="a263f-103">Ressourcentyp synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="a263f-103">synchronizationQuarantine resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a263f-104">Enthält Informationen zu den Quarantäne Status einer [SynchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="a263f-104">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a263f-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a263f-105">Properties</span></span>
| <span data-ttu-id="a263f-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a263f-106">Property</span></span>     | <span data-ttu-id="a263f-107">Typ</span><span class="sxs-lookup"><span data-stu-id="a263f-107">Type</span></span>   |<span data-ttu-id="a263f-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a263f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a263f-109">currentBegan</span><span class="sxs-lookup"><span data-stu-id="a263f-109">currentBegan</span></span>|<span data-ttu-id="a263f-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a263f-110">DateTimeOffset</span></span>|<span data-ttu-id="a263f-111">Datum und Uhrzeit, wann die Quarantäne letzten, ausgewertet und eingeführt.</span><span class="sxs-lookup"><span data-stu-id="a263f-111">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="a263f-112">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="a263f-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a263f-113">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a263f-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="a263f-114">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="a263f-114">nextAttempt</span></span>|<span data-ttu-id="a263f-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a263f-115">DateTimeOffset</span></span>|<span data-ttu-id="a263f-116">Datum und Uhrzeit beim nächste Versuch die Quarantäne für die Überprüfung erfolgt.</span><span class="sxs-lookup"><span data-stu-id="a263f-116">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="a263f-117">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="a263f-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a263f-118">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a263f-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="a263f-119">Grund</span><span class="sxs-lookup"><span data-stu-id="a263f-119">reason</span></span>|<span data-ttu-id="a263f-120">String</span><span class="sxs-lookup"><span data-stu-id="a263f-120">String</span></span>|<span data-ttu-id="a263f-121">Ein Code, der angibt, warum die Quarantäne eingeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="a263f-121">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="a263f-122">Mögliche Werte sind: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException` und `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="a263f-122">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span></span>|
|<span data-ttu-id="a263f-123">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="a263f-123">seriesBegan</span></span>|<span data-ttu-id="a263f-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a263f-124">DateTimeOffset</span></span>|<span data-ttu-id="a263f-125">Datum und Uhrzeit, als die Quarantäne zunächst, in dieser Reihe (eine Datenreihe beginnt eingeführt wurde, wenn eine Quarantäne wird zuerst eingeführt und wird zurückgesetzt, sobald die Quarantäne transformiert ist).</span><span class="sxs-lookup"><span data-stu-id="a263f-125">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="a263f-126">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="a263f-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a263f-127">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a263f-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="a263f-128">seriesCount</span><span class="sxs-lookup"><span data-stu-id="a263f-128">seriesCount</span></span>|<span data-ttu-id="a263f-129">Int64</span><span class="sxs-lookup"><span data-stu-id="a263f-129">Int64</span></span>|<span data-ttu-id="a263f-130">Wie oft dieser Serie aus der Quarantäne wurde erneut ausgewertet und Links in Kraft (eine Datenreihe beginnt, wenn Quarantäne wird zuerst eingeführt und wird als Quarantäne transformiert wird zurückgesetzt).</span><span class="sxs-lookup"><span data-stu-id="a263f-130">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a263f-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a263f-131">JSON representation</span></span>

<span data-ttu-id="a263f-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a263f-132">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationQuarantine resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-quarantine.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
