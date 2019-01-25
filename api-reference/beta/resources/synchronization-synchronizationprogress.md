---
title: Ressourcentyp synchronizationProgress
description: Stellt den Fortschritt des ein SynchronizationJob an.
localization_priority: Normal
ms.openlocfilehash: b22bd95f54a9f268524dc98a8d3df94fcc14f773
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510974"
---
# <a name="synchronizationprogress-resource-type"></a><span data-ttu-id="c6624-103">Ressourcentyp synchronizationProgress</span><span class="sxs-lookup"><span data-stu-id="c6624-103">synchronizationProgress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6624-104">Stellt den Fortschritt des ein [SynchronizationJob](synchronization-synchronizationjob.md) an.</span><span class="sxs-lookup"><span data-stu-id="c6624-104">Represents the progress of a [synchronizationJob](synchronization-synchronizationjob.md) toward completion.</span></span>

## <a name="properties"></a><span data-ttu-id="c6624-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c6624-105">Properties</span></span>

| <span data-ttu-id="c6624-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c6624-106">Property</span></span>                              | <span data-ttu-id="c6624-107">Typ</span><span class="sxs-lookup"><span data-stu-id="c6624-107">Type</span></span>      | <span data-ttu-id="c6624-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6624-108">Description</span></span>    |
|:--------------------------------------|:----------|:---------------|
|<span data-ttu-id="c6624-109">completedUnits</span><span class="sxs-lookup"><span data-stu-id="c6624-109">completedUnits</span></span>|<span data-ttu-id="c6624-110">Int32</span><span class="sxs-lookup"><span data-stu-id="c6624-110">Int32</span></span>|<span data-ttu-id="c6624-111">Die Zähler Fortschritt das Verhältnis der; die Anzahl der Einheiten von Änderungen, die bereits verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="c6624-111">The numerator of a progress ratio; the number of units of changes already processed.</span></span>|
|<span data-ttu-id="c6624-112">progressObservationDateTime</span><span class="sxs-lookup"><span data-stu-id="c6624-112">progressObservationDateTime</span></span>|<span data-ttu-id="c6624-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6624-113">DateTimeOffset</span></span>|<span data-ttu-id="c6624-114">Der Zeitpunkt der eine Beobachtung Fortschritt als Offset in Minuten aus UTC.</span><span class="sxs-lookup"><span data-stu-id="c6624-114">The time of a progress observation as an offset in minutes from UTC.</span></span>|
|<span data-ttu-id="c6624-115">totalUnits</span><span class="sxs-lookup"><span data-stu-id="c6624-115">totalUnits</span></span>|<span data-ttu-id="c6624-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c6624-116">Int32</span></span>|<span data-ttu-id="c6624-117">Die als Nenner des Fortschritts das Verhältnis der; eine Anzahl von Einheiten Änderungen verarbeitet werden, um die Synchronisierung ausführen.</span><span class="sxs-lookup"><span data-stu-id="c6624-117">The denominator of a progress ratio; a number of units of changes to be processed to accomplish synchronization.</span></span>|
|<span data-ttu-id="c6624-118">Einheiten: </span><span class="sxs-lookup"><span data-stu-id="c6624-118">units</span></span>|<span data-ttu-id="c6624-119">String</span><span class="sxs-lookup"><span data-stu-id="c6624-119">String</span></span>|<span data-ttu-id="c6624-120">Eine optionale Beschreibung der Einheiten.</span><span class="sxs-lookup"><span data-stu-id="c6624-120">An optional description of the units.</span></span>|

<!-- The troubleshootingUrl property is missing a description -->

## <a name="json-representation"></a><span data-ttu-id="c6624-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c6624-121">JSON representation</span></span>

<span data-ttu-id="c6624-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c6624-122">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationProcess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationprogress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
