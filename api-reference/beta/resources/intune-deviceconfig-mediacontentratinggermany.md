---
title: mediaContentRatingGermany-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a43f919bb24d25d0e22dab0ecc192b2b6757f9e7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147096"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="b3063-103">mediaContentRatingGermany-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b3063-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="b3063-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b3063-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3063-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b3063-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3063-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b3063-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b3063-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b3063-107">Properties</span></span>
|<span data-ttu-id="b3063-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b3063-108">Property</span></span>|<span data-ttu-id="b3063-109">Typ</span><span class="sxs-lookup"><span data-stu-id="b3063-109">Type</span></span>|<span data-ttu-id="b3063-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3063-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3063-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="b3063-111">movieRating</span></span>|[<span data-ttu-id="b3063-112">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="b3063-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="b3063-113">Film Bewertung für Deutschland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="b3063-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="b3063-114">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="b3063-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="b3063-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="b3063-115">tvRating</span></span>|[<span data-ttu-id="b3063-116">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b3063-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="b3063-117">TV-Bewertung für Deutschland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="b3063-117">TV rating selected for Germany.</span></span> <span data-ttu-id="b3063-118">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="b3063-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3063-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b3063-119">Relationships</span></span>
<span data-ttu-id="b3063-120">Keine</span><span class="sxs-lookup"><span data-stu-id="b3063-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3063-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b3063-121">JSON Representation</span></span>
<span data-ttu-id="b3063-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b3063-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```




