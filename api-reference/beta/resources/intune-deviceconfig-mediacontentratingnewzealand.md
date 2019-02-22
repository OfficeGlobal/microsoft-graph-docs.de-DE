---
title: mediaContentRatingNewZealand-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9328ccc8b3c6b7ce6af220d8f798497e00448a8b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159276"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="2ffe8-103">mediaContentRatingNewZealand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2ffe8-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="2ffe8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2ffe8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ffe8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2ffe8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ffe8-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2ffe8-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2ffe8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2ffe8-107">Properties</span></span>
|<span data-ttu-id="2ffe8-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2ffe8-108">Property</span></span>|<span data-ttu-id="2ffe8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="2ffe8-109">Type</span></span>|<span data-ttu-id="2ffe8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ffe8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ffe8-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="2ffe8-111">movieRating</span></span>|[<span data-ttu-id="2ffe8-112">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="2ffe8-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="2ffe8-113">Ausgewählte Filme für Neuseeland.</span><span class="sxs-lookup"><span data-stu-id="2ffe8-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="2ffe8-114">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="2ffe8-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="2ffe8-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="2ffe8-115">tvRating</span></span>|[<span data-ttu-id="2ffe8-116">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="2ffe8-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="2ffe8-117">TV-Bewertung für Neuseeland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="2ffe8-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="2ffe8-118">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="2ffe8-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ffe8-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2ffe8-119">Relationships</span></span>
<span data-ttu-id="2ffe8-120">Keine</span><span class="sxs-lookup"><span data-stu-id="2ffe8-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ffe8-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2ffe8-121">JSON Representation</span></span>
<span data-ttu-id="2ffe8-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2ffe8-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```




