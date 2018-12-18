---
title: mediaContentRatingUnitedKingdom-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 0fcd17f27d999f933ce6824f8a49018013341c7b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315533"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="79031-103">mediaContentRatingUnitedKingdom-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="79031-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="79031-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="79031-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79031-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="79031-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="79031-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="79031-106">Properties</span></span>
|<span data-ttu-id="79031-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="79031-107">Property</span></span>|<span data-ttu-id="79031-108">Typ</span><span class="sxs-lookup"><span data-stu-id="79031-108">Type</span></span>|<span data-ttu-id="79031-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79031-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79031-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="79031-110">movieRating</span></span>|[<span data-ttu-id="79031-111">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="79031-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="79031-112">Bewertung für Großbritannien ausgewählten Filme.</span><span class="sxs-lookup"><span data-stu-id="79031-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="79031-113">Mögliche Werte: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="79031-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="79031-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="79031-114">tvRating</span></span>|[<span data-ttu-id="79031-115">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="79031-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="79031-116">TV-Bewertung für Großbritannien ausgewählt.</span><span class="sxs-lookup"><span data-stu-id="79031-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="79031-117">Mögliche Werte sind: `allAllowed`, `allBlocked` und `caution`.</span><span class="sxs-lookup"><span data-stu-id="79031-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79031-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="79031-118">Relationships</span></span>
<span data-ttu-id="79031-119">Keine</span><span class="sxs-lookup"><span data-stu-id="79031-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="79031-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="79031-120">JSON Representation</span></span>
<span data-ttu-id="79031-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="79031-121">Here is a JSON representation of the resource.</span></span>
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



