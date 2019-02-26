---
title: mediaContentRatingFrance-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 40883571c2c17b466dbc6740280c34f8efa55282
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165667"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="5d5d6-103">mediaContentRatingFrance-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5d5d6-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="5d5d6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5d5d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d5d6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5d5d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d5d6-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="5d5d6-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5d5d6-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5d5d6-107">Properties</span></span>
|<span data-ttu-id="5d5d6-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5d5d6-108">Property</span></span>|<span data-ttu-id="5d5d6-109">Typ</span><span class="sxs-lookup"><span data-stu-id="5d5d6-109">Type</span></span>|<span data-ttu-id="5d5d6-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d5d6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d5d6-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="5d5d6-111">movieRating</span></span>|[<span data-ttu-id="5d5d6-112">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="5d5d6-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="5d5d6-113">Ausgewählte Filme für Frankreich.</span><span class="sxs-lookup"><span data-stu-id="5d5d6-113">Movies rating selected for France.</span></span> <span data-ttu-id="5d5d6-114">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="5d5d6-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="5d5d6-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="5d5d6-115">tvRating</span></span>|[<span data-ttu-id="5d5d6-116">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="5d5d6-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="5d5d6-117">TV-Bewertung für Frankreich ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="5d5d6-117">TV rating selected for France.</span></span> <span data-ttu-id="5d5d6-118">Mögliche Werte sind: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="5d5d6-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d5d6-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5d5d6-119">Relationships</span></span>
<span data-ttu-id="5d5d6-120">Keine</span><span class="sxs-lookup"><span data-stu-id="5d5d6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d5d6-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5d5d6-121">JSON Representation</span></span>
<span data-ttu-id="5d5d6-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5d5d6-122">Here is a JSON representation of the resource.</span></span>
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




