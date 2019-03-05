---
title: mediaContentRatingNewZealand-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c2d9d58413153699f93841470364cb673979a17
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253400"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="6542a-103">mediaContentRatingNewZealand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6542a-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="6542a-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6542a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6542a-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6542a-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6542a-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6542a-106">Properties</span></span>
|<span data-ttu-id="6542a-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6542a-107">Property</span></span>|<span data-ttu-id="6542a-108">Typ</span><span class="sxs-lookup"><span data-stu-id="6542a-108">Type</span></span>|<span data-ttu-id="6542a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6542a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6542a-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="6542a-110">movieRating</span></span>|[<span data-ttu-id="6542a-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="6542a-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="6542a-112">Ausgewählte Filme für Neuseeland.</span><span class="sxs-lookup"><span data-stu-id="6542a-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="6542a-113">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="6542a-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="6542a-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="6542a-114">tvRating</span></span>|[<span data-ttu-id="6542a-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="6542a-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="6542a-116">TV-Bewertung für Neuseeland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="6542a-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="6542a-117">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="6542a-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6542a-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6542a-118">Relationships</span></span>
<span data-ttu-id="6542a-119">Keine</span><span class="sxs-lookup"><span data-stu-id="6542a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6542a-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6542a-120">JSON Representation</span></span>
<span data-ttu-id="6542a-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6542a-121">Here is a JSON representation of the resource.</span></span>
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



