---
title: mediaContentRatingJapan-Ressourcentyp
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1c129fb2853025758fc71aff381efe500d38ec8f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394838"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="6fe1d-103">mediaContentRatingJapan-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6fe1d-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="6fe1d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6fe1d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6fe1d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6fe1d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6fe1d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6fe1d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fe1d-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="6fe1d-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6fe1d-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6fe1d-108">Properties</span></span>
|<span data-ttu-id="6fe1d-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6fe1d-109">Property</span></span>|<span data-ttu-id="6fe1d-110">Typ</span><span class="sxs-lookup"><span data-stu-id="6fe1d-110">Type</span></span>|<span data-ttu-id="6fe1d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6fe1d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fe1d-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="6fe1d-112">movieRating</span></span>|[<span data-ttu-id="6fe1d-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="6fe1d-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="6fe1d-114">Bewertung für Japan ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="6fe1d-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="6fe1d-115">Mögliche Werte sind: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15` und `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="6fe1d-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="6fe1d-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="6fe1d-116">tvRating</span></span>|[<span data-ttu-id="6fe1d-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="6fe1d-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="6fe1d-118">TV-Bewertung für Japan ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="6fe1d-118">TV rating selected for Japan.</span></span> <span data-ttu-id="6fe1d-119">Mögliche Werte sind: `allAllowed`, `allBlocked` und `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="6fe1d-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fe1d-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6fe1d-120">Relationships</span></span>
<span data-ttu-id="6fe1d-121">Keine</span><span class="sxs-lookup"><span data-stu-id="6fe1d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6fe1d-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6fe1d-122">JSON Representation</span></span>
<span data-ttu-id="6fe1d-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6fe1d-123">Here is a JSON representation of the resource.</span></span>
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




