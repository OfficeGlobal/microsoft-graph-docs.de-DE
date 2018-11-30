---
title: Ressourcentyp synchronizationSchedule
description: Definiert den Zeitplan zum Ausführen einer SynchronizationJob verwendet.
ms.openlocfilehash: c0435b3957f138751f34a1e0e522683b352294da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061900"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="d31b9-103">Ressourcentyp synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="d31b9-103">synchronizationSchedule resource type</span></span>

> <span data-ttu-id="d31b9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d31b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d31b9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d31b9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d31b9-106">Definiert den Zeitplan zum Ausführen einer [SynchronizationJob](synchronization-synchronizationjob.md)verwendet.</span><span class="sxs-lookup"><span data-stu-id="d31b9-106">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d31b9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d31b9-107">Properties</span></span>
| <span data-ttu-id="d31b9-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d31b9-108">Property</span></span>     | <span data-ttu-id="d31b9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d31b9-109">Type</span></span>   |<span data-ttu-id="d31b9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d31b9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d31b9-111">Ablaufdatum</span><span class="sxs-lookup"><span data-stu-id="d31b9-111">expiration</span></span>|<span data-ttu-id="d31b9-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d31b9-112">DateTimeOffset</span></span>|<span data-ttu-id="d31b9-113">Datum und Uhrzeit, wann dieser Auftrag abläuft.</span><span class="sxs-lookup"><span data-stu-id="d31b9-113">Date and time when this job will expire.</span></span> <span data-ttu-id="d31b9-114">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="d31b9-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d31b9-115">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="d31b9-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="d31b9-116">Intervall</span><span class="sxs-lookup"><span data-stu-id="d31b9-116">interval</span></span>|<span data-ttu-id="d31b9-117">Duration</span><span class="sxs-lookup"><span data-stu-id="d31b9-117">Duration</span></span>|<span data-ttu-id="d31b9-118">Das Intervall zwischen Synchronisierung Iterationen.</span><span class="sxs-lookup"><span data-stu-id="d31b9-118">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="d31b9-119">state</span><span class="sxs-lookup"><span data-stu-id="d31b9-119">state</span></span>|<span data-ttu-id="d31b9-120">String</span><span class="sxs-lookup"><span data-stu-id="d31b9-120">String</span></span>| <span data-ttu-id="d31b9-121">Mögliche Werte: `Active`, `Disabled`.</span><span class="sxs-lookup"><span data-stu-id="d31b9-121">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d31b9-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d31b9-122">JSON representation</span></span>

<span data-ttu-id="d31b9-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d31b9-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchedule"
}-->

```json
{
  "expiration": "String (timestamp)",
  "interval": "String (duration)",
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->