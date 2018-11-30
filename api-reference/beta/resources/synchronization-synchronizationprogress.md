---
title: Ressourcentyp synchronizationProgress
description: Stellt den Fortschritt des ein SynchronizationJob an.
ms.openlocfilehash: 412b7754dac97a36efe082026ab360569c0fe789
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065763"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="a9e62-103">Ressourcentyp synchronizationProgress</span><span class="sxs-lookup"><span data-stu-id="a9e62-103">synchronizationProgress resource type</span></span>

> <span data-ttu-id="a9e62-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a9e62-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9e62-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a9e62-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a9e62-106">Stellt den Fortschritt des ein [SynchronizationJob](synchronization-synchronizationjob.md) an.</span><span class="sxs-lookup"><span data-stu-id="a9e62-106">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="a9e62-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a9e62-107">Properties</span></span>

| <span data-ttu-id="a9e62-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a9e62-108">Property</span></span>                              | <span data-ttu-id="a9e62-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a9e62-109">Type</span></span>      | <span data-ttu-id="a9e62-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a9e62-110">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="a9e62-111">completedUnits</span><span class="sxs-lookup"><span data-stu-id="a9e62-111">completedUnits</span></span>|<span data-ttu-id="a9e62-112">Int32</span><span class="sxs-lookup"><span data-stu-id="a9e62-112">Int32</span></span>|<span data-ttu-id="a9e62-113">Die Zähler Fortschritt das Verhältnis der; die Anzahl der Einheiten von Änderungen, die bereits verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="a9e62-113">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="a9e62-114">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="a9e62-114">progressObservationDateTime</span></span>|<span data-ttu-id="a9e62-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9e62-115">DateTimeOffset</span></span>|<span data-ttu-id="a9e62-116">Der Zeitpunkt der eine Beobachtung Fortschritt als Offset in Minuten aus UTC.</span><span class="sxs-lookup"><span data-stu-id="a9e62-116">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="a9e62-117">totalUnits</span><span class="sxs-lookup"><span data-stu-id="a9e62-117">totalUnits</span></span>|<span data-ttu-id="a9e62-118">Int32</span><span class="sxs-lookup"><span data-stu-id="a9e62-118">Int32</span></span>|<span data-ttu-id="a9e62-119">Die als Nenner des Fortschritts das Verhältnis der; eine Anzahl von Einheiten Änderungen verarbeitet werden, um die Synchronisierung ausführen.</span><span class="sxs-lookup"><span data-stu-id="a9e62-119">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="a9e62-120">Einheiten</span><span class="sxs-lookup"><span data-stu-id="a9e62-120">units</span></span>|<span data-ttu-id="a9e62-121">String</span><span class="sxs-lookup"><span data-stu-id="a9e62-121">String</span></span>|<span data-ttu-id="a9e62-122">Eine optionale Beschreibung der Einheiten.</span><span class="sxs-lookup"><span data-stu-id="a9e62-122">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="a9e62-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a9e62-123">JSON representation</span></span>

<span data-ttu-id="a9e62-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a9e62-124">The following is a JSON representation of the resource.</span></span>

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
