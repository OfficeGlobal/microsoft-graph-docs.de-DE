---
title: mediaContentRatingUnitedKingdom-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0169e26be7590031ba5e7e7f676d51f69a526452
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160179"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="f37ab-103">mediaContentRatingUnitedKingdom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f37ab-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="f37ab-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f37ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f37ab-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f37ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f37ab-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f37ab-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f37ab-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f37ab-107">Properties</span></span>
|<span data-ttu-id="f37ab-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f37ab-108">Property</span></span>|<span data-ttu-id="f37ab-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f37ab-109">Type</span></span>|<span data-ttu-id="f37ab-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f37ab-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f37ab-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="f37ab-111">movieRating</span></span>|[<span data-ttu-id="f37ab-112">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="f37ab-112">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="f37ab-113">Film Bewertung für Vereinigtes Königreich ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="f37ab-113">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="f37ab-114">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="f37ab-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="f37ab-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="f37ab-115">tvRating</span></span>|[<span data-ttu-id="f37ab-116">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f37ab-116">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="f37ab-117">TV-Bewertung für Großbritannien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="f37ab-117">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="f37ab-118">Mögliche Werte sind: `allAllowed`, `allBlocked` und `caution`.</span><span class="sxs-lookup"><span data-stu-id="f37ab-118">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f37ab-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f37ab-119">Relationships</span></span>
<span data-ttu-id="f37ab-120">Keine</span><span class="sxs-lookup"><span data-stu-id="f37ab-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f37ab-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f37ab-121">JSON Representation</span></span>
<span data-ttu-id="f37ab-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f37ab-122">Here is a JSON representation of the resource.</span></span>
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




