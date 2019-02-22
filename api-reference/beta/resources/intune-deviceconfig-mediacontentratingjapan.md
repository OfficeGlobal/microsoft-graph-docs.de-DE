---
title: mediaContentRatingJapan-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b10d498edd03850a52aa09ba29e352a143a77c5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163441"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="e113c-103">mediaContentRatingJapan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e113c-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="e113c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e113c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e113c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e113c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e113c-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e113c-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e113c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e113c-107">Properties</span></span>
|<span data-ttu-id="e113c-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e113c-108">Property</span></span>|<span data-ttu-id="e113c-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e113c-109">Type</span></span>|<span data-ttu-id="e113c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e113c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e113c-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="e113c-111">movieRating</span></span>|[<span data-ttu-id="e113c-112">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="e113c-112">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="e113c-113">Ausgewählte Filme für Japan.</span><span class="sxs-lookup"><span data-stu-id="e113c-113">Movies rating selected for Japan.</span></span> <span data-ttu-id="e113c-114">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="e113c-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="e113c-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="e113c-115">tvRating</span></span>|[<span data-ttu-id="e113c-116">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e113c-116">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="e113c-117">TV-Bewertung für Japan ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="e113c-117">TV rating selected for Japan.</span></span> <span data-ttu-id="e113c-118">Mögliche Werte sind: `allAllowed`, `allBlocked` und `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="e113c-118">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e113c-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e113c-119">Relationships</span></span>
<span data-ttu-id="e113c-120">Keine</span><span class="sxs-lookup"><span data-stu-id="e113c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e113c-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e113c-121">JSON Representation</span></span>
<span data-ttu-id="e113c-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e113c-122">Here is a JSON representation of the resource.</span></span>
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




