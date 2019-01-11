---
title: Ressourcentyp synchronizationSchedule
description: Definiert den Zeitplan zum Ausführen einer SynchronizationJob verwendet.
localization_priority: Normal
ms.openlocfilehash: b59c36a36d837c21c147033dff8de66b85c863a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877868"
---
# <a name="synchronizationschedule-resource-type"></a><span data-ttu-id="f9738-103">Ressourcentyp synchronizationSchedule</span><span class="sxs-lookup"><span data-stu-id="f9738-103">synchronizationSchedule resource type</span></span>

> <span data-ttu-id="f9738-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f9738-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f9738-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f9738-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f9738-106">Definiert den Zeitplan zum Ausführen einer [SynchronizationJob](synchronization-synchronizationjob.md)verwendet.</span><span class="sxs-lookup"><span data-stu-id="f9738-106">Defines the schedule used to run a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f9738-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f9738-107">Properties</span></span>
| <span data-ttu-id="f9738-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f9738-108">Property</span></span>     | <span data-ttu-id="f9738-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f9738-109">Type</span></span>   |<span data-ttu-id="f9738-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f9738-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9738-111">Ablaufdatum</span><span class="sxs-lookup"><span data-stu-id="f9738-111">expiration</span></span>|<span data-ttu-id="f9738-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9738-112">DateTimeOffset</span></span>|<span data-ttu-id="f9738-113">Datum und Uhrzeit, wann dieser Auftrag abläuft.</span><span class="sxs-lookup"><span data-stu-id="f9738-113">Date and time when this job will expire.</span></span> <span data-ttu-id="f9738-114">Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben.</span><span class="sxs-lookup"><span data-stu-id="f9738-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f9738-115">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="f9738-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f9738-116">Intervall</span><span class="sxs-lookup"><span data-stu-id="f9738-116">interval</span></span>|<span data-ttu-id="f9738-117">Duration</span><span class="sxs-lookup"><span data-stu-id="f9738-117">Duration</span></span>|<span data-ttu-id="f9738-118">Das Intervall zwischen Synchronisierung Iterationen.</span><span class="sxs-lookup"><span data-stu-id="f9738-118">The interval between synchronization iterations.</span></span>|
|<span data-ttu-id="f9738-119">state</span><span class="sxs-lookup"><span data-stu-id="f9738-119">state</span></span>|<span data-ttu-id="f9738-120">String</span><span class="sxs-lookup"><span data-stu-id="f9738-120">String</span></span>| <span data-ttu-id="f9738-121">Mögliche Werte: `Active`, `Disabled`.</span><span class="sxs-lookup"><span data-stu-id="f9738-121">Possible values are: `Active`, `Disabled`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9738-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f9738-122">JSON representation</span></span>

<span data-ttu-id="f9738-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f9738-123">The following is a JSON representation of the resource.</span></span>

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
