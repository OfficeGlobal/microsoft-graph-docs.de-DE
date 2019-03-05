---
title: mediaContentRatingJapan-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0543aec86312d90a5896ed3f06f004c87d8e6a58
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250306"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="9e6c9-103">mediaContentRatingJapan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9e6c9-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="9e6c9-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9e6c9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e6c9-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9e6c9-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9e6c9-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9e6c9-106">Properties</span></span>
|<span data-ttu-id="9e6c9-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9e6c9-107">Property</span></span>|<span data-ttu-id="9e6c9-108">Typ</span><span class="sxs-lookup"><span data-stu-id="9e6c9-108">Type</span></span>|<span data-ttu-id="9e6c9-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e6c9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e6c9-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="9e6c9-110">movieRating</span></span>|[<span data-ttu-id="9e6c9-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="9e6c9-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="9e6c9-112">Ausgewählte Filme für Japan.</span><span class="sxs-lookup"><span data-stu-id="9e6c9-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="9e6c9-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="9e6c9-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="9e6c9-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="9e6c9-114">tvRating</span></span>|[<span data-ttu-id="9e6c9-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="9e6c9-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="9e6c9-116">TV-Bewertung für Japan ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="9e6c9-116">TV rating selected for Japan.</span></span> <span data-ttu-id="9e6c9-117">Mögliche Werte sind: `allAllowed`, `allBlocked` und `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="9e6c9-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e6c9-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9e6c9-118">Relationships</span></span>
<span data-ttu-id="9e6c9-119">Keine</span><span class="sxs-lookup"><span data-stu-id="9e6c9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e6c9-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9e6c9-120">JSON Representation</span></span>
<span data-ttu-id="9e6c9-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9e6c9-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```



