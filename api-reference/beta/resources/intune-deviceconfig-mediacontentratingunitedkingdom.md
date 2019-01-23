---
title: mediaContentRatingUnitedKingdom-Ressourcentyp
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7d21ac4650072c4523f9e120d5d73ad393686635
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408075"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="e58b8-103">mediaContentRatingUnitedKingdom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e58b8-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="e58b8-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="e58b8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e58b8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e58b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e58b8-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e58b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e58b8-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="e58b8-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e58b8-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e58b8-108">Properties</span></span>
|<span data-ttu-id="e58b8-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e58b8-109">Property</span></span>|<span data-ttu-id="e58b8-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e58b8-110">Type</span></span>|<span data-ttu-id="e58b8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e58b8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e58b8-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="e58b8-112">movieRating</span></span>|[<span data-ttu-id="e58b8-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="e58b8-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="e58b8-114">Bewertung für Großbritannien ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="e58b8-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="e58b8-115">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="e58b8-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="e58b8-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="e58b8-116">tvRating</span></span>|[<span data-ttu-id="e58b8-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e58b8-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="e58b8-118">TV-Bewertung für Großbritannien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="e58b8-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="e58b8-119">Mögliche Werte sind: `allAllowed`, `allBlocked` und `caution`.</span><span class="sxs-lookup"><span data-stu-id="e58b8-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e58b8-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e58b8-120">Relationships</span></span>
<span data-ttu-id="e58b8-121">Keine</span><span class="sxs-lookup"><span data-stu-id="e58b8-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e58b8-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e58b8-122">JSON Representation</span></span>
<span data-ttu-id="e58b8-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e58b8-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```




