---
title: mediaContentRatingUnitedStates-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: baa5d98f0fcb1d267221c95c0b27be988d3a197f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254730"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="8d36b-103">mediaContentRatingUnitedStates-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8d36b-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="8d36b-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8d36b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d36b-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="8d36b-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8d36b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8d36b-106">Properties</span></span>
|<span data-ttu-id="8d36b-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8d36b-107">Property</span></span>|<span data-ttu-id="8d36b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="8d36b-108">Type</span></span>|<span data-ttu-id="8d36b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8d36b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d36b-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="8d36b-110">movieRating</span></span>|[<span data-ttu-id="8d36b-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="8d36b-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="8d36b-112">Film Bewertung für USA ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="8d36b-112">Movies rating selected for United States.</span></span> <span data-ttu-id="8d36b-113">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="8d36b-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="8d36b-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="8d36b-114">tvRating</span></span>|[<span data-ttu-id="8d36b-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8d36b-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="8d36b-116">TV-Bewertung für USA ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="8d36b-116">TV rating selected for United States.</span></span> <span data-ttu-id="8d36b-117">Mögliche Werte: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="8d36b-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d36b-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8d36b-118">Relationships</span></span>
<span data-ttu-id="8d36b-119">Keine</span><span class="sxs-lookup"><span data-stu-id="8d36b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d36b-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8d36b-120">JSON Representation</span></span>
<span data-ttu-id="8d36b-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8d36b-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```



