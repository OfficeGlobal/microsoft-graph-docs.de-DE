---
title: mediaContentRatingAustralia-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37e42c3629e73d8dc629ba754583f8023c168b30
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259115"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="efdc3-103">mediaContentRatingAustralia-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="efdc3-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="efdc3-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="efdc3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efdc3-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="efdc3-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="efdc3-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="efdc3-106">Properties</span></span>
|<span data-ttu-id="efdc3-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="efdc3-107">Property</span></span>|<span data-ttu-id="efdc3-108">Typ</span><span class="sxs-lookup"><span data-stu-id="efdc3-108">Type</span></span>|<span data-ttu-id="efdc3-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="efdc3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efdc3-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="efdc3-110">movieRating</span></span>|[<span data-ttu-id="efdc3-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="efdc3-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="efdc3-112">Film Bewertung für Australien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="efdc3-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="efdc3-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="efdc3-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="efdc3-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="efdc3-114">tvRating</span></span>|[<span data-ttu-id="efdc3-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="efdc3-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="efdc3-116">TV-Bewertung für Australien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="efdc3-116">TV rating selected for Australia.</span></span> <span data-ttu-id="efdc3-117">Mögliche Werte: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="efdc3-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efdc3-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="efdc3-118">Relationships</span></span>
<span data-ttu-id="efdc3-119">Keine</span><span class="sxs-lookup"><span data-stu-id="efdc3-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="efdc3-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="efdc3-120">JSON Representation</span></span>
<span data-ttu-id="efdc3-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="efdc3-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```



