---
title: mediaContentRatingUnitedStates-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 130b74fa3cf0a5424f7ad816107b80101b9cee49
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161901"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="b2538-103">mediaContentRatingUnitedStates-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b2538-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="b2538-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b2538-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2538-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b2538-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2538-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b2538-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b2538-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b2538-107">Properties</span></span>
|<span data-ttu-id="b2538-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b2538-108">Property</span></span>|<span data-ttu-id="b2538-109">Typ</span><span class="sxs-lookup"><span data-stu-id="b2538-109">Type</span></span>|<span data-ttu-id="b2538-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2538-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2538-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="b2538-111">movieRating</span></span>|[<span data-ttu-id="b2538-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="b2538-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="b2538-113">Film Bewertung für USA ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="b2538-113">Movies rating selected for United States.</span></span> <span data-ttu-id="b2538-114">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted` und `adults`.</span><span class="sxs-lookup"><span data-stu-id="b2538-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="b2538-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="b2538-115">tvRating</span></span>|[<span data-ttu-id="b2538-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b2538-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="b2538-117">TV-Bewertung für USA ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="b2538-117">TV rating selected for United States.</span></span> <span data-ttu-id="b2538-118">Mögliche Werte: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="b2538-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2538-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b2538-119">Relationships</span></span>
<span data-ttu-id="b2538-120">Keine</span><span class="sxs-lookup"><span data-stu-id="b2538-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2538-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b2538-121">JSON Representation</span></span>
<span data-ttu-id="b2538-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b2538-122">Here is a JSON representation of the resource.</span></span>
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




