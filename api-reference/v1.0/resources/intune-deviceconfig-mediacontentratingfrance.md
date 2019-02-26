---
title: mediaContentRatingFrance-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 979a5996b655ba13847e52dc09b083169ff0815a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260228"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="5dcd6-103">mediaContentRatingFrance-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5dcd6-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="5dcd6-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5dcd6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dcd6-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="5dcd6-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5dcd6-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5dcd6-106">Properties</span></span>
|<span data-ttu-id="5dcd6-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5dcd6-107">Property</span></span>|<span data-ttu-id="5dcd6-108">Typ</span><span class="sxs-lookup"><span data-stu-id="5dcd6-108">Type</span></span>|<span data-ttu-id="5dcd6-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5dcd6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dcd6-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="5dcd6-110">movieRating</span></span>|[<span data-ttu-id="5dcd6-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="5dcd6-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="5dcd6-112">Ausgewählte Filme für Frankreich.</span><span class="sxs-lookup"><span data-stu-id="5dcd6-112">Movies rating selected for France.</span></span> <span data-ttu-id="5dcd6-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="5dcd6-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="5dcd6-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="5dcd6-114">tvRating</span></span>|[<span data-ttu-id="5dcd6-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="5dcd6-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="5dcd6-116">TV-Bewertung für Frankreich ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="5dcd6-116">TV rating selected for France.</span></span> <span data-ttu-id="5dcd6-117">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="5dcd6-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5dcd6-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5dcd6-118">Relationships</span></span>
<span data-ttu-id="5dcd6-119">Keine</span><span class="sxs-lookup"><span data-stu-id="5dcd6-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5dcd6-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5dcd6-120">JSON Representation</span></span>
<span data-ttu-id="5dcd6-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5dcd6-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



