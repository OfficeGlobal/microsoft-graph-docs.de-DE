---
title: mediaContentRatingIreland-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 153164010b6beda5d38779f67ffcd0654a1c986a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252637"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="c523a-103">mediaContentRatingIreland-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c523a-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="c523a-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c523a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c523a-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c523a-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c523a-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c523a-106">Properties</span></span>
|<span data-ttu-id="c523a-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c523a-107">Property</span></span>|<span data-ttu-id="c523a-108">Typ</span><span class="sxs-lookup"><span data-stu-id="c523a-108">Type</span></span>|<span data-ttu-id="c523a-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c523a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c523a-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="c523a-110">movieRating</span></span>|[<span data-ttu-id="c523a-111">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="c523a-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="c523a-112">Film Bewertung für Irland ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="c523a-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="c523a-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="c523a-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="c523a-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="c523a-114">tvRating</span></span>|[<span data-ttu-id="c523a-115">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c523a-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="c523a-116">Für Irland ausgewählte TV-Bewertung.</span><span class="sxs-lookup"><span data-stu-id="c523a-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="c523a-117">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="c523a-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c523a-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c523a-118">Relationships</span></span>
<span data-ttu-id="c523a-119">Keine</span><span class="sxs-lookup"><span data-stu-id="c523a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c523a-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c523a-120">JSON Representation</span></span>
<span data-ttu-id="c523a-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c523a-121">Here is a JSON representation of the resource.</span></span>
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



