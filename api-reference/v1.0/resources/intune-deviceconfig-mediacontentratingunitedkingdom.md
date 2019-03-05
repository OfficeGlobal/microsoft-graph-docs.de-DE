---
title: mediaContentRatingUnitedKingdom-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 947fd12d8219215b0828ef1c05d2d8b36f970f16
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252455"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="795cf-103">mediaContentRatingUnitedKingdom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="795cf-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="795cf-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="795cf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="795cf-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="795cf-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="795cf-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="795cf-106">Properties</span></span>
|<span data-ttu-id="795cf-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="795cf-107">Property</span></span>|<span data-ttu-id="795cf-108">Typ</span><span class="sxs-lookup"><span data-stu-id="795cf-108">Type</span></span>|<span data-ttu-id="795cf-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="795cf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="795cf-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="795cf-110">movieRating</span></span>|[<span data-ttu-id="795cf-111">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="795cf-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="795cf-112">Film Bewertung für Vereinigtes Königreich ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="795cf-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="795cf-113">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="795cf-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="795cf-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="795cf-114">tvRating</span></span>|[<span data-ttu-id="795cf-115">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="795cf-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="795cf-116">TV-Bewertung für Großbritannien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="795cf-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="795cf-117">Mögliche Werte sind: `allAllowed`, `allBlocked` und `caution`.</span><span class="sxs-lookup"><span data-stu-id="795cf-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="795cf-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="795cf-118">Relationships</span></span>
<span data-ttu-id="795cf-119">Keine</span><span class="sxs-lookup"><span data-stu-id="795cf-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="795cf-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="795cf-120">JSON Representation</span></span>
<span data-ttu-id="795cf-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="795cf-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```



