---
title: mediaContentRatingUnitedKingdom-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8bdcd67bbc81cb5436c6be22c395a6c9804b0637
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951593"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="bff6c-103">mediaContentRatingUnitedKingdom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bff6c-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="bff6c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bff6c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bff6c-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bff6c-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="bff6c-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bff6c-106">Properties</span></span>
|<span data-ttu-id="bff6c-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bff6c-107">Property</span></span>|<span data-ttu-id="bff6c-108">Typ</span><span class="sxs-lookup"><span data-stu-id="bff6c-108">Type</span></span>|<span data-ttu-id="bff6c-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bff6c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bff6c-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="bff6c-110">movieRating</span></span>|[<span data-ttu-id="bff6c-111">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="bff6c-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="bff6c-112">Bewertung für Großbritannien ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="bff6c-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="bff6c-113">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="bff6c-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="bff6c-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="bff6c-114">tvRating</span></span>|[<span data-ttu-id="bff6c-115">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="bff6c-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="bff6c-116">TV-Bewertung für Großbritannien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="bff6c-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="bff6c-117">Mögliche Werte sind: `allAllowed`, `allBlocked` und `caution`.</span><span class="sxs-lookup"><span data-stu-id="bff6c-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bff6c-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bff6c-118">Relationships</span></span>
<span data-ttu-id="bff6c-119">Keine</span><span class="sxs-lookup"><span data-stu-id="bff6c-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bff6c-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bff6c-120">JSON Representation</span></span>
<span data-ttu-id="bff6c-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bff6c-121">Here is a JSON representation of the resource.</span></span>
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



