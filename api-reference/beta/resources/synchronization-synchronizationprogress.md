---
title: Ressourcentyp synchronizationProgress
description: Stellt den Fortschritt des ein SynchronizationJob an.
localization_priority: Normal
ms.openlocfilehash: 3c1168cdac6a073842cb5e08d165572591d2d8e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885386"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="de7ee-103">Ressourcentyp synchronizationProgress</span><span class="sxs-lookup"><span data-stu-id="de7ee-103">synchronizationProgress resource type</span></span>

> <span data-ttu-id="de7ee-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="de7ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de7ee-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="de7ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="de7ee-106">Stellt den Fortschritt des ein [SynchronizationJob](synchronization-synchronizationjob.md) an.</span><span class="sxs-lookup"><span data-stu-id="de7ee-106">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="de7ee-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="de7ee-107">Properties</span></span>

| <span data-ttu-id="de7ee-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="de7ee-108">Property</span></span>                              | <span data-ttu-id="de7ee-109">Typ</span><span class="sxs-lookup"><span data-stu-id="de7ee-109">Type</span></span>      | <span data-ttu-id="de7ee-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de7ee-110">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="de7ee-111">completedUnits</span><span class="sxs-lookup"><span data-stu-id="de7ee-111">completedUnits</span></span>|<span data-ttu-id="de7ee-112">Int32</span><span class="sxs-lookup"><span data-stu-id="de7ee-112">Int32</span></span>|<span data-ttu-id="de7ee-113">Die Zähler Fortschritt das Verhältnis der; die Anzahl der Einheiten von Änderungen, die bereits verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="de7ee-113">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="de7ee-114">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="de7ee-114">progressObservationDateTime</span></span>|<span data-ttu-id="de7ee-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de7ee-115">DateTimeOffset</span></span>|<span data-ttu-id="de7ee-116">Der Zeitpunkt der eine Beobachtung Fortschritt als Offset in Minuten aus UTC.</span><span class="sxs-lookup"><span data-stu-id="de7ee-116">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="de7ee-117">totalUnits</span><span class="sxs-lookup"><span data-stu-id="de7ee-117">totalUnits</span></span>|<span data-ttu-id="de7ee-118">Int32</span><span class="sxs-lookup"><span data-stu-id="de7ee-118">Int32</span></span>|<span data-ttu-id="de7ee-119">Die als Nenner des Fortschritts das Verhältnis der; eine Anzahl von Einheiten Änderungen verarbeitet werden, um die Synchronisierung ausführen.</span><span class="sxs-lookup"><span data-stu-id="de7ee-119">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="de7ee-120">Einheiten</span><span class="sxs-lookup"><span data-stu-id="de7ee-120">units</span></span>|<span data-ttu-id="de7ee-121">String</span><span class="sxs-lookup"><span data-stu-id="de7ee-121">String</span></span>|<span data-ttu-id="de7ee-122">Eine optionale Beschreibung der Einheiten.</span><span class="sxs-lookup"><span data-stu-id="de7ee-122">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="de7ee-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="de7ee-123">JSON representation</span></span>

<span data-ttu-id="de7ee-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="de7ee-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
}-->

```json
{
  "completedUnits": 1025,
  "progressObservationDateTime": "2017-10-10T17:00:00Z",
  "totalUnits": 3024,
  "units": "pages"
}

```

<!-- uuid: 15571993-7e2f-4842-84d5-01ceb67cdc05
20185-08-14 22:30:00 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
