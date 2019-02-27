---
title: mediaContentRatingIreland-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a17ea1ddbd4e63af846ab6343f66f4a5726e9739
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140978"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="970a8-103">mediaContentRatingIreland-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="970a8-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="970a8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="970a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="970a8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="970a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="970a8-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="970a8-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="970a8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="970a8-107">Properties</span></span>
|<span data-ttu-id="970a8-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="970a8-108">Property</span></span>|<span data-ttu-id="970a8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="970a8-109">Type</span></span>|<span data-ttu-id="970a8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="970a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="970a8-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="970a8-111">movieRating</span></span>|[<span data-ttu-id="970a8-112">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="970a8-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="970a8-113">Film Bewertung für Irland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="970a8-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="970a8-114">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="970a8-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="970a8-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="970a8-115">tvRating</span></span>|[<span data-ttu-id="970a8-116">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="970a8-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="970a8-117">Für Irland ausgewählte TV-Bewertung.</span><span class="sxs-lookup"><span data-stu-id="970a8-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="970a8-118">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="970a8-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="970a8-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="970a8-119">Relationships</span></span>
<span data-ttu-id="970a8-120">Keine</span><span class="sxs-lookup"><span data-stu-id="970a8-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="970a8-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="970a8-121">JSON Representation</span></span>
<span data-ttu-id="970a8-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="970a8-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```




